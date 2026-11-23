---
name: track-royalties-on-dsps
description: "Royalty Tracker for independent musicians and artist managers. Every royalty stream in one tracker, so nothing slips through. Use when an artist asks for help with Royalty Tracker (Finance). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Royalty Tracker

Every royalty stream in one tracker, so nothing slips through.

Artispreneur skill `track-royalties-on-dsps` · Finance · Release Manager · about 20 minutes with the artist.

## What the artist gets

- Map of every royalty stream you're owed
- Monthly royalty tracker template
- Gap check: accounts you haven't set up

## Ask first

- Your distributor and PRO
- Whether you're registered with The MLC and SoundExchange
- Recent statements (paste totals)

## Steps

1. Map your streams
2. Find registration gaps
3. Build the tracker
4. Set a monthly reconciliation routine

## Guardrails

- Works from statements you provide — no account logins

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a complete royalty map and tracker.
1. Use only supplied statements and reported registration status. Missing status is unknown, not a registration gap. Establish jurisdiction before applying collector scope or eligibility; a fictional case cannot inherit account-profile facts, even in a privacy assurance footer.
2. Preserve source labels. A distributor or publisher name alone does not establish the royalty subtype, platform or territory. Publisher receipts may contain multiple streams; mark subtype unknown unless stated. Describe only confirmed collection channels, with optional research questions separate.
3. Net reported is not net received, paid or bank-reconciled. Keep statement period, usage period, payment date and payment status separate. Unknown rights shares cannot be inferred from net/gross or fees.
4. Tracker: period, reported source, platform/territory if known, gross, fees, net, payment status and statement link. Compute exact totals, preserving currency and avoiding double-counting statements covering the same receipts. Flag any discrepancy, not only an invented 5% tolerance. Proposed monthly routine and dates are optional, not collector deadlines. Do not infer unpaid balances or verified eligibility.
5. Call create_document (type "budget", skill "track-royalties-on-dsps"). No bank access, registrations, claims or account changes.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me track all my royalties across streaming. Ask me my distributor, PRO, and what I'm registered with first.
