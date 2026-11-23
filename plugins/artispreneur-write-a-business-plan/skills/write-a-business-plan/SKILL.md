---
name: write-a-business-plan
description: "Business Plan for independent musicians and artist managers. A real plan with real numbers — for you, a partner, or a lender. Use when an artist asks for help with Business Plan (Finance). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Business Plan

A real plan with real numbers — for you, a partner, or a lender.

Artispreneur skill `write-a-business-plan` · Finance · Manager · about 30 minutes with the artist.

## What the artist gets

- One-page executive summary
- Revenue streams and 12-month projections
- Costs, budget, and break-even
- Milestones and KPIs

## Ask first

- Current income by source
- Monthly costs
- Goals for the next 12 months

## Steps

1. Baseline where you are
2. Model revenue and costs
3. Set milestones
4. Write the plan

## Guardrails

- Projections use your inputs with stated assumptions — nothing invented

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a credible, numbers-first business plan.
1. Use supplied income, costs, audience, goals and audience for the plan. Missing confirmed income means income UNKNOWN, never factual $0. Unknown entity, rights paperwork, accounts, releases or audience remain unknown, never none formed/completed/active. Isolate fictional cases from account facts.
2. Separate confirmed facts, explicit hypotheses, missing inputs and proposed actions. Draft sections need not be filled with invented information. A financial forecast and break-even need confirmed revenue/pricing/volume and cost assumptions; otherwise show the missing inputs, not a forecast.
3. Show arithmetic using supplied costs only. A $600 recording ceiling plus $100 artwork is $700 planned ceiling, not cash available and not a quote. Unknown extra costs remain unknown, never a known minimum or expanded known ceiling. Do not invent distributor/collector fees, price ranges, market size, fan demographics or launch dates.
4. Proposed milestones require artist approval and should remain relative or undated if no horizon is supplied. Do not impose jurisdiction-specific registration, dual-pool split sheets, membership, entity formation or service gates without verified applicable rules. Verify current official terms/prices if a specific service comparison is requested; otherwise mark research pending.
5. Call create_document (type "plan", skill "write-a-business-plan"). Do not claim an export, upload or other action occurred, or recommend a nonexistent UI export control.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Write my music business plan with real numbers. Ask me about my current income, costs, and goals first.
