---
name: create-content-calendar
description: "Content Calendar for independent musicians and artist managers. A posting plan you can actually keep up with. Use when an artist asks for help with Content Calendar (Content & marketing). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Content Calendar

A posting plan you can actually keep up with.

Artispreneur skill `create-content-calendar` · Content & marketing · Content Director · about 15 minutes with the artist.

## What the artist gets

- 30-day calendar by platform
- Content pillars and formats
- Batch-shoot shot list

## Ask first

- Platforms you post on and how often you can
- Upcoming releases or shows
- What's worked before

## Steps

1. Set pillars
2. Map the month
3. Plan batch shoots
4. Deliver the calendar

## Guardrails

- Built around your real capacity — not a 5-posts-a-day fantasy

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a realistic 30-day calendar.
1. Use the requested date range, not a default30days. Use confirmed platforms, weekly capacity and dates; do not infer releases, shows or prior wins. Keep a separate supplied-assets list.
2. Propose content pillars, clearly ideas rather than artist facts. Do not claim a synth, DAW, mix chain, alternate artwork, footage or behind-the-scenes file exists unless supplied.
3. Calendar table: exact weekday/date, platform, proposed hook, asset needed, optional CTA. Calculate weekday/date and countdown differences. An unavailable asset must be marked NEW TO CREATE with estimated effort, plus a fallback using only confirmed assets.
4. Respect zero budget: prefer the artist's existing assets and tools. Do not recommend trials, paid tools, subscription-dependent exports or promise a tool is free without a current verified source. A free-looking trial is not a zero-cost guarantee.
5. Count actual rows by platform before stating totals; totals must match the table, not a target. Separate proposed posts from published or scheduled posts. If capacity is unknown, offer a small reversible plan and label the effort estimate.
6. Call create_document (type "plan", skill "create-content-calendar"). Keep it a draft, never claim account scheduling or publication. Offer the Social Content Pack skill next.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Build my 30-day content calendar. Ask me my platforms, how often I can post, and what's coming up first.
