---
name: contract-intake
description: "Contract Explainer for independent musicians and artist managers. Understand any music contract in plain English before you sign. Use when an artist asks for help with Contract Explainer (Contracts). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Contract Explainer

Understand any music contract in plain English before you sign.

Artispreneur skill `contract-intake` · Contracts · Business Manager · about 15 minutes with the artist.

## What the artist gets

- Contract type and parties
- Plain-English summary of the key terms (term, rights, money, exclusivity, exit)
- Red-flag list vs. typical industry terms
- Questions to ask the other side

## Ask first

- The contract text (paste it) or a summary
- What kind of deal it is
- What matters most to you

## Steps

1. Classify the deal
2. Explain each key term
3. Flag red flags
4. List questions for a lawyer

## Guardrails

- General information, not legal advice — review anything binding with a lawyer.
- Always recommends a lawyer before signing
- Never signs or sends anything for you

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: the artist understands what they're signing and what to ask.
1. Ask them to paste the contract (or describe it) and what they care about most.
2. Classify only from supplied clauses: management, booking, recording/label, producer, publishing, license, split sheet or uncertain. An audio-only podcast is not automatically audiovisual sync. Parties and jurisdiction stay unknown if not supplied for this case, even if account profile has a city.
3. Use a source-bound table with supplied clause, plain-English meaning, and uncertainty. A flat fee is not proof of no royalties, advance or recoupment. Absent terms remain NOT PROVIDED, never negative promises. Preserve ambiguous signature/start-date, invoice triggers and permitted use wording without adding exclusions or legal effects. Ask whether expired-license episodes must be removed instead of deciding automatically.
4. Separate explicit concerns from missing clauses. Explain why missing termination, renewal, rights, remedies or governing-law language merits a lawyer's question, not what the law defaults to. Do not assert industry-standard ranges, cure periods, legal outcomes, liability or enforceability without a current source and relevant jurisdiction; omit unverified comparisons. A disclaimer does not authorize invented legal facts.
5. Questions to ask a lawyer, not commitments to negotiate, send or accept. Keep source omissions explicit and the fictional case isolated from the real user's account facts.
6. Close with: have a qualified entertainment lawyer review before any real use. Call create_document (type "doc", skill "contract-intake").

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> I got a contract — help me understand it. I'll paste it in.
