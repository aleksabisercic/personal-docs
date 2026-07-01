---
tags:
  - ai-tips
  - claude-code
  - agents
  - workflow
  - testing
  - e2e
  - skills
category: prompts
created: 2026-07-01
language: en
summary: Claude Code skill that drives a real running app (Electron, web, or dev server) from the terminal for manual end-to-end verification — attaching via Chrome DevTools Protocol or Playwright to click, inspect the DOM, evaluate JS, and read console/network output before claiming a change works.
---

# Manual E2E Skill: driving a running app for verification

A drop-in Claude Code **skill** (not a paste-in prompt) — the procedural field guide for proving user-visible behavior against the *real running application*, not mocks. It tells an agent when a manual pass is worth doing, how to attach to the app, how to run a disciplined pass, and what to do with the result. Trigger it whenever the task is "test the app", reproduce a UI bug, or confirm a change works end to end.

---

## When to Use It

- The task is to verify user-visible behavior of a running app (clicking around, checking the DOM, reading console/network output).
- You're reproducing or investigating a UI bug.
- You're confirming a change works end to end — the real main process, IPC/preload bridge, permissions, auth, or file system that mocks can't cover.
- Any hands-on "testing the app" request, even when the user never says "E2E".

---

## Skill Definition (drop into `.claude/skills/`)

````markdown
---
name: manual-e2e
description: Drive a real running app (Electron, web, or local dev server) from the terminal for manual end-to-end verification — clicking around, inspecting the DOM, evaluating JS, and reading console/network output via Chrome DevTools Protocol or Playwright. Use this skill whenever the task involves verifying user-visible behavior of a running app, reproducing or investigating a UI bug, checking that a change works end-to-end, or "testing the app" in any hands-on sense — even if the user doesn't say "E2E".
---

# Manual E2E: driving a running app for verification

This skill is the procedural field guide for proving user-visible behavior against the *real running application*, not mocks. It covers when a manual pass is appropriate, how to attach to the app, how to run a disciplined pass, and what to do with the result.

## Scope discipline (read first)

- Manual E2E is for **one of three things**: proving the behavior relevant to the current change, investigating a user-visible bug, or checking an integration that mocks can't cover (real main process, IPC/preload bridge, permissions, auth, file system).
- **Before starting, write down the one user-visible behavior you need to prove**, phrased as a checkable assertion (e.g., "clicking Save persists the note across app restart"). Keep the pass narrow unless the task explicitly asks for a broader product sweep.
- Repeatable product verification belongs in **automated tests**, not repeated manual passes. Pyramid: colocated unit/component tests (Vitest/Jest) for pure logic, services, adapters, and components; a focused automated E2E spec (Playwright) only when the assertion needs the real runtime; manual passes only for the three cases above.
- If a manual pass proves something worth keeping, **promote it**: write it as a permanent automated spec before closing the task, so it never regresses silently.
- Do not add feature-specific items to any permanent manual checklist unless a human explicitly asks.

## Attaching to the app

Pick the lightest mechanism that reaches the real runtime:

**Electron apps** — launch with remote debugging enabled, then attach via Chrome DevTools Protocol (CDP):
1. Start the app with `--remote-debugging-port=9222` (or the project's dev script if it already exposes one).
2. List targets: `curl -s http://localhost:9222/json` → grab the `webSocketDebuggerUrl` of the renderer page.
3. Drive it with a CDP client (`chrome-devtools` MCP if available, `playwright`'s `_electron.launch()` / `connectOverCDP`, or raw WebSocket + CDP commands: `Runtime.evaluate`, `DOM.querySelector`, `Input.dispatchMouseEvent`, `Page.captureScreenshot`, `Runtime.consoleAPICalled`).

**Web apps / dev servers** — prefer Playwright:
```bash
npx playwright open http://localhost:5173      # headed exploration
# or scripted: chromium.launch() → page.goto() → interact → assert
```
Attach to an already-running Chrome with `connectOverCDP('http://localhost:9222')` when session state matters.

**Anything with an HTTP API** — verify the contract directly with `curl` before touching the UI; many "UI bugs" are API bugs.

## Environment & state hygiene

- **Never test against the user's real profile/data.** Use a throwaway/isolated user-data dir (temp dir, `--user-data-dir=$(mktemp -d)`, or the project's env var for it, e.g. `<APP>_USER_DATA_DIR`). If the project's dev script already creates a throwaway profile, use that.
- Credentials: use the app's own connection/login flow or a dedicated test account; never hardcode secrets into scripts or logs.
- **Keep personal/sensitive details out of prompts, screenshots, logs, and scratch files.**
- Note where the app stores state (config/auth paths) in the project-facts section below, so passes are reproducible.

## The pass itself (procedure)

1. **State the assertion** (one sentence, user-visible).
2. **Launch clean**: fresh isolated profile unless the assertion requires existing state; record the exact launch command.
3. **Drive minimally**: navigate → interact → observe. Prefer `Runtime.evaluate` / `page.evaluate` for reading state over screenshot-guessing; use screenshots to confirm visuals.
4. **Watch the console and network** the whole time — errors/warnings during the pass are findings even if the assertion passes.
5. **Record the verdict**: assertion, steps, result (pass/fail), console anomalies, screenshots if relevant. One short block, not a report.
6. **Clean up**: kill processes, delete temp profiles.
7. If the finding matters long-term → write the automated spec (see scope discipline).

## Failure triage

- Assertion fails → reduce to smallest repro; check whether it fails in an automated spec too (if yes, the spec is the deliverable, not the manual log).
- Can't attach → verify the port is exposed, the app isn't sandboxing the debugger, and no other client holds the CDP connection.
- Flaky behavior → suspect timing; use explicit waits on DOM/network conditions, never `sleep`-and-hope.

## One-time understanding (fill per project)

Before the first pass in a new project, spend a few minutes establishing and recording here (or in a project-local copy of this skill):

- **Dev launch**: what command runs the app, what it builds, which ports it opens, whether it creates a throwaway profile (e.g., `pnpm dev` → builds main+preload, Vite server on `http://localhost:5173`, temp userData dir).
- **State locations**: where auth/config live under the profile dir.
- **Debug access**: which port/env var exposes remote debugging.
- **Test layout**: where unit tests and E2E specs live, and the command to run each.

Keep this section short and factual — it's the map, the sections above are the method.
````

---

## Why It Works

- **Scope discipline up front** stops the agent from wandering: a manual pass is only justified for proving the current change, investigating a bug, or exercising an integration mocks can't reach — everything else belongs in automated tests.
- **One checkable assertion before touching anything** turns "test the app" into a falsifiable claim ("Save persists the note across restart"), which keeps the pass narrow and the verdict honest.
- **Lightest-mechanism-that-reaches-the-runtime** (CDP for Electron, Playwright for web, `curl` for APIs) avoids over-tooling and catches the common case where a "UI bug" is really an API bug.
- **State hygiene rules** (throwaway profile, no real user data, no secrets in logs) make passes safe and reproducible instead of destructive.
- **Read state over screenshot-guessing** — `Runtime.evaluate` / `page.evaluate` gives ground truth; screenshots only confirm visuals.
- **Watch console + network the whole time** treats runtime errors as findings even when the assertion itself passes.
- **Promote-what-matters** closes the loop: anything worth keeping becomes a permanent automated spec so it never regresses silently — the manual pass is a probe, not the product.

---

## Related

- [[long-horizon-task-prompt]] — companion: its "self-verify end to end" step is exactly what this skill operationalizes for a running app.
- [[goal-first-prompt]] — the single user-visible assertion here mirrors the success-criteria contract that prompt forces up front.
- [[architect]] — the "blast radius" question tells you *which* behavior is worth a manual pass; this skill is how you actually prove it.
