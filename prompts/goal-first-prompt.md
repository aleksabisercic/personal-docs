---
tags:
  - ai-tips
  - prompting
  - workflow
  - agents
  - planning
category: prompts
created: 2026-06-16
language: en
summary: Drop-in prompt that forces an agentic AI to define its own /goal, success criteria, and boundaries (plus a sub-goal per helper agent) and get your approval before doing any work — so you catch misalignment before execution, not after.
---

# Goal-First Prompt

A reusable framing prompt that stops an agent from charging straight into the work. Before touching anything, the AI has to write its own `/goal`, list concrete success criteria, name the boundaries it won't cross, and — if it plans to spawn helper agents — write a separate `/goal` for each one. Then it **waits for your approval**. You correct the plan when it's cheap to correct, not after a long run has gone sideways.

---

## When to Use It

- The task is ambiguous or open-ended and you want to confirm alignment before any execution.
- The work is large enough that a wrong assumption early is expensive to unwind.
- You expect the agent to spawn sub-agents and want each one's mandate pinned down up front.
- You want an explicit, approvable contract (goal + success criteria + boundaries) you can edit.

---

## The Prompt (Paste at Task Start)

```
Before starting, write your own /goal for this task.

Task: [describe the task]
Context: [paste files, docs, requirements, or links]
Constraints: [scope limits, style rules, deadlines, things to avoid]
Definition of done: [what success looks like]

Return:
1. Your main /goal.
2. 3-5 success criteria.
3. Boundaries you should not cross.
4. If you spawn helper agents, write a separate /goal for each one.
5. Ask me to approve or edit the goals before execution.

Do not start until I approve the /goal.
```

---

## Why It Works

- **Goal-before-action** surfaces the agent's interpretation of the task while it's still cheap to fix — misalignment gets caught at the plan, not after the work.
- **The four input slots** (task / context / constraints / definition of done) force you to hand over the information the agent needs instead of letting it guess.
- **3-5 success criteria** convert a vague "do the thing" into testable conditions the agent can later check itself against.
- **Explicit boundaries** make the no-go zones part of the contract rather than something you hope the agent infers.
- **A separate `/goal` per helper agent** keeps each sub-agent's mandate scoped, so parallel work doesn't drift or overlap.
- **Mandatory approval gate** ("do not start until I approve") puts a human checkpoint between planning and execution — you approve, edit, or redirect before any tokens go toward the actual work.

---

## Related

- [[long-horizon-task-prompt]] — companion prompt: once the goal is approved, frame the execution as a long-horizon, self-verifying task.
- [[extract-playbook-from-chat]] — after a run lands a good result, mine the chat into a reusable playbook.
