# Capture to Notion AI Inbox

## Purpose

iPhone Shortcut for fast mobile captures into the Notion `AI Notes` database.

## Input types

- Clipboard text
- Shared text
- URLs
- Images / screenshots, if supported by the Shortcut branch

## Output

A new Notion page in the `AI Notes` database.

## Default properties

- `Type = Mobile Capture`
- `Status = Captured`
- `Review = Pending`

## Behaviour for text

1. Get clipboard or shared input.
2. Extract title from first meaningful line.
3. Create page in Notion.
4. Place captured text in the page body.

## Behaviour for image

1. Detect image input where possible.
2. Extract text from image using local OCR if available.
3. Store raw image in Google Drive if it is worth preserving.
4. Create a Notion page containing OCR and context.

## Storage rule

Do not save raw images into Notion by default.
