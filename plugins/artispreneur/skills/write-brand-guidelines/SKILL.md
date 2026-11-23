---
name: write-brand-guidelines
description: "Brand Guidelines for independent musicians and artist managers. Your brand bible: voice, visuals, and rules everyone follows. Use when an artist asks for help with Brand Guidelines (Studio). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Brand Guidelines

Your brand bible: voice, visuals, and rules everyone follows.

Artispreneur skill `write-brand-guidelines` · Studio · Business Manager · about 20 minutes with the artist.

## What the artist gets

- Brand story and positioning
- Voice & tone rules with examples
- Palette, type, and logo usage
- Social, merch, and press rules

## Ask first

- Existing logo, colors, and fonts (if any)
- Three words you want fans to feel
- Examples of posts or visuals you're proud of

## Steps

1. Capture your identity
2. Codify voice with do/don't examples
3. Lock visual rules
4. Deliver a shareable brand guide

## Guardrails

- Builds on what you already have — no forced rebrand

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a brand guide collaborators can follow without asking.
1. Ask for current logo/colors/fonts, audience, three feeling words, and good/bad examples.
2. Write a brand story only from confirmed artist-supplied facts. Never pad to a word count or infer instruments, recording methods, career stage, origin or musical arrangements from genre/name/visual style. If no actual story is supplied, leave a clearly labeled artist-statement prompt instead. Label positioning and voice rules as proposals; example sentences must not invent releases, dates, equipment, metrics or credits.
3. Visual rules: preserve the exact supplied spelling, case and color limits. Additional colors, usage ratios, type hierarchy and clear-space values are proposals only, not approved brand facts. Rendered readability remains unverified until actual assets are tested.
4. Channel rules: social, merch, press photos, collaborator checklist.
5. Call create_document (type "doc", skill "write-brand-guidelines") with a compact complete text-only draft. Preserve supplied brand rules; mark missing facts unknown and optional choices proposed. Do not promise slide, Canva or vector exports that were not actually created. Do not assert tool features, font licensing or legal clearance without current source evidence.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Write my artist brand guidelines: voice, palette, type, logo usage, and social rules. Ask me about my current visuals and vibe first.
