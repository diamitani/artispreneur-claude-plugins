---
name: legal-business-checklist
description: "Business Setup Checklist for independent musicians and artist managers. The business basics — entity, copyright, licensing, PRO — in the right order. Use when an artist asks for help with Business Setup Checklist (Legal entity). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Business Setup Checklist

The business basics — entity, copyright, licensing, PRO — in the right order.

Artispreneur skill `legal-business-checklist` · Legal entity · Business Manager · about 15 minutes with the artist.

## What the artist gets

- Your business-readiness checklist with status
- Plain-language explanation of each item
- Real steps and typical fees, in order
- Which tool handles each next step

## Ask first

- Which topic: business entity, copyright, licensing, or PRO
- What you've already done
- Your state (for entity questions)

## Steps

1. Pick the topic
2. Explain it plainly
3. List the steps and fees
4. Hand off to the doing tool

## Guardrails

- General information, not legal advice — review anything binding with a lawyer.
- General information, not tax advice — confirm with a CPA or tax professional.
- Never collects SSNs or files anything for you

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: the artist knows what's done, what's next and why.
1. Ask which topics matter now (entity/LLC, copyright, licensing, PRO) — don't cover all four unless asked — and what's already done.
2. For each topic: what it is and why it matters, in two sentences.
3. Steps in order with typical fees labelled as general and "check your state/official site": e.g. EIN (free from the IRS), LLC (state filing fee varies by state), copyright registration (US Copyright Office fee), PRO membership.
4. Status checklist: done / next / later.
5. Point each next step to the doing skill (EIN Registration, LLC Formation, PRO Registration, Split Sheet Agreement, Music Licensing Brief).
6. Call create_document (type "checklist").

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> What business and legal setup do I need as an artist? Walk me through it in order.
