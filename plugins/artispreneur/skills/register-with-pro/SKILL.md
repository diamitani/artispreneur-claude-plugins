---
name: register-with-pro
description: "PRO Registration for independent musicians and artist managers. Join ASCAP, BMI, or SESAC the right way — writer and publisher. Use when an artist asks for help with PRO Registration (Publishing & PRO). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# PRO Registration

Join ASCAP, BMI, or SESAC the right way — writer and publisher.

Artispreneur skill `register-with-pro` · Publishing & PRO · Release Manager · about 20 minutes with the artist.

## What the artist gets

- Which PRO fits you (and why)
- Writer (and publisher) application plan you review and confirm
- Assisted portal run: fields filled, your tax ID injected securely, you confirm the submit
- Key sheet: member and IPI numbers (no passwords)

## Ask first

- Country and whether you write/co-write your songs
- Any existing PRO, publisher, or admin deal
- Legal name, pen names, address, date of birth
- SSN/ITIN (or EIN for a publisher) — only in the secure form

## Steps

1. Choose a PRO and role
2. Collect your details
3. Add your tax ID in the secure form
4. Review and confirm the plan
5. Runner fills the portal; you handle login, ID check and fees
6. Save member/IPI numbers

## Guardrails

- One PRO per writer per territory — checks for conflicts first
- Your SSN/TIN never appears in chat, prompts or logs
- Nothing is submitted without your explicit confirmation
- No PRO has a public registration API; portals are filled with your confirmation

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: applicable PRO/CMO readiness or an explicitly requested registration plan.
1. Preserve supplied facts and unknowns. No collaborators stated does not establish sole ownership; missing affiliation is unknown, not unaffiliated. A separate case must not inherit account facts. Establish country and relevant residence, rights role and existing deals before selecting a society.
2. For readiness-only work, save confirmed facts, unanswered eligibility questions and next research steps. Do not collect legal identity, date of birth or tax identifiers when the artist asks for no identity collection. Do not make all possible fields prerequisites for every society. ISRC identifies a recording, not proof of composition ownership or a universal writer-membership requirement.
3. Society availability, exclusivity, fees, identification and membership requirements need applicable current official sources. No default ASCAP/BMI choice, one-society-per-territory rule, SSN/ITIN/EIN requirement or publisher registration requirement without verification. Do not present MLC/SoundExchange as universal next steps without jurisdiction and rights scope.
4. Actual portal planning requires a selected supported destination and explicit request beyond drafting. Only then use plan_royalty_registration with non-sensitive authorized fields. Never request tax identifiers in chat; use only the supported secure flow. No submission, fees, account changes or claim of successful affiliation without separate approval and confirmation.
5. Call create_document (type "checklist", skill "register-with-pro"). The final reply must accurately describe remaining unknowns and unverified requirements, not claim no rules were assumed when the draft asserts them.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me register with a PRO (ASCAP, BMI, or SESAC). Ask me where I'm based and whether I already have any deals first.
