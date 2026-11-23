---
name: release-music-with-dsp
description: "Release Engine for independent musicians and artist managers. A release plan that works backward from drop day. Use when an artist asks for help with Release Engine (Release & DSP). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Release Engine

A release plan that works backward from drop day.

Artispreneur skill `release-music-with-dsp` · Release & DSP · Release Manager · about 25 minutes with the artist.

## What the artist gets

- Dated rollout timeline counted back from release
- Distribution and metadata checklist (ISRC, UPC, credits)
- Editorial pitch plan
- Drop-week daily checklist

## Ask first

- Release title, type, and date
- Distributor
- Budget and promo assets you have

## Steps

1. Set the timeline from release date
2. Prep metadata and upload
3. Pitch editorial in time
4. Run drop week

## Guardrails

- Builds in distributor lead time and the 7-day editorial pitch window

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a source-bound release-readiness plan, not a date commitment.
1. Preserve supplied title, format, proposed date, distributor, budget and asset status. A proposed date is not approved. A budget ceiling is not cash available. Unknown assets, rights documents, profiles or identifiers are unknown, not absent or confirmed blockers. Never infer genre from a title or import another artist's catalog.
2. Keep confirmed facts, unknowns, source-verified requirements and optional ideas separate. Without a selected distributor/platform and current official sources, do not assert mandatory audio/artwork specs, identifiers, dual100% split sheets, upload lead times or editorial deadlines. No generic2–4week or7day rule as a confirmed requirement.
3. Calculate dates from the supplied target and local timezone, but label any proposed work windows as optional estimates, not service gates. Pre-save, Canvas, ads, outreach and daily content are optional, not mandatory readiness blockers. Actual platform feature specs and eligibility require sources.
4. Do not invent price ranges or allocations as if grounded by a ceiling. Show unknown costs and cash, and decisions needed before committing. No uploads, submissions, pitches, spending or release-date commitments for a draft-only request.
5. Call create_document (type "rollout", skill "release-music-with-dsp"). Final reply must describe actual limitations accurately, never claim no costs or rules were invented when the saved draft contains them.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

If the Artispreneur MCP server is connected, these read-only tools help:

- `check_release_readiness`: Check music release readiness.
- `plan_release`: Plan a music release timeline.

## Starter

> Build my release plan working back from my release date. Ask me the title, date, distributor, and budget first.
