# Docs Style Guide

Mandatory formatting rules for every topic file in the `docs/` folder. Read before creating or editing any doc. See [docs-template.md](docs-template.md) for the starting skeleton and [project-overview.md](project-overview.md) for what the docs describe.

## Structure (required order)

```
# Title

`tag` · `tag` · **Level:** Beginner | Intermediate | Advanced

> [!NOTE]
> One-sentence description of what this topic is.

---

## What it is / Why it exists
## Example
## Key points
## Common mistakes
## References

---

> [!TIP]
> **TL;DR** — one sentence summary.
```

- Exactly one `#` (the title) per file — linter requirement.
- `##` for all sections; never skip levels; no `###` or deeper (use bold text or a table instead).
- `---` horizontal rule between every section.

## Tags line

Second line after the title. Backtick inline code for tags, `·` separator, bold level:
`bridge` · `native-modules` · `android` · **Level:** Intermediate

## Alerts (GitHub alert syntax, no emojis)

- `> [!NOTE]` — opening description of the topic.
- `> [!IMPORTANT]` — a constraint the reader must not miss.
- `> [!WARNING]` — something that crashes or breaks silently.
- `> [!TIP]` — TL;DR summary at the end, or a recommendation.

A list inside a WARNING needs a blank line after the alert opener:
```markdown
> [!WARNING]
>
> - item one
> - item two
```

## Tables

- Always aligned column syntax (`:---`, `:---:`, `---:`).
- Add an `Action needed?` column when comparing behaviors/rules.
- Italic caption line above the table: `_Caption text:_`.
- `**Bold**` (asterisks) for critical cell values; `—` for empty/N-A cells.

## Code blocks

- Always specify the language: ```` ```kotlin ````, ```` ```tsx ````, ```` ```text ````.
- Use ```` ```text ```` for diagrams and ASCII flows.
- Inline code uses single backticks.

## Diagrams

- Use Mermaid for all architecture diagrams, flow comparisons, sequence charts — written inline, no image files.
- `flowchart LR` = architecture/data flow; `sequenceDiagram` = step-by-step message passing; `flowchart TD` = decision trees; `timeline` = phases/migration/version history.
- One diagram per concept. Italic caption directly above every diagram. Short node labels (2–4 words); put detail in a table below.
- `LR` for pipelines/data flows, `TD` for trees.
- For screenshots/mockups: PNG in an `assets/` folder next to the `.md`, referenced with `![Alt](assets/file.png)`, max width 1200px. Never raw HTML `<img>`.

## Collapsible sections

Use `<details><summary>Deep dive — subject</summary>` only for deep-dive content that would interrupt the main flow.

## Emphasis

- `**bold**` (asterisks) for important terms and critical values.
- `_italic_` (underscores) for captions and soft emphasis.
- Never mix styles (`__bold__`, `*italic*` are wrong).

## References section

Always last, before the TL;DR tip. One list of links.

## What not to do

- No emojis anywhere.
- No `###` or deeper headings.
- No trailing plain blockquote summaries — use `> [!TIP]`.
- No bare `> blockquote` for warnings — use `> [!WARNING]`.
