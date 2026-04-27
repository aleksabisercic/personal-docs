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
- **Trigger**: a new project (idea, brief, or request).
- **Inputs**: just a description of the project. Low-friction on purpose.
- **Steps**: clarify with questions → brainstorm approaches → pick the best → build timeline and tasks → **start executing the AI-owned tasks**.
- **Output**: planned project + work already underway. Credited with **3× project throughput**.
- **Why it matters**: this is the keystone playbook — it spawns the tasks every other playbook in your stack executes (campaign launch, inbox-zero, sales personalization).

→ Full breakdown with phase-by-phase detail, question lists, success criteria, and the client-work adaptation lives in **[[project-planning-playbook]]**.

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
