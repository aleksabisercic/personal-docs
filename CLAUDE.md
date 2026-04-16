# Personal Knowledge Wiki

This is an Obsidian vault and personal knowledge base. It doubles as an LLM-friendly wiki — every note has YAML frontmatter with tags, categories, and a summary line for fast retrieval.

## Structure

```
/
├── finance/           # Tax, investing, brokerage topics
├── learning-notes/    # Mental models, frameworks, study notes
├── _templates/        # Note templates (Obsidian Templater compatible)
└── index.md           # Master Map of Content linking to all topics
```

## Conventions

- **Frontmatter**: Every note has YAML frontmatter with `tags`, `category`, `created`, and `summary`.
- **Wikilinks**: Notes use `[[wikilinks]]` for internal cross-references. When creating or editing notes, link to related topics.
- **Atomic notes**: One concept per note when possible. Long guides (like the IBKR tax guide) are acceptable as reference documents.
- **Language**: Content may be in English or Serbian. The `language` frontmatter field indicates which.
- **File naming**: Lowercase kebab-case (`ibkr-serbian-tax-guide.md`), no spaces.

## When adding a new note

1. Use the template in `_templates/note-template.md` for structure.
2. Fill in all frontmatter fields.
3. Add the note to `index.md` under the appropriate section.
4. Link to related existing notes using `[[wikilinks]]`.

## When editing existing notes

- Preserve frontmatter structure.
- Update the `summary` field if the content changes significantly.
- Add wikilinks to newly related notes.
