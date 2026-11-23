---
name: get-ein
description: "EIN Registration for independent musicians and artist managers. Prepare a source-backed checklist before using the official IRS process. Use when an artist asks for help with EIN Registration (Legal entity). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# EIN Registration

Prepare a source-backed checklist before using the official IRS process.

Artispreneur skill `get-ein` · Legal entity · Business Manager · about 15 minutes with the artist.

## What the artist gets

- Private readiness checklist
- Non-sensitive supplied facts and open questions
- Current official source links and verification gaps

## Ask first

- Business structure (sole proprietor, LLC, corporation)
- Legal name, trade name and address
- Existing EIN and formation status (unknown is allowed); no tax ID in chat

## Steps

1. Clarify applicability and supplied facts
2. Read current official IRS sources
3. Save a non-sensitive readiness draft
4. Review the applicable official IRS process yourself

## Guardrails

- Never asks for, repeats or stores an SSN in chat
- The IRS charges nothing — warns about paid look-alike sites
- Nothing is submitted without your confirmation

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a source-backed private readiness draft, not an application or EIN. No assisted filing or tax-ID collection tool is available in this workflow.
1. Determine country/tax jurisdiction, entity structure, purpose and existing EIN status before applicability. Unknown existing EIN is not no EIN. Do not steer to entity formation or imply every artist/entity needs an EIN. A readiness-only request stays educational and does not start assisted filing.
2. Prep only non-sensitive answers supplied for this case. Missing names, addresses, dates and staffing remain unknown. Contractors are not automatically employees; do not infer payroll obligations. No immigration/citizenship question unless a verified applicable process requires it.
3. Current IRS rules, routes, identifiers, fees and exceptions must be verified against official sources and cited with actual retrieved URLs. No categorical SSN/ITIN requirement across all applicants: online eligibility and SS-4 foreign-responsible-party exceptions differ. If verification is unavailable, omit the rule and mark the specific question pending, not a categorical rule followed by a blanket unverified disclaimer.
4. Never ask for, repeat or store SSN/ITIN in chat or the saved note. No application, identifier collection or assisted-run tool for draft-only work. The artist must use the applicable official IRS process themselves; do not claim an EIN filing runner is available.
5. Call create_document (type "checklist", skill "get-ein") with source facts, unknowns and non-binding next questions. Say saved draft, never EIN issued, eligibility established or application submitted.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Walk me through getting an EIN for my music business, one question at a time. Ask me about my business structure first.
