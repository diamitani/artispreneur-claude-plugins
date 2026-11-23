---
name: create-brand-logo
description: "Brand Logo for independent musicians and artist managers. A logo brief a designer (or Canva) can execute on day one. Use when an artist asks for help with Brand Logo (Studio). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Brand Logo

A logo brief a designer (or Canva) can execute on day one.

Artispreneur skill `create-brand-logo` · Studio · Business Manager · about 15 minutes with the artist.

## What the artist gets

- Brand positioning summary
- Three logo concepts described in detail
- Wordmark type and color recommendations
- Designer / Canva-ready brief

## Ask first

- Artist name and genre
- Visual references you love (and hate)
- Where the logo will live (streaming, merch, stage)

## Steps

1. Define the brand feel in three words
2. Develop three distinct concepts
3. Specify type, color, and lockups
4. Package a production brief

## Guardrails

- Describes concepts — image generation isn't part of this tool yet
- Flags trademark checks before you commit

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a logo brief ready for a designer or Canva.
1. Ask for name, genre, audience, references, and uses (avatar, merch, stage screen).
2. Name the brand feel in three words.
3. Write three distinct proposed concepts: idea, wordmark style, icon (if any), and why it fits. Check every referenced letter exists in the exact artist name; never describe a nonexistent O or other glyph. Mark minimum-size and line-weight rules as starting specs to test, not proof an unrendered logo is legible.
4. Suggest named typefaces subject to checking the exact current license/version, a proposed palette with hex codes only when the artist has not already constrained it; monochrome and supplied color limits take priority over any palette count and horizontal/stacked/avatar lockups. Do not assert free-commercial font licensing or zero-cost tool features without a verified current source. A Markdown concept brief is not an importable logo design or vector asset.
5. Remind them to use the current official trademark search service and get qualified advice before a binding choice. Do not name a retired search system, invent lawyer-price ranges or imply clearance was performed. Handle suggestions must preserve the exact spelling of the artist name and be labeled unchecked, not available.
6. Call create_document (type "doc", skill "create-brand-logo"). State this is a concept brief only; actual logo rendering, readability tests and legal clearance remain undone. Offer manual build instructions, never an unperformed export.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me create my artist logo: three concepts, typography, colors, and a brief I can hand to a designer or build in Canva. Ask me about my sound and references first.
