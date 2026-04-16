# personal-docs

**Live site:** https://aleksabisercic.github.io/personal-docs

A personal knowledge wiki stored as plain markdown. Designed to work as:

1. **An Obsidian vault** — open this repo in Obsidian for graph view, wikilinks, search, and Dataview queries.
2. **An LLM-friendly knowledge base** — every note has YAML frontmatter (tags, summary, category) so LLMs can quickly understand and retrieve content. See `CLAUDE.md` for conventions.

## Quick start

```
git clone <this-repo>
# Open the repo folder as an Obsidian vault
# Recommended plugins: Templater, Dataview
```

## Structure

| Folder | Purpose |
|--------|---------|
| `finance/` | Tax, investing, brokerage |
| `learning-notes/` | Mental models, frameworks, study notes |
| `_templates/` | Note templates (Obsidian Templater compatible) |
| `index.md` | Master Map of Content |
| `CLAUDE.md` | LLM context and conventions |
