---
name: create-llc
description: "LLC Formation for independent musicians and artist managers. Separate your music money from your personal money. Use when an artist asks for help with LLC Formation (Legal entity). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# LLC Formation

Separate your music money from your personal money.

Artispreneur skill `create-llc` · Legal entity · Business Manager · about 25 minutes with the artist.

## What the artist gets

- State-by-state filing plan for your state
- Operating agreement outline
- Post-filing checklist (EIN, bank, PRO publisher, DBA)

## Ask first

- State you live and operate in
- Solo or with partners
- Business name ideas

## Steps

1. Pick the formation state
2. Check name availability steps
3. Walk the state filing
4. Plan everything after approval

## Guardrails

- State fees vary — shown as a range to verify on your state's site
- General information, not legal advice — review anything binding with a lawyer.

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: an LLC filing in motion.
1. Establish country/jurisdiction, existing entity and the artist's decision. A consideration/readiness request is not approval to form an LLC. For separate fictional cases do not use account profile, city, catalog, PRO status, career stage or goals. Unknown income is not zero and solo songwriter is not proof no business partners exist.
2. Without jurisdiction and applicable sources, discuss questions rather than assert tax classification, liability protection, default formation state, bank requirements, legal effects or required memberships. Do not invent fees, examples, tax-saving claims, income thresholds or milestones. An unverified label does not make an invented figure useful.
3. Separate optional entity choices, missing inputs and verified requirements. Recommend a qualified local professional for actual entity/tax advice without prescribing credentials/titles or paid consults as mandatory. Do not imply every artist needs an LLC, EIN or publisher entity.
4. If an actual filing plan is later requested, research the relevant official jurisdiction rules first, preserving current sources and limits. Never promise protection, savings, approval or timing. No identifiers, applications, purchases or account changes for a draft-only case.
5. Call create_document (type "checklist", skill "create-llc") with source facts, unknowns and non-binding questions. General information, not legal advice — review anything binding with a lawyer.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Walk me through forming an LLC for my music business. Ask me which state I'm in and whether I have partners first.
