---
name: directory-search
description: "Industry Contact Finder for independent musicians and artist managers. Plan a high-fit industry contact list (blogs, playlists, radio, podcasts, press, venues) and organize contacts you supply into an outreach table. Use when an artist asks for help with Industry Contact Finder (Outreach). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Industry Contact Finder

Plan a high-fit industry contact list (blogs, playlists, radio, podcasts, press, venues) and organize contacts you supply into an outreach table.

Artispreneur skill `directory-search` · Outreach · Booking Agent · about 5 minutes with the artist.

## What the artist gets

- Up to 15 matched contacts, ranked by fit
- Outreach-ready table (name, contact, channel, genres)
- Suggested next tool to pitch them

## Ask first

- Channel: blog, playlist, radio, podcast, press or venue
- Your genres
- Market/city (for venues)

## Steps

1. Pick the channel
2. Match by genre and market
3. Rank by fit
4. Hand off to a pitch tool

## Guardrails

- Results come only from the Artispreneur directory — never made up
- Returns a focused list, not the whole directory

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a short, high-fit contact list ready for outreach.
1. Ask the channel (blog, playlist, radio, podcast, press, venue), genres, and market (venues).
2. Call search_directory filtered by channel + genre (+ market), limit 15.
3. Rank by genre match; drop poor fits. Never invent a contact or fill gaps from memory.
4. Present an outreach-ready table: name, outlet, contact method, channel, genres, notes.
5. Suggest the matching pitch skill (PR Campaign, Playlist Outreach, Booking Outreach) and offer to start it.
6. Call create_document (type "doc") with the list.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- The live Artispreneur industry directory (`search_directory`) is app-only: never invent contacts; work from contacts the artist supplies, or point them to the Artispreneur app.
- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Find me industry contacts that fit my music. Ask me which kind — blogs, playlists, radio, podcasts, press, or venues.
