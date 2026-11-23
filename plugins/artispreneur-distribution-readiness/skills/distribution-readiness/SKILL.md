---
name: distribution-readiness
description: "Distribution Readiness for independent musicians and artist managers. Everything checked before you upload — and the right distributor for you. Use when an artist asks for help with Distribution Readiness (Release & DSP). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Distribution Readiness

Everything checked before you upload — and the right distributor for you.

Artispreneur skill `distribution-readiness` · Release & DSP · Release Manager · about 15 minutes with the artist.

## What the artist gets

- Upload readiness checklist (masters, artwork, metadata, rights)
- Distributor comparison for your situation
- Blockers list with fixes

## Ask first

- Release type and date
- What's finished (masters, artwork, credits)
- Do you own all rights (samples, beats, features)?

## Steps

1. Confirm rights
2. Check assets
3. Check metadata
4. Pick a distributor

## Guardrails

- Unclear ownership (samples, leased beats) is flagged before upload
- General information, not legal advice — review anything binding with a lawyer.

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: no rejected uploads, no rights surprises.
1. Separate supplied artist claims, unknowns and verified requirements. Ownership claims are unverified; instrumental does not establish no featured artists or leased beats. No samples does not prove all other clearances. Unknown identifiers/credits are not absent identifiers/credits.
2. Final audio and artwork readiness are artist-reported until inspected. Exact audio/artwork specs, lead times and deadlines depend on the selected distributor and stores; verify current official requirements before presenting a gate. If no distributor is selected, list questions to check, not universal3000px/WAV/2–4week rules or calculated delivery deadlines.
3. Metadata checklist: title, artist names, contributors, rights, identifiers, explicit flag, language, release date and territories. Keep values unknown unless supplied; instrumental is not automatic explicit=false. Confirm who assigns ISRC/UPC before instructing purchases or acquisition.
4. Separate delivery blockers from optional promotion and royalty administration. PRO/MLC/SoundExchange memberships, pre-save/editorial pitches and a solo signed dual-pool split sheet are not universal upload prerequisites. Do not require them without a selected service's verified rule.
5. Compare distributors only if requested, with current official prices/terms or mark research pending. Draft checklist can say not ready based on confirmed unfinished assets without inventing gates. Call create_document (type "checklist", skill "distribution-readiness"). No signup, upload, fee or release guarantee.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

If the Artispreneur MCP server is connected, these read-only tools help:

- `check_release_readiness`: Check music release readiness.
- `plan_release`: Plan a music release timeline.

## Starter

> Am I ready to upload my release? Check everything and help me pick a distributor.
