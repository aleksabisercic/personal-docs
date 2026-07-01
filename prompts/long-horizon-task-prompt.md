---
tags:
  - ai-tips
  - prompting
  - workflow
  - claude-code
  - agents
category: prompts
created: 2026-06-09
language: en
summary: Drop-in prompt that tells an agentic AI to treat work as a long-horizon task — keep going until done, split large work into sub-agents, self-verify end to end (web/mobile/backend), and report what changed, how it was verified, and what risks remain.
---

# Long-Horizon Task Prompt

A reusable framing prompt for agentic coding tools (Claude Code, etc.). It sets the AI up to *finish* the job instead of stopping at the first plausible result: keep working until the outcome is complete, parallelize big work across sub-agents, and — most importantly — **self-verify before claiming done**.

---

## When to Use It

- The task is large enough to span many steps or a long session.
- You won't be watching every step and want the agent to push to completion on its own.
- You care about *verified* completion, not just "I made the edits."
- The work has a testable surface (a web UI, a mobile app, or a backend service).

---

## The Prompt (Paste at Task Start)

```
Run this as a long-horizon task.

Use auto-approved permissions only for safe project actions.
Use /goal or /loop to keep working until the outcome is complete.
If the task is too large, create a dynamic workflow and split it into sub-agents.
Do not report "done" until you self-verify end to end:
- Web: test in the browser.
- Mobile: test in an iOS or Android simulator MCP.
- Backend: start the full service and run the relevant checks.

At the end, give me:
1. What changed
2. How you verified it
3. What risks remain
```

---

## Why It Works

- **"Long-horizon task" framing** sets the expectation that the job spans many steps, so the agent plans for completion instead of stopping at the first plausible stopping point.
- **Safe-actions-only permissions** keeps the autonomy bounded — the agent moves fast on reversible project work but still surfaces anything risky.
- **`/goal` or `/loop`** keeps the agent driving toward the outcome rather than ending its turn early.
- **Sub-agents for large work** prevents one context from getting overloaded and lets independent pieces run in parallel.
- **Mandatory end-to-end self-verification** is the core move: "done" must mean *observed working* (browser, simulator, or a running service), not just "edits applied."
- **The three-part closeout** (changed / verified / risks) forces an honest report you can act on — especially the residual risks the agent might otherwise gloss over.

---

## Related

- [[goal-first-prompt]] — companion prompt: define and approve the `/goal` before kicking off the long-horizon run.
- [[extract-playbook-from-chat]] — companion prompt: once a long-horizon run lands a good result, mine the chat into a reusable playbook.
- [[manual-e2e-skill]] — the hands-on skill that operationalizes this prompt's "self-verify end to end" step against a real running app.
- [[architect]] — the "blast radius" question pairs well with the *what risks remain* closeout.
