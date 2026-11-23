---
name: artist-profile
description: "Artist Profile for independent musicians and artist managers. Build one complete artist record (identity, genre, stage, city, links) with a career-stage assessment and a list of gaps. Use when an artist asks for help with Artist Profile (Career). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Artist Profile

Build one complete artist record (identity, genre, stage, city, links) with a career-stage assessment and a list of gaps.

Artispreneur skill `artist-profile` · Career · Manager · about 10 minutes with the artist.

## What the artist gets

- Complete artist profile (identity, genre, stage, city, links)
- Career-stage assessment with reasons
- List of missing facts to add later

## Ask first

- Stage name (and legal name if different)
- Genres, city, and how long you've been releasing
- Your streaming and social links

## Steps

1. Check what's already on file
2. Ask only for what's missing
3. Classify your career stage
4. Save the profile

## Guardrails

- Never invent facts, numbers, contacts, or credits — ask, or leave it out.
- Date of birth and phone stay private unless you say otherwise

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: an accurate profile draft, not a complete invented record.
1. Use supplied facts only. A separate fictional/client case must not inherit account profile, earlier unrelated conversations, catalog or memory. For an actual account profile request, review existing owned sources without overwriting unknowns or resolving conflicts by guessing.
2. Missing release/show/audience/income data means unknown, never zero, no public releases or pre-release/new status. Do not assign Instrumentalist/Producer/Composer roles from instrumental project alone. Stage assessment remains unknown unless supplied evidence supports it.
3. Preserve the requested private goal and weekly capacity; a private demo is not an upcoming public release. Relative dates use the artist's local request date, not server UTC. Do not add genre, branding, achievements, collaborators or links.
4. Missing facts to ask later are optional enrichment, not legal-identity or platform prerequisites. No account profile, memory or roadmap change for a draft-only request, and no permission grant can be inferred from a profile field.
5. Call create_document (type "doc", skill "artist-profile") titled "Artist profile — <name>" with confirmed facts, unknowns and any explicitly requested assessment. Do not claim a mutation or no mutations solely from generated prose.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Set up my artist profile so every agent knows who I am. Ask only for what you don't already have.
