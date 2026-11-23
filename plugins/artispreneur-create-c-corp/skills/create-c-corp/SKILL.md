---
name: create-c-corp
description: "C-Corp Formation for independent musicians and artist managers. Incorporate for investors, a label, or scale — with eyes open. Use when an artist asks for help with C-Corp Formation (Legal entity). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# C-Corp Formation

Incorporate for investors, a label, or scale — with eyes open.

Artispreneur skill `create-c-corp` · Legal entity · Business Manager · about 30 minutes with the artist.

## What the artist gets

- Is a C-corp right for you? decision memo
- Incorporation steps (state, articles, bylaws, board, shares)
- Post-incorporation compliance checklist

## Ask first

- Revenue today and goals
- Plans to raise money or bring in partners
- State of operation

## Steps

1. Test whether an LLC or S-corp election fits better
2. Choose the state
3. Walk incorporation filings
4. Set up compliance

## Guardrails

- Explains double taxation and alternatives before you commit
- General information, not legal advice — review anything binding with a lawyer.
- General information, not tax advice — confirm with a CPA or tax professional.

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a clear decision, then a filing plan.
1. Use supplied facts only. No investment plans stated means plans unknown, never zero outside investment plans. Unknown entity, jurisdiction, residency, income or assets remain unknown. Never import account profile into a separate case.
2. A decision-preparation request gets a short neutral questions memo, not a formation recommendation or incorporation steps. Without jurisdiction and verified current sources, do not assert tax classification, QSBS rules/holding periods, deductions, liability, salary or distribution rules, payroll requirements or which structure fits most artists.
3. Compare only requested options at a question level when sources are missing: possible administrative effort, ownership needs, financing intent, local costs and ongoing obligations to research. Do not invent fees, thresholds, timelines, savings or investment preferences. Professional review is advice, not a fabricated legal prerequisite that two professionals must approve.
4. Actual filing instructions require established jurisdiction and applicable current official sources, plus a user request. Draft-only work performs no filings, identity collection, purchases, bookings or account changes.
5. Call create_document (type "plan", skill "create-c-corp"). Keep unknowns explicit and do not claim a disclaimer makes unsupported legal/tax assertions safe. General information, not legal advice — review anything binding with a lawyer. General information, not tax advice — confirm with a CPA or tax professional.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me decide whether to incorporate as a C-corp and walk me through it. Ask me about my revenue, partners, and goals first.
