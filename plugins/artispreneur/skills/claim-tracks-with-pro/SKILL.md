---
name: claim-tracks-with-pro
description: "Unclaimed Royalties for independent musicians and artist managers. Find and claim royalties already owed to you. Use when an artist asks for help with Unclaimed Royalties (Publishing & PRO). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Unclaimed Royalties

Find and claim royalties already owed to you.

Artispreneur skill `claim-tracks-with-pro` · Publishing & PRO · Release Manager · about 20 minutes with the artist.

## What the artist gets

- Search plan across your PRO, The MLC, and SoundExchange
- Claim plan per missing work, filed with your confirmation
- Dispute/correction message templates
- Claim tracker with follow-up dates

## Ask first

- Your catalog (titles, writers, ISRCs)
- Your PRO and registrations
- Any statements showing gaps

## Steps

1. Royalty readiness check per stream
2. Search each database
3. Match missing or wrong entries (you pick the match)
4. File claims with your confirmation
5. Track outcomes

## Guardrails

- Only claims what you actually own or co-own
- Never guesses a match or promises an amount
- Nothing is filed without your confirmation

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: evidence-led royalty investigation, not an assumed unpaid balance.
1. Use supplied case facts only. Preserve reported ownership and unknown co-writers/shares, country, affiliations, statements and registration status. Unknown is not missing registration, unpaid royalties or money owed. No account catalog import for a separate case.
2. Draft-only work saves facts, unknowns and optional research questions. Choose applicable collectors only after jurisdiction, rights stream and affiliation are established. Do not assume US collector scope. Current search access, API approval and collector rules require official sources; do not confuse a public search page with an API.
3. Do not make full splits, signed agreements, ISRC, UPC or release data universal prerequisites for every preliminary title/writer search. Identify what a selected search actually needs and what remains necessary to establish a reliable match or authorize a claim. Composition and master evidence remain separate.
4. A possible match is not ownership proof, a registration gap is not proof of unpaid money, and statements need period/currency/payment reconciliation. Never invent matches, owed amounts, eligibility, deadlines or follow-up rules. Draft-only work makes no searches, exports, portal plans, contacts or claims beyond the requested scope.
5. Actual claim planning requires established rights, a verified matching record, selected supported destination and explicit approval. Call create_document (type "checklist", skill "claim-tracks-with-pro") for the evidence-gathering draft, with proposed future actions clearly separate from completed work.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me find and claim royalties I'm owed. Ask me for my catalog and which organizations I'm registered with first.
