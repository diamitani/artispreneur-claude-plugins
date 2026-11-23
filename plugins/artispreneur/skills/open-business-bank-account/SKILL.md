---
name: open-business-bank-account
description: "Business Bank Account for independent musicians and artist managers. Walk into the bank (or app) with everything they'll ask for. Use when an artist asks for help with Business Bank Account (Finance). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Business Bank Account

Walk into the bank (or app) with everything they'll ask for.

Artispreneur skill `open-business-bank-account` · Finance · Business Manager · about 10 minutes with the artist.

## What the artist gets

- Document checklist for your entity type
- Questions to ask any bank
- Account setup plan (checking, savings for taxes, card)

## Ask first

- Entity type and state
- Monthly income and how you get paid (DSPs, shows, merch)
- Banking preferences

## Steps

1. List required documents
2. Compare what matters (fees, deposits, integrations)
3. Plan your account structure

## Guardrails

- No specific bank endorsements — criteria you can apply anywhere

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a source-bound bank-readiness draft, not an account application.
1. Use supplied facts only. Ask or mark unknown the country, entity, tax residence, income sources and volume, existing accounts and banking needs. Music project does not imply DSP, show or merch revenue. Do not import account facts for a separate case.
2. Without a selected bank, jurisdiction and current official bank requirements, do not prescribe ID, EIN, SSN, formation documents or deposit insurance as universal requirements. List questions to verify instead. Never collect sensitive identification or claim eligibility.
3. Comparison questions can cover fees, deposit methods, access, integrations, local deposit protection and transfer limits. No unsupported fee quotes or bank endorsements. Current exact requirements need actual retrieved bank sources.
4. Account structure is optional, never a default checking/savings/card bundle or fixed tax percentage. A draft-only request performs no application, card request, fee, transfer or account change.
5. Call create_document (type "checklist", skill "open-business-bank-account"). Preserve unknowns and clearly separate confirmed facts, possible questions and bank-specific checks.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Get me ready to open a business bank account for my music. Ask me my business type and how I get paid first.
