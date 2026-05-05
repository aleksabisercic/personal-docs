---
tags:
  - ai-consulting
  - discovery
  - client-work
  - operations
  - playbooks
  - rachel-woods
category: consulting
created: 2026-04-27
language: en
summary: Rachel Woods' playbooking method — define repeatable client/business work as a four-part playbook (trigger, inputs, steps, outputs) so AI can run it; reframe prompting as writing an employee handbook for an AI hire.
---

# The Playbooking Method (Rachel Woods)

A reusable framework for defining a problem with a client (or yourself) so AI can actually run the work. The core shift: **stop asking "how do I prompt AI?" and start asking "how would I teach a human to do this?"** Write the employee handbook, then hand it to the AI. The result is a playbook that runs in any tool — Claude Skills, ChatGPT custom GPTs/Agents, Microsoft Copilot, Gemini Gems, or one-step-per-Zapier-action — so you **own the playbook, rent the tech**.

---

## The Four-Component Playbook

Every playbook is just these four things. When defining work with a client, this is the discovery scaffold.

| Component | What it is | Example (newsletter playbook) |
|-----------|------------|-------------------------------|
| **Trigger** | What kicks it off — schedule or event | Monday 9:00 AM |
| **Inputs** | What varies each run (the human-shaped raw material) | Brain dump of topics top of mind |
| **Steps** | The actual process the AI follows | Pick topic → outline → draft → edit for voice → write subject line |
| **Outputs** | The end result | Drafted newsletter |

The newsletter playbook collapsed 2–3 hours/week of writing into ~30 minutes — ~130 hours/year saved on a single playbook.

---

## The Mental Model Shift

When AI feels like a fight (you correct it, it adds emojis, you correct again, you give up and write it yourself), the missing piece is the playbook. AI without a playbook is a contractor with no brief.

To set up a human assistant well you'd give them: **company context → what to do → how to do it → an employee handbook to follow.** A playbook is that handbook — written for AI instead of for a person. Once it's in writing, you can trust the output the same way you'd trust the assistant who follows the handbook to the letter.

---

## Writing the Steps (The Specificity Layer)

A playbook is only as good as how each step is written. For each step:

1. **Be clear and non-contradictory** — the most common failure mode is instructions that quietly conflict.
2. **Inject background context** — what does the AI need to know about the company, audience, or constraint to do this step well?
3. **Show, don't tell** — give examples for anything easier to demonstrate than describe (voice, formatting, tone).
4. **Define success criteria** — a checklist of what a good output looks like. The AI optimizes against it.

---

## Where to Find Playbook Candidates

Four hunting grounds — useful both for your own work and for client discovery sessions:

1. **Existing SOPs** — any documented process is already 80% of a playbook.
2. **Recurring calendar meetings** — look at the last 1–2 months. For each recurring meeting ask: what's the prep, what's the follow-up, and **could this meeting just be a playbook?**
3. **Recurring to-do items** — anything that takes **>4–6 hours/month** is over the threshold; playbooking it unlocks meaningful time.
4. **The wish list** — things you'd do if time were unlimited. Some of the highest-leverage playbooks live here.

---

## Running a Playbook

1. Save the playbook in the AI tool of choice (Claude Skill, custom GPT, Copilot agent, Gemini Gem, Zapier flow).
2. Invoke with the trigger phrase: *"Run my newsletter playbook."*
3. The AI loads the saved instructions, asks for the inputs it knows it needs, and walks the steps in order.
4. You stop prompting per-task and start operating with AI.

---

## Using This With Clients (Discovery)

When defining a problem with a client, drive the conversation toward filling out the four boxes:

- **Trigger**: When does this problem fire? (calendar event, inbound message, end of a campaign, end of a call)
- **Inputs**: What do you have in hand each time it fires? What's variable vs. constant?
- **Steps**: Walk me through how you (or your best person) does it today. *Then* sharpen each step with context, examples, and success criteria.
- **Outputs**: What does "done" look like, and who consumes it next?

If a client cannot describe one of the four, that gap **is** the consulting work. Operational debt — the difference between how things should run and how they actually run — almost always shows up as a missing or fuzzy component.

---

## Operational Debt (The Frame)

The gap between *how you know things should run* and *how they actually run*. Symptoms:

- Work on your plate that's below your pay grade.
- Busy all day, not productive.
- Re-explaining the same thing to the same person more than once.
- Trying to delegate, going back-and-forth, giving up and doing it yourself.

Playbooking is the fastest way out — every playbook closes a slice of the gap.

---

## Related

- [[business-streamlining-playbooks]] — concrete playbook candidates for an AI consulting practice, modeled on Rachel's stack.
- [[extract-playbook-from-chat]] — drop-in prompt for mining an existing AI chat for the *steps* component.
- [[architect]] — the simplicity / cost-of-change / blast-radius lens applies when deciding which playbooks to build first.
