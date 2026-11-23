---
name: budget-planning
description: "Budget & Runway for independent musicians and artist managers. A plain-language budget and runway for your release, tour, or year. Use when an artist asks for help with Budget & Runway (Finance). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Budget & Runway

A plain-language budget and runway for your release, tour, or year.

Artispreneur skill `budget-planning` · Finance · Business Manager · about 15 minutes with the artist.

## What the artist gets

- Budget by category (recording, marketing, travel, gear, fees)
- Runway: months of funds at your current spend
- Answer to your spend question ("can I afford X?")
- One recommended money move

## Ask first

- The project or period
- Money in (income) and money out (expenses) — rough is fine
- The decision you're facing

## Steps

1. Gather the numbers
2. Categorize
3. Calculate runway
4. Answer the question

## Guardrails

- General information, not tax advice — confirm with a CPA or tax professional.
- Uses only the numbers you give — no guessing your finances

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a budget a non-accountant can use to decide.
1. Use the supplied project/period, available cash, expected income, and planned expenses. A budget ceiling is not proof of available cash. Separate confirmed numbers, estimates, and unknowns. No projected income supplied means unknown, not a factual $0; a zero-income scenario must be explicitly labeled as an assumption.
2. Categorize recording/mixing/mastering, artwork/video, marketing/ads, PR, distribution, travel, gear, and other. Do not add fees, vendor quotes, taxes, or income not supplied.
3. Compute allocation totals, percentages and budget variance. Runway = confirmed available funds ÷ confirmed average monthly spend only when both are supplied and the period is recurring; otherwise mark N/A or unknown.
4. Answer only what the numbers establish. Allocations fitting a ceiling does NOT prove affordability or recoupment. Never say the artist can afford it without available cash and obligations. If asked for a budget only, do not invent an affordability question.
5. A cashflow checklist is a proposed plan, not a ledger: leave paid/spent status and due dates unconfirmed unless supplied. Keep every scenario tense explicit, including the final reply: planned unpaid costs are not money already spent. Label any suggested timing, reserve period or allocation change as optional and unapproved. Do not assume zero spent, pending invoices or actual payments. Recommend caution, never spending for its own sake. Defer tax questions to a professional.
6. Call create_document (type "budget", skill "budget-planning") with the numbers and a clearly marked assumptions/unknowns section. No money, bookings or settings are changed.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me budget for my release (or tour). I'll give you rough numbers.
