# AI to Notion Workflow

## Purpose

Save structured AI-generated notes into the Notion `AI Inbox` system.

## Flow

ChatGPT / Other AI  
↓  
Create or update Notion page in `AI Notes` database  
↓  
Set properties such as Type, Status, Review, Domain, Source, Raw Location, Target  
↓  
Review in Notion  
↓  
[Optional] Promote cleaned notes to Personal Wiki

## Required AI output

The AI-generated page should contain:

- Summary
- Main Note
- Links / Suggested Links
- Source / Raw Location
- Review / Next Actions

## Status lifecycle

```text
Captured → Draft → Processing → Ready → Promoted / Archived
```

## Notion database

Recommended database name:

```text
AI Notes
```
