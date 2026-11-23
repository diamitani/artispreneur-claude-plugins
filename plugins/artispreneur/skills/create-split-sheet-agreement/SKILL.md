---
name: create-split-sheet-agreement
description: "Split Sheet Agreement for independent musicians and artist managers. Everyone's share, in writing, before the song blows up. Use when an artist asks for help with Split Sheet Agreement (Contracts). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Split Sheet Agreement

Everyone's share, in writing, before the song blows up.

Artispreneur skill `create-split-sheet-agreement` · Contracts · Business Manager · about 10 minutes with the artist.

## What the artist gets

- Split sheet with writers, roles, and percentages
- PRO/IPI and publisher fields
- Signature and date block
- How-to-bring-it-up talking points

## Ask first

- Song title and date
- Every contributor, their role, and agreed percentage
- PRO and publisher info (if known)

## Steps

1. Collect contributors and roles
2. Check splits total exactly 100%
3. Fill PRO/publisher fields
4. Deliver a signable draft

## Guardrails

- Won't finalize unless splits total 100%
- General information, not legal advice — review anything binding with a lawyer.

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a signable split sheet.
1. Use supplied song title, date, contributors, roles, percentages, PRO, IPI and publisher. Never infer songwriter/producer roles from a composition percentage; missing roles and identifiers stay [TO CONFIRM]. Ask for missing details without blocking a clearly requested proposed draft.
2. Verify composition shares total exactly100% with master/producer points a separate pool only if requested. Proposed is not agreed: unless agreement is explicitly confirmed, use Proposed% column and proposed unsigned status everywhere, never Agreed%. Do not imply signatures, registrations, legal validity or consent exist.
3. Build song info, contributor table, publisher/PRO fields, blank signature/date lines for everyone. Never complete an unknown creation/agreement date, jurisdiction or personal identifier. A composition-only draft does not require a master agreement to be signed; label master rights outside scope when not requested.
4. Add review checklist and up to3talking points. Never promise ten-minute completion, months saved, painless licensing or any legal outcome. A master agreement is not a prerequisite in the composition-only checklist; optional separate master-rights work belongs outside that checklist. Include: General information, not legal advice — review anything binding with a lawyer.
5. Call create_document (type "contract", skill "create-split-sheet-agreement").

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Draft a split sheet for my song. Ask me the title, every collaborator, their role, and the agreed percentages first.
