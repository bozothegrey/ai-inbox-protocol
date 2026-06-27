# AI Inbox Protocol

This repository defines the operating protocol for Stefano's AI-to-Notion and AI-to-Obsidian workflow.

It is not the live inbox itself.

## System model

- Google Drive is the raw/source archive.
- Notion is the AI-operable inbox and working layer.
- Personal Wiki is the canonical destination for reviewed permanent notes.
- This GitHub repository is the canonical source for workflow rules, templates, contracts, and agent instructions.

## Main directories

- `contracts/` contains system rules and output contracts.
- `templates/` contains Markdown/Notion templates for notes.
- `workflows/` describes operational flows.
- `shortcuts/` documents iPhone Shortcut behaviour.
- `folder-map/` describes the expected Notion and Obsidian structures.

## Core principle

Raw data stays in Google Drive.

Processed notes, drafts, OCR summaries, maps, and review candidates live in Notion.

Curated permanent notes eventually move to the Personal Wiki / Obsidian.

Rules and templates live here.
