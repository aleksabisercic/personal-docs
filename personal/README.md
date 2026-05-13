# Personal — Audit System

Adapted from Jordan Peterson's *How to Plan Your Life* (90-minute audit), reframed for solo use.

## Structure

```
personal/
├── 01 Daily/       — daily notes, one per day
├── 02 Audits/      — weekly review notes
├── 03 Dragons/     — one note per active recurring friction
├── 04 Experiments/ — one note per running experiment
├── 05 Vision/      — ideal self, ideal week
├── 06 Past/        — memories sorted out, regret-work
└── 99 Templates/   — the template files
```

All entries sync via git so they're available across devices. The whole `personal/` tree is excluded from the published Quartz site (see `ignorePatterns` in `quartz.config.ts` and the `--exclude` rule in `.github/workflows/deploy-quartz.yml`), so it won't appear on the web — but if this repo is public on GitHub, the files are still readable there.

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
