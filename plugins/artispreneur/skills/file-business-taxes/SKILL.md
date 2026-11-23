---
name: file-business-taxes
description: "Business Tax Filing for independent musicians and artist managers. Get organized for tax season instead of panicking through it. Use when an artist asks for help with Business Tax Filing (Finance). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Business Tax Filing

Get organized for tax season instead of panicking through it.

Artispreneur skill `file-business-taxes` · Finance · Business Manager · about 25 minutes with the artist.

## What the artist gets

- Which forms likely apply to your structure
- Document gathering checklist (1099s, statements, receipts)
- Deduction review by category
- Questions to bring to your CPA

## Ask first

- Business structure
- Income sources and the forms you received
- Expenses by category (or your tracker)

## Steps

1. Identify likely filings
2. Gather documents
3. Review deductions
4. Prep your CPA handoff or DIY plan

## Guardrails

- Doesn't file for you or give tax advice
- General information, not tax advice — confirm with a CPA or tax professional.

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: an organized tax packet and CPA handoff.
1. Use supplied jurisdiction, entity, reporting period and bookkeeping inputs. Missing jurisdiction means no specific forms, rates, deadlines, filing thresholds or tax elections can be prescribed. Ask the next jurisdiction question or create the requested general preparation draft.
2. Income minus expenses is an arithmetic difference only, not taxable profit, deductible expenses, cash balance or tax due. Paid expenses are not automatically claimed expenses. Never infer tax treatment, residency, entity, tax year or registration from an artist name or account profile.
3. Collect source records for only the supplied transactions and income streams. Additional record categories are optional if applicable, not a demand for every artist to produce tax forms, royalty statements, home-office records or entity documents. Missing documents means not supplied, not nonexistent.
4. Identify unknowns and neutral questions for a qualified local professional. No US-specific Schedule C/1099/QBI/Section179/S-corp checklist without US jurisdiction and current applicable sources. Do not universalize CPA/EA titles or require entity formation. Where relevant law is unverified, state research pending.
5. Keep the requested draft concise. Call create_document (type "checklist", skill "file-business-taxes"). No filings, payments, account access or claims are performed. General information, not tax advice — confirm with a CPA or tax professional.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me get my music business taxes organized. Ask me my business structure and income sources first.
