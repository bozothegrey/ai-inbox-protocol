# Authorship Policy

## Purpose

Track who created or imported each note in the Notion `AI Inbox` database.

## Required property

The Notion `AI Inbox` database must include:

```text
Author
```

Type: `Select`

Options:

- `Sergio` — generated or substantially edited by Sergio
- `Stefano` — written directly by Stefano
- `Zbigniew` — generated or substantially edited by Zbigniew
- `Imported` — imported from another system without substantial editing

## Rule

When Sergio creates a Notion page, set:

```text
Author = Sergio
```

When the source is unclear, use `Imported` or leave blank until reviewed.

## Review use

The `Author` property helps distinguish Sergio-generated notes from user-written notes, imported material, and notes created by other AI tools.
