# Personal — Audit System

Adapted from Jordan Peterson's *How to Plan Your Life* (90-minute audit), reframed for solo use.

## Structure

```
personal/
├── 01 Daily/       — daily notes, one per day (gitignored)
├── 02 Audits/      — weekly review notes (gitignored)
├── 03 Dragons/     — one note per active recurring friction (gitignored)
├── 04 Experiments/ — one note per running experiment (gitignored)
├── 05 Vision/      — ideal self, ideal week (gitignored)
├── 06 Past/        — memories sorted out, regret-work (gitignored)
└── 99 Templates/   — the template files (committed, syncs across devices)
```

Only `99 Templates/` is committed. Everything else is local-only per `.gitignore`, so honest journaling stays off the web.

## Three loops, nested

- **Daily note** (5 + 5 min): morning intention, evening review. Catches small dragons as they bite.
- **Weekly audit** (45–90 min, same time each week): triage the week, run experiments, sort one piece of the past.
- **Vision** (written once, re-read monthly): ideal self, ideal week, ideal day.

## One-time setup in Obsidian

1. Settings → Core plugins → enable **Daily notes** and **Templates**.
2. **Templates** → template folder: `personal/99 Templates`.
3. **Daily notes** → new file location: `personal/01 Daily`, template: `personal/99 Templates/Template Daily Note`.
4. Calendar: recurring weekly event for the audit. Treat it like a doctor's appointment.

## Four rules

1. **Capture without interpreting.** "Kitchen feels chaotic by Wednesday" is data. "I'm a slob" is a story. Stories belong in the weekly audit, not the daily note.
2. **Experiments are time-boxed.** "Try this for one week, decide on Sunday." Open-ended resolutions don't survive.
3. **Reward yourself for small steps.** If you ignore your own progress, you train yourself to stop trying. Every weekly audit closes with one specific thing you did well.
4. **Watch for rumination.** If the daily note becomes a complaint log, you've drifted. Short and concrete beats long and analytical.

## Optional: fast capture from iPhone

When a dragon bites and you don't want to open Obsidian, add it to an Apple Reminders list called "Dragons" via Siri. On Sunday, paste the list into the weekly audit note and clear it. Or use Drafts with an Obsidian-append action.
