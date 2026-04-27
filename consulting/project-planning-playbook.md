---
tags:
  - ai-consulting
  - playbooks
  - project-management
  - operations
  - rachel-woods
category: consulting
created: 2026-04-27
language: en
summary: Full breakdown of Rachel Woods' project-planning playbook — the keystone playbook that takes a project description, asks clarifying questions, brainstorms approaches, picks one, builds a timeline and tasks, then executes the AI-owned tasks; credited with 3× project throughput.
---

# Project-Planning Playbook

Rachel Woods' favorite playbook — the one she contributed as a bonus to Dean Graziosi's boot camp and credits with **3× more projects shipped** as a team. Its differentiator vs. a normal project-planning prompt: it doesn't stop at the plan — it **starts doing the work** at the end. This is the keystone that makes every other playbook in your stack more valuable, because it spawns the tasks the others execute.

For the framework this sits inside, see [[playbooking-method]]. For where it fits in the broader business stack, see [[business-streamlining-playbooks]].

---

## What Rachel explicitly says (transcript, 1:33:29–1:33:54)

> "We have a playbook that we use to do three times more projects as a team because we have a playbook that helps us not only plan the projects, but also get started on them. How it works is the playbook takes in just a description of the project and what we do is the AI then asks us questions to clarify the project. It helps brainstorm approaches, decide what the best approach is, then turn that into a timeline and tasks. And the best part is after the AI has helped us plan the project, we have the AI go, 'Oh, I can do those tasks. Let me start on them.'"

---

## The Four Components (directly from the transcript)

- **Trigger**: a new project (an idea, a brief, or a request).
- **Inputs**: **just a description of the project**. That's the entire bar to invoke. Low-friction on purpose.
- **Steps** (her exact order, five phases):
  1. **Clarify** — AI asks questions to fill gaps in the project description.
  2. **Brainstorm approaches** — surface multiple ways to tackle the project.
  3. **Decide the best approach** — pick one.
  4. **Build a timeline and tasks** — convert the chosen approach into a sequenced plan.
  5. **Start executing** — AI looks at the task list, picks the ones it can do, and begins. *("Oh, I can do those tasks. Let me start on them.")*
- **Output**: a planned project **with work already underway** — not a doc that sits in Notion waiting for someone to act on it.

> The structure above is hers. The phase-level detail below is **a reasonable v1 built using her own four guidance rules** for writing playbook steps — clear instructions, background context, examples, success criteria (see [[playbooking-method]]). Use it as a starting point and refine against your own projects.

---

## Phase 1 — Clarify the Project

The AI interviews the human until it has enough signal to plan. Likely question set:

- What's the **definition of done** / desired outcome?
- Who's the **audience or stakeholder** (client? team? self?)?
- Is there a **hard deadline**, a soft one, or none?
- What are the **constraints** — budget, team, dependencies, tools?
- What's been **tried or ruled out** already?
- What does **success** look like — measurable if possible?
- What level of quality bar — quick draft, polished, production?

**Success criterion**: AI must not move on until the answers cover *outcome, audience, deadline, constraints, success metric*.

---

## Phase 2 — Brainstorm Approaches

Surface **2–4 distinct approaches**, not variations of one. Useful axes to force diversity:

- Fast/cheap vs. thorough/expensive
- Build vs. buy vs. delegate
- Sequential vs. parallel
- Minimal-viable vs. complete

Each approach gets: short description, est. effort, est. timeline, key risk.

---

## Phase 3 — Pick the Best Approach

Score against the constraints and success metric from Phase 1. Either:

- AI picks and explains why, then asks human to confirm, or
- AI ranks and lets human choose.

The output of this phase is **a single chosen approach + a one-line "why this one."**

---

## Phase 4 — Build Timeline and Tasks

Convert the approach into:

- An ordered **task list** with dependencies.
- Each task tagged with an **owner**: `AI`, `human`, or `human + AI`.
- Each task with a rough **time estimate**.
- A timeline that respects deadline + dependencies.

**Success criterion**: every task is small enough to be a discrete unit of work — anything fuzzy must be broken down further.

---

## Phase 5 — Start Executing

The AI:

1. Filters the task list to tasks where owner = `AI`.
2. Runs the first one (often by handing off to another playbook — e.g., "draft the landing page" hands to the campaign-launch playbook).
3. Returns: tasks completed, tasks blocked (waiting on human), tasks remaining.

Human is left with **only the tasks that genuinely require them**.

---

## Why This Is the Keystone Playbook

Rachel notes (1:34:14) that her playbooks **stack into a personal operating system** — playbooks calling playbooks. The project-planning playbook is the one that **spawns work for every other playbook in the stack**:

- "Draft the landing page" → hands off to the **campaign-launch playbook**.
- "Personalize outreach to these 5 leads" → hands off to the **sales-lead personalization playbook**.
- "Send the project kickoff email" → hands off to the **inbox-zero playbook**.

If you build only one playbook this quarter, this is the one — it makes every other playbook more valuable.

---

## Adapting It For Client Work

Same skeleton, swap the framing:

- **Trigger**: signed SOW or kickoff call complete.
- **Inputs**: SOW + discovery brief instead of a "project description."
- **Phase 1 clarifying questions** add: client's success metric, who internally signs off, cadence of check-ins, what the client has already tried.
- **Phase 5 execution**: AI-owned tasks output drafts the consultant reviews before sending — a non-zero blast radius means a **human-in-the-loop gate** before anything reaches the client.

---

## Related

- [[playbooking-method]] — the four-component framework this is built on.
- [[business-streamlining-playbooks]] — where this sits in the broader stack of business playbooks.
- [[architect]] — simplicity / cost-of-change / blast-radius lens for deciding which AI-owned tasks to gate behind human review.
