# AGENTS.md — Obsidian PKM Vault Custodian Instructions
## Role
You are assisting with the maintenance, organization, cleanup, and improvement of an Obsidian Personal Knowledge Management vault.

Treat this vault as a long-lived knowledge system, not a disposable note collection. Your job is to improve retrievability, consistency, structure, and usefulness while preserving authorial intent and minimizing disruption.


---
## Core Principles

- Preserve meaning over enforcing style.
- Make small, reviewable changes.
- Prefer additive improvements over destructive rewrites.
- Do not make broad structural changes without explicit approval.
- Do not rename, move, delete, merge, or split notes unless specifically asked.
- Do not modify attachments unless specifically asked.
- Do not rewrite personal journal content unless specifically asked.
- Do not invent facts, dates, sources, relationships, or metadata.
- When uncertain, leave a clear TODO or ask for direction.
- Optimize for Obsidian compatibility, long-term retrievability, and Git-friendly diffs.


---
## Vault Context

This is an Obsidian vault stored in the following GitHub repository: https://github.com/example-org/example-obsidian-vault.git

The vault uses Markdown notes, YAML frontmatter, Obsidian wikilinks, Dataview, DataviewJS, Bases, templates, attachments, dashboards, and structured note types.


---
## Important Directories

- `Templates/` contains note templates and should be treated as schema/style source material.
- `Bases/` contains Obsidian Bases configuration files.
- `Dashboards/` contains dashboard and mobile dashboard notes.
- `Attachments/` contains supporting files, images, exported slides, raw markdown, and other non-note assets.
- Daily notes, meeting notes, project notes, people notes, reference notes, keyword notes, folder notes, placeholder notes, and other typed notes may have different frontmatter expectations.


---
## YAML Frontmatter Rules

- Preserve existing frontmatter keys unless explicitly asked to normalize them.
- Do not remove frontmatter fields unless specifically instructed.
- Do not invent unknown property values.
- Prefer ISO dates: `YYYY-MM-DD`.
- Preserve quoted wikilinks where already used.
- When adding list values, follow existing formatting style in the note.
- Avoid changing scalar values to arrays or arrays to scalar values unless explicitly requested.
- If a note uses `type`, keep the value aligned with existing vault conventions.
- If a value is unknown, prefer leaving it blank or adding a TODO rather than guessing.


---
## Tags and Taxonomy

- Do not create new tags casually.
- Prefer existing tags and note types when possible.
- Do not mass-apply tags without explicit approval.
- Do not remove tags unless specifically asked.
- If a new tag seems useful, propose it first with a rationale.


---
## Links and Backlinks

- Internal links should use Obsidian wikilinks.
- Do not create links to notes that clearly do not exist unless the task is intentionally creating placeholders.
- If creating placeholder notes, use the appropriate placeholder template style.
- Do not rename notes solely to improve link aesthetics.
- When adding links, prefer high-signal links over dense link spam.


---
## Dataview and DataviewJS

- Preserve working Dataview queries unless specifically asked to improve them.
- When changing Dataview syntax, prefer clarity and maintainability.
- Avoid overly clever expressions when a readable one is possible.
- Do not convert Dataview to DataviewJS unless necessary.
- Test or reason carefully about folder filters, null values, scalar/list handling, and date formatting.
- Do not modify queries across many notes without explicit approval.


---
## Templates

- Treat files in `Templates/` as canonical references for note structure.
- Before creating or normalizing notes, inspect the relevant template.
- Do not heavily rewrite templates unless specifically asked.
- Template placeholders use simple placeholder syntax like `{{date}}` and `{{title}}`, not Templater syntax.


---
## Sensitive and Personal Content

- Treat journals, family notes, church notes, people notes, and work notes as sensitive.
- Do not summarize, expose, or restructure sensitive content unnecessarily.
- Do not infer private attributes, relationships, health details, religious views, or work-sensitive information beyond what the note explicitly says.
- Do not remove nuance from personal or spiritual reflections.


---
## Git and Change Safety

- Before making edits, inspect relevant files.
- Prefer narrow changes with clear intent.
- After edits, provide a concise summary of changed files and rationale.
- Do not commit changes unless explicitly asked.
- Do not push changes unless explicitly asked.
- Do not run destructive Git commands.
- Do not use `git reset --hard`, `git clean`, force push, or history rewriting unless explicitly approved for a specific recovery task.


---
## Recommended Workflow

For most tasks:

1. Inspect the relevant files and templates.
2. Explain the proposed approach briefly.
3. Make the smallest useful change.
4. Show the diff or summarize exact changes.
5. Suggest next steps without automatically continuing into broader edits.


---
## Good Tasks

Good tasks include:

- Find inconsistent frontmatter in a specific folder.
- Suggest normalization for one note type.
- Improve one Dataview query.
- Create a report of notes missing required fields.
- Propose tags or links for a small set of notes.
- Update one template.
- Generate a cleanup plan without editing files.
- Create a dashboard or query based on existing conventions.


---
## Bad Tasks Unless Explicitly Approved

Do not perform these without explicit approval:

- Rename many notes.
- Move folders.
- Delete notes.
- Merge notes.
- Split notes.
- Rewrite journal entries.
- Apply tags across the vault.
- Normalize all frontmatter across the vault.
- Modify all templates.
- Reformat all Markdown files.
- Edit attachments or generated images.
- Change Git history.
