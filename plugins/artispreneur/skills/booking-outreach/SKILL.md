---
name: booking-outreach
description: "Booking Outreach for independent musicians and artist managers. Venue and promoter outreach for the cities and dates you want. Use when an artist asks for help with Booking Outreach (Outreach). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Booking Outreach

Venue and promoter outreach for the cities and dates you want.

Artispreneur skill `booking-outreach` · Outreach · Outreach Manager · about 20 minutes with the artist.

## What the artist gets

- Booking inquiry email template
- Matched venue/promoter list for your market
- Follow-up sequence
- Show tracker: venue, date, status, offer

## Ask first

- Target city/region and date range
- Draw you can honestly expect (or past show numbers)
- Your EPK link

## Steps

1. Set the market and dates
2. Write the inquiry
3. Match venues
4. Track to confirmed shows

## Guardrails

- Never overstate draw — bookers check
- Never invent facts, numbers, contacts, or credits — ask, or leave it out.

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: truthful booking drafts within the requested scope.
1. Preserve supplied city, proposed window, set length and slot type as possibilities, not dates or availability commitments. Missing draw/history, gear, tech needs, fee, travel budget, assets and links remain unknown. No account facts for a separate case.
2. Never infer first show, minimal tech needs, reliable draw, flexible availability, self-funded travel or ability to share live video/EPK from missing data. Placeholders must cover the entire uncertain assertion, not only a detail after a false promise. Do not invent buy-on/fee offers or artist experience.
3. A generic draft needs no selected venue or research. Save a concise editable inquiry plus requested unknowns, with optional fields optional. An EPK is not a universal prerequisite to drafting or researching. If stating word count, actually count rather than guessing.
4. No unrequested follow-up sequence or7/14day commitment. Draft-only work calls create_document (type "pitch", skill "booking-outreach") and stops; no directory search, CRM, connected apps, sends, bookings, holds or spending.
5. Actual outreach needs verified recipient/venue fit and artist approval of recipients, sending identity, exact words and any commitment. Queued sends are not sent. A proposed date inquiry never establishes artist availability or a confirmed show.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.
- The live Artispreneur industry directory (`search_directory`) is app-only: never invent contacts; work from contacts the artist supplies, or point them to the Artispreneur app.
- Contact storage (`manage_contacts`) is app-only: keep contacts in the conversation.
- App actions (`find_app_actions`, `run_app_action`) are app-only: describe the next step instead of running it.

## Starter

> Help me book shows. I'll tell you the city and dates I want.
