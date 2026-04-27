---
tags:
  - ai-consulting
  - operations
  - playbooks
  - business-development
  - rachel-woods
category: consulting
created: 2026-04-27
language: en
summary: Catalog of playbook candidates for streamlining an AI consulting business — inbox zero, campaign launch & analysis, sales-lead personalization, post-call client coaching, and the project-planning playbook — modeled on Rachel Woods' stack where a 10-person agency runs sales outreach, inbox, and marketing reporting with zero humans.
---

# Business-Streamlining Playbooks

Rachel Woods runs a 10-person AI operations agency where **zero humans** do sales outreach and follow-up, manage the inbox, report on marketing campaigns, or build marketing funnels — the work still gets done, on time, every week, because every recurring process is a playbook (see [[playbooking-method]]). This note is a working list of playbooks worth building for a solo or small AI consulting practice, plus prompts for what to define before writing each one.

---

## Why this matters

Sales, marketing, ops, and reporting are where most consulting practices lose hours that should be billable or invested in delivery. Each item below is a candidate to remove from the human todo list. The pattern is always the same — define the four components ([[playbooking-method]]: trigger, inputs, steps, outputs) and pick a host (Claude Skill, custom GPT, Copilot agent, Gemini Gem, Zapier).

---

## Rachel's Stack (Use as Templates)

### 1. Inbox-zero playbook
- **Trigger**: every morning at 8:00 AM.
- **Inputs**: incoming emails since the last run.
- **Steps**: categorize by urgency → decide response posture → draft replies → check calendar and propose/send meeting times.
- **Output**: inbox triaged; drafts ready to skim and send.

### 2. Campaign launch playbook
- **Trigger**: a new offer is greenlit.
- **Inputs**: the offer description, audience, dates.
- **Steps**: draft landing page → draft email sequence → draft lead magnet outline.
- **Output**: launch-ready assets in one pass.

### 3. Post-campaign performance analysis
- **Trigger**: campaign end-date.
- **Inputs**: campaign metrics dump.
- **Steps**: run analysis against historical baseline → extract key takeaways → recommend next actions.
- **Output**: campaign post-mortem with a "do next" list.

### 4. Sales-lead personalization
- **Trigger**: new qualified lead.
- **Inputs**: lead profile, source, expressed interest.
- **Steps**: research lead → match to relevant offer → draft personalized outreach.
- **Output**: personalized first-touch ready for review.

### 5. Post-call client coaching
- **Trigger**: end of any client call.
- **Inputs**: call transcript + the coaching rubric ("how we want to show up for clients").
- **Steps**: score the call against the rubric → flag misses → suggest concrete improvements for next call.
- **Output**: a self-coaching note before the next session.

### 6. Project-planning playbook *(Rachel's favorite — the one she contributed as a bonus)*

The playbook she says **turned her into a "project machine"** and lets her team ship **3× more projects**. Its differentiator vs. a normal project-planning prompt: it doesn't stop at the plan — it **starts doing the work** at the end.

#### What Rachel explicitly says (transcript, 1:33:29–1:33:54)

> "We have a playbook that we use to do three times more projects as a team because we have a playbook that helps us not only plan the projects, but also get started on them. How it works is the playbook takes in just a description of the project and what we do is the AI then asks us questions to clarify the project. It helps brainstorm approaches, decide what the best approach is, then turn that into a timeline and tasks. And the best part is after the AI has helped us plan the project, we have the AI go, 'Oh, I can do those tasks. Let me start on them.'"

#### The four components (directly from the transcript)

- **Trigger**: a new project (you have an idea, a brief, or a request).
- **Inputs**: **just a description of the project** — that's the entire bar to invoke. Low-friction on purpose.
- **Steps** (her exact order, five phases):
  1. **Clarify** — AI asks the human questions to fill gaps in the project description.
  2. **Brainstorm approaches** — surface multiple ways to tackle the project.
  3. **Decide the best approach** — pick one.
  4. **Build a timeline and tasks** — convert the chosen approach into a sequenced plan.
  5. **Start executing** — AI looks at the task list, picks the ones it can do, and begins. *("Oh, I can do those tasks. Let me start on them.")*
- **Output**: a planned project **with work already underway** — not a doc that sits in Notion waiting for someone to act on it.

#### Step-by-step detail

Rachel does not publish her exact prompts on stage, so the **structure below is hers**, the **specific question-list and success criteria are reasonable inferences** — built using her own four guidance rules for writing good steps (clear instructions, background context, examples, success criteria — see [[playbooking-method]]). Use this as a v1 to copy and refine.

**Phase 1 — Clarify the project**

The AI interviews the human until it has enough signal to plan. Likely question set:

- What's the **definition of done** / desired outcome?
- Who's the **audience or stakeholder** (client? team? self?)?
- Is there a **hard deadline**, a soft one, or none?
- What are the **constraints** — budget, team, dependencies, tools?
- What's been **tried or ruled out** already?
- What does **success** look like — measurable if possible?
- What level of quality bar — quick draft, polished, production?

Success criterion for this phase: AI must not move on until the answers cover *outcome, audience, deadline, constraints, success metric*.

**Phase 2 — Brainstorm approaches**

Surface **2–4 distinct approaches**, not variations of one. Useful axes to force diversity:

- Fast/cheap vs. thorough/expensive
- Build vs. buy vs. delegate
- Sequential vs. parallel
- Minimal-viable vs. complete

Each approach gets: short description, est. effort, est. timeline, key risk.

**Phase 3 — Pick the best approach**

Score against the constraints and success metric from Phase 1. Either:
- AI picks and explains why, then asks human to confirm, or
- AI ranks and lets human choose.

The output of this phase is a single chosen approach + a one-line "why this one."

**Phase 4 — Build timeline and tasks**

Convert the approach into:
- An ordered **task list** with dependencies.
- Each task tagged with an **owner**: `AI`, `human`, or `human + AI`.
- Each task with a rough **time estimate**.
- A timeline that respects deadline + dependencies.

Success criterion: every task is small enough to be a discrete unit of work — anything fuzzy must be broken down further.

**Phase 5 — Start executing**

The AI:
1. Filters the task list to tasks where owner = `AI`.
2. Runs the first one (often by handing off to another playbook — e.g., "draft the landing page" hands to the campaign-launch playbook).
3. Returns: tasks completed, tasks blocked (waiting on human), tasks remaining.

Human is left with **only the tasks that genuinely require them**.

#### Why this is the keystone playbook

Rachel notes (1:34:14) that her playbooks **stack into a personal operating system** — playbooks calling playbooks. The project-planning playbook is the one that **spawns work for every other playbook in the stack**:

- "Draft the landing page" → hands off to the **campaign-launch playbook**.
- "Personalize outreach to these 5 leads" → hands off to the **sales-lead personalization playbook**.
- "Send the project kickoff email" → hands off to the **inbox-zero playbook**.

If you build only one playbook this quarter, this is the one — it makes every other playbook more valuable.

#### Adapting it for client work

Same skeleton, swap the framing:

- **Trigger**: signed SOW or kickoff call complete.
- **Inputs**: SOW + discovery brief instead of "project description."
- **Phase 1 clarifying questions** add: client's success metric, who internally signs off, cadence of check-ins, what the client has already tried.
- **Phase 5 execution**: AI-owned tasks output drafts the consultant reviews before sending — a non-zero blast radius means a human-in-the-loop gate before anything reaches the client.

---

These can be **stacked into a personal operating system** — playbooks calling playbooks (morning routine → strategy → projects → ideas → tasks → life admin). That's the end state to work toward, not the starting point.

---

## Candidate Playbooks for an AI Consulting Practice

Inspired by Rachel's set, biased toward client-facing work:

- **Discovery-call playbook** — trigger: scheduled discovery call. Inputs: prospect's company, role, expressed problem. Steps: pre-call research → tailored question list (driving toward the four playbook components) → post-call summary → proposal-shaped notes. Output: a discovery brief + a draft proposal angle.
- **Proposal playbook** — trigger: discovery brief approved. Inputs: discovery brief, pricing tiers. Steps: scope → deliverables → timeline → SOW → cover note. Output: send-ready proposal.
- **Client-onboarding playbook** — trigger: signed SOW. Inputs: client details, project type. Steps: kickoff agenda → access/credentials checklist → intro email → calendar holds. Output: client onboarded in <24h.
- **Weekly client status report** — trigger: every Friday. Inputs: this week's commits, calls, decisions. Steps: summarize progress → flag risks → list next-week commitments. Output: same-format report each client expects.
- **Playbook-discovery playbook** (meta) — trigger: new client engagement. Inputs: client's calendar, SOP folder, todo list, wish list. Steps: scan each of Rachel's four hunting grounds → score candidates by hours/month and reversibility → return a prioritized backlog. Output: the engagement's roadmap.
- **Content-from-client-work playbook** — trigger: end of a notable engagement. Inputs: anonymized case notes. Steps: extract the lesson → draft post / newsletter / case study. Output: marketing artifact built from delivery work (turns delivery into top-of-funnel without dedicated marketing time).
- **Lead-qualification playbook** — trigger: inbound lead form. Inputs: form data + LinkedIn/website. Steps: score fit → route (book call / nurture / decline) → draft response. Output: every lead handled in minutes, consistently.

---

## How to choose what to build first

Apply the [[architect]] lens before writing any of these:

1. **Simplicity** — what's the smallest version of this playbook that could work end-to-end? Build that, not the full thing.
2. **Cost of change** — playbooks are cheap to revise; bias toward shipping the v1 and editing in production.
3. **Blast radius** — start with playbooks where a bad output is recoverable (drafts you review) before automating anything that sends to a client unattended.

Threshold rule from Rachel: anything recurring that costs **>4–6 hours/month** is worth playbooking now.

---

## Related

- [[playbooking-method]] — the four-component framework these all sit on top of.
- [[architect]] — prioritization lens for which playbooks to build first.
