# Personal Knowledge Wiki

Obsidian vault + LLM-friendly knowledge base. Every note has YAML frontmatter for fast retrieval.

Web publishing is currently **paused** — the Quartz/GitHub Pages deploy workflow has been removed. The Quartz config files are kept so it can be re-enabled later (see Deployment below).

## Structure

```
/
├── finance/           # Tax, investing, brokerage topics
├── learning-notes/    # Mental models, frameworks, study notes
├── consulting/        # AI consulting playbooks and guides
├── prompts/           # Reusable drop-in prompts for AI tools
├── personal/          # Personal notes
├── _templates/        # Note templates (Obsidian Templater compatible)
├── private/           # Local-only notes (gitignored — never pushed)
├── index.md           # Master Map of Content — link every note here
├── quartz.config.ts   # Quartz site config (title, theme, plugins, baseUrl) — retained, deploy paused
└── quartz.layout.ts   # Quartz page layout (sidebar, graph, TOC, backlinks) — retained, deploy paused
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

**Currently disabled.** The GitHub Pages deploy workflow (`.github/workflows/deploy-quartz.yml`) has been removed, so pushing to `main` no longer builds or publishes anything. The Quartz site config (`quartz.config.ts`, `quartz.layout.ts`) is retained at the repo root. To re-enable publishing, restore a workflow that clones Quartz, copies content (excluding templates and meta-files like CLAUDE.md / README.md), applies these config files, and deploys to GitHub Pages.

## Obsidian

This repo is an Obsidian vault — open the folder in Obsidian (desktop or mobile). `.obsidian/` is gitignored, so per-device settings stay local. Sensitive files go in `private/` (gitignored, never pushed). On iOS, clone via Working Copy and open the folder as a vault; on Android, use Termux + the Obsidian Git plugin.
