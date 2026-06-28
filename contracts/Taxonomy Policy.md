# Taxonomy Policy

## Purpose

Govern Notion taxonomy fields used by the `AI Inbox`, including select, multi-select, tag, label, domain, target, status, review, and similar categorical properties.

This policy exists to prevent two equal and opposite disasters:

- a taxonomy so rigid that useful notes cannot be classified properly;
- a taxonomy so loose that every tiny variation becomes a new option.

## Scope

This policy applies to Notion properties such as:

- `Type`
- `Status`
- `Review`
- `Domain`
- `Target`
- future tag or label fields

`Author` is governed separately by `/contracts/Authorship Policy.md`.

## Core rule

Agents should treat existing Notion taxonomy values as the preferred vocabulary, not as an exhaustive vocabulary.

When creating or updating a note, agents must first try to use the closest existing category.

Agents may propose a new tag, label, domain, target, type, status, or review value only when the semantic gap is material.

## When to use an existing category

Use the closest existing category when:

- the difference is only a wording preference or synonym;
- the distinction is too granular for retrieval or review;
- the note is a one-off edge case;
- the proposed value would duplicate an existing value;
- the proposed value captures a temporary state better handled in the note body or review section.

Do not propose a new taxonomy value for every small variation in topic, source, framing, or mood. That is not classification. That is decorative entropy.

## When to propose a new category

An agent may propose a new taxonomy value when:

- no existing value describes the note without misleading future retrieval;
- the concept is likely to recur across multiple notes;
- the proposed value would improve summarisation, filtering, or project routing;
- the note belongs to a durable project, domain, or workflow state not represented by the current taxonomy;
- using only the closest existing value would hide an important distinction.

## Human confirmation rule

Agents must not create new Notion taxonomy options automatically unless explicitly authorised by Stefano.

Suggested additions remain provisional until a human confirms, rejects, renames, or merges them.

When the existing taxonomy is close but imperfect, the agent should:

1. use the closest existing value in the actual Notion property;
2. record the proposed addition in the note body under review or next actions;
3. explain briefly why the new value may be useful.

## Proposal format

When proposing a new taxonomy value, use this format in the note body:

```markdown
## Review / Next Actions

### Proposed Taxonomy Additions

- Property: `Domain`
  Proposed value: `AI Economy`
  Closest existing value used now: `Tech`
  Rationale: Captures recurring notes about AI capex, margins, labour effects, market structure, and economic consequences of AI adoption.
  Human decision: Pending
```

## Canonical taxonomy hygiene

When a human approves a new value, update the relevant protocol guidance so future agents can find it from `AGENTS.md`.

Prefer durable categories over fashionable micro-tags.

Prefer one good category used consistently over five clever categories nobody will remember in three weeks.
