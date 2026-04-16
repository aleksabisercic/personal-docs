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

| Path | Purpose |
|------|---------|
| `finance/` | Tax, investing, brokerage |
| `learning-notes/` | Mental models, frameworks, study notes |
| `private/` | Unpublished notes (excluded from site build) |
| `_templates/` | Note templates (Obsidian Templater compatible) |
| `index.md` | Master Map of Content |
| `quartz.config.ts` | Site config: title, theme, plugins, base URL |
| `quartz.layout.ts` | Page layout: sidebar, graph, TOC, backlinks |
| `CLAUDE.md` | LLM context and conventions |

## Deployment

Push to `main` → GitHub Actions clones [Quartz](https://github.com/jackyzha0/quartz), copies content + config, builds static HTML, and deploys to GitHub Pages. Quartz is not checked into this repo.

To change site theme, plugins, or layout, edit `quartz.config.ts` and `quartz.layout.ts` here — they're overlaid onto Quartz at build time.
