# Personal Knowledge Wiki

Obsidian vault + LLM-friendly knowledge base. Every note has YAML frontmatter for fast retrieval. Published to web via Quartz (cloned at build time — not checked into this repo).

**Live site**: `aleksabisercic.github.io/personal-docs`

## Structure

```
/
├── finance/           # Tax, investing, brokerage topics
├── learning-notes/    # Mental models, frameworks, study notes
├── _templates/        # Note templates (Obsidian Templater compatible)
├── private/           # Unpublished notes (gitignored from build via ignorePatterns)
├── index.md           # Master Map of Content — link every note here
├── quartz.config.ts   # Quartz site config (title, theme, plugins, baseUrl)
├── quartz.layout.ts   # Quartz page layout (sidebar, graph, TOC, backlinks)
└── .github/workflows/deploy-quartz.yml  # Builds + deploys to GitHub Pages on push to main
```

## Conventions

- **Frontmatter**: Every note needs `tags`, `category`, `created`, `language`, and `summary` in YAML front matter.
- **Wikilinks**: Use `[[note-name]]` for internal cross-references. Link generously.
- **File naming**: Lowercase kebab-case (`ibkr-serbian-tax-guide.md`), no spaces.
- **Atomic notes**: One concept per note. Long reference guides are acceptable.
- **Category**: The `category` frontmatter value must match the parent folder name (e.g. `category: finance` for notes in `finance/`).
- **Language**: English or Serbian. The `language` frontmatter field indicates which.
- **Summaries**: Keep the `summary` field to one information-dense sentence. This is the primary field LLMs use for retrieval.

## When adding a new note

1. Use the template in `_templates/note-template.md`.
2. Fill in all frontmatter fields.
3. Add the note to `index.md` under the appropriate section.
4. Add `[[wikilinks]]` to and from related existing notes.

## When editing existing notes

- Preserve frontmatter. Update `summary` if content changes significantly.
- Add wikilinks to newly related notes.

## Deployment

Pushing to `main` triggers `.github/workflows/deploy-quartz.yml`, which clones Quartz, copies content, and deploys to GitHub Pages. The site config lives in `quartz.config.ts` and `quartz.layout.ts` at the repo root — edit these to change theme, layout, or plugins. Templates and meta-files (CLAUDE.md, README.md) are excluded from the build.
