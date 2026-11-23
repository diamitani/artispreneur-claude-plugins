---
name: royalty-readiness
description: "Royalty Readiness for independent musicians and artist managers. Make sure every royalty stream you're owed has somewhere to land. Use when an artist asks for help with Royalty Readiness (Publishing & PRO). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Royalty Readiness

Make sure every royalty stream you're owed has somewhere to land.

Artispreneur skill `royalty-readiness` · Publishing & PRO · Business Manager · about 15 minutes with the artist.

## What the artist gets

- Royalty map: performance, mechanical, neighboring, master — who collects each
- Your registration status for each
- Ordered to-do list (what to register first)

## Ask first

- Are you registered with a PRO (ASCAP, BMI, SESAC)?
- SoundExchange, publishing admin, distributor status
- Upcoming or past releases

## Steps

1. Explain the royalty types
2. Check each registration
3. Order the gaps
4. Hand off to registration tools

## Guardrails

- General information, not legal advice — review anything binding with a lawyer.
- Registration is done by the artist on official sites

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a source-grounded readiness map, never a promise all royalties are owed or collectible.
1. Establish jurisdiction, actual uses and artist roles before applying collector rules. Do not assume US. If unavailable, list jurisdiction questions and conditional research topics, not a universal registration sequence or eligibility finding.
2. Keep reported ownership separate from verified rights. No registration confirmation supplied means UNKNOWN, never no membership/account/registration. No identifier supplied means identifier unknown, not none assigned. Preserve this in the final summary too.
3. PRO, mechanical, neighboring/digital-performance and master/distribution streams vary by territory, use, contracts and role. Verify current official sources before claims about collection scope, retroactive windows, accrual, registration prerequisites, fees or who can claim. Do not rank by money at stake without actual statements or usage evidence.
4. Suggest the next missing fact to verify per stream and matching readiness/registration skill. Separate optional royalty administration from distributor upload gates. Existing released music is not evidence the artist needs a new distributor. Do not infer unpaid balances, guarantees or eligibility from ownership alone.
5. Call create_document (type "checklist", skill "royalty-readiness"). Draft questions and conditional actions only, no accounts, filings, claims or sends.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

If the Artispreneur MCP server is connected, these read-only tools help:

- `plan_release`: Plan a music release timeline.

## Starter

> Am I set up to collect all my royalties? Check what I'm missing.
