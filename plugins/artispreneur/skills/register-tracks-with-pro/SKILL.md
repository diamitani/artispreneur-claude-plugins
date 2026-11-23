---
name: register-tracks-with-pro
description: "Track Registration for independent musicians and artist managers. Register every song so royalties can actually find you. Use when an artist asks for help with Track Registration (Publishing & PRO). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Track Registration

Register every song so royalties can actually find you.

Artispreneur skill `register-tracks-with-pro` · Publishing & PRO · Release Manager · about 15 minutes with the artist.

## What the artist gets

- Work registration sheet per song
- Split and IPI verification
- Assisted registration plan per PRO and The MLC (you confirm each)
- Registration tracker (song, date, work ID, status)

## Ask first

- Song titles, writers, and splits
- Each writer's PRO and IPI (if known)
- Release info (ISRC, release date) from your catalog

## Steps

1. Check catalog metadata completeness
2. Verify splits total 100%
3. Plan the registration per destination
4. You confirm; the runner fills the form
5. Track confirmations

## Guardrails

- Won't register splits that don't total 100%
- Never changes splits without your direction
- Nothing is submitted without your confirmation

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: source-bound composition registration worksheet or explicitly authorized portal plan.
1. Use the requested case's supplied composition title, writers and reported shares. Do not pull account catalog for a separate fictional case. Unknown legal names, affiliations, IPI, publisher, roles, performer, links and existing registrations remain unknown. Never fill missing links with none or infer composer/lyricist roles.
2. Calculate the supplied split total but arithmetic is not rights verification. Preserve reported/unverified labels. Do not silently convert composition ownership shares into a society's writer/publisher pool convention. Missing split documentation is unknown, not absent or a universal legal prerequisite.
3. Without a selected society and current official requirements, list fields to check rather than declaring universal required or exempt fields. Composition and recording identifiers must stay distinct; do not assume a recording ISRC proves work ownership or is universally required or exempt. Do not group all collector types as sound recording registration or assume US collector scope.
4. Draft-only work saves a worksheet and missing inputs, not a portal plan, catalog export, submission or affiliation change. Use plan_royalty_registration only for an explicitly requested supported destination after applicable fields and authority are established. Current bulk-delivery routes and membership rules require sources, not remembered assertions.
5. Call create_document (type "checklist", skill "register-tracks-with-pro"). Keep proposed future steps separate from completed actions and never claim registrations or verified rights from a draft.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

If the Artispreneur MCP server is connected, these read-only tools help:

- `plan_release`: Plan a music release timeline.

## Starter

> Help me register my songs with my PRO. Ask me for each song's title, writers, and splits first.
