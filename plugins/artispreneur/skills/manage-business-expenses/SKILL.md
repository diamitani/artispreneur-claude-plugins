---
name: manage-business-expenses
description: "Expense Manager for independent musicians and artist managers. Know where every dollar goes — and keep the receipts that save you taxes. Use when an artist asks for help with Expense Manager (Finance). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Expense Manager

Know where every dollar goes — and keep the receipts that save you taxes.

Artispreneur skill `manage-business-expenses` · Finance · Business Manager · about 15 minutes with the artist.

## What the artist gets

- Expense categories built for musicians
- Tracking template (spreadsheet-ready)
- Weekly 15-minute money routine

## Ask first

- What you spend on now (studio, gear, travel, promo, software)
- Current tools (app, spreadsheet, nothing)
- How you get paid

## Steps

1. Build your category list
2. Set up the tracker
3. Create the weekly routine

## Guardrails

- General information, not tax advice — confirm with a CPA or tax professional.

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a system the artist will actually use.
1. Ask current spending, tools, income streams.
2. Categories: studio/production, gear, software, marketing/ads, travel, merch COGS, contractors (collect W-9s), fees (distribution, PRO), home office, education.
3. Tracker: date, vendor, category, amount, payment method, receipt link, business purpose. Populate only supplied facts. A studio rental does not establish a recording session; artwork does not establish cover art; travel does not establish a show. Keep business purpose [TO CONFIRM] unless supplied. A due date is not a transaction or travel date. Paid is not proof of cleared or reconciled funds. No receipt supplied means receipt not provided, not proof none exists.
4. Compute paid, unpaid and committed totals separately. Unused budget ceiling is not cash available. Do not invent tax jurisdiction, deductibility, clearance or audit-readiness rules. Optional categories, routines and proof requests must be marked proposed rather than factual obligations.
5. Routine: proposed weekly 15 minutes (log, gather receipts, reconcile), monthly review; tax planning requires confirmed jurisdiction and qualified advice.
6. Call create_document (type "budget", skill "manage-business-expenses"). General information, not tax advice — confirm with a CPA or tax professional.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Set up expense tracking for my music business: categories, a tracker, and a simple weekly routine. Ask me what I spend on now first.
