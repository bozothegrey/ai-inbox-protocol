# AI Output Contract

## Purpose

This note defines the required format for all AI-generated notes saved into the Notion `AI Inbox` system.

## Core rule

Every AI-generated note should have a clear title and structured content.

## Standard Notion properties

Recommended properties for the `AI Inbox` database:

| Property | Type | Purpose |
|---|---|---|
| `Name` | Title | Note title |
| `Author` | Select | `Sergio`, `Stefano`, `Other AI`, `Imported` |
| `Type` | Select | `AI Note`, `Mobile Capture`, `Source Summary`, `Working Note`, `Promotion Candidate` |
| `Status` | Status | workflow stage |
| `Review` | Select | `Pending`, `Reviewed`, `Rejected` |
| `Domain` | Multi-select | `BoGa`, `Fitness`, `Music`, `Sovereign Debt`, `Tech`, `Reading`, `Family` |
| `Source` | URL or Text | Original web/chat/email/source reference |
| `Raw Location` | URL or Text | Google Drive path or link |
| `Target` | Select or Text | `Personal Wiki`, `BoGa`, `Lecture`, `Fitness`, `Archive` |
| `Created` | Created time | Automatic creation timestamp |
| `Last Edited` | Last edited time | Automatic edit timestamp |

## Standard body structure

```markdown
## Summary

Short summary of the note.

## Main Note

Structured content.

## Links / Suggested Links

- Suggested related note or concept

## Source / Raw Location

Google Drive location, URL, or source reference if relevant.

## Review / Next Actions

- [ ] Keep
- [ ] Edit
- [ ] Promote
- [ ] Archive
```

## Storage rule

Raw/source material lives in Google Drive.

Notion contains processed notes, drafts, review queues, working notes, indexes, source summaries, and promotion candidates.

The Personal Wiki contains curated structured notes and cumulative research outputs.
