---
name: add-music-to-collaborative-playlist
description: "Playlist Pitching for independent musicians and artist managers. Real playlist curators, honest pitches, no pay-for-play. Use when an artist asks for help with Playlist Pitching (Outreach). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Playlist Pitching

Real playlist curators, honest pitches, no pay-for-play.

Artispreneur skill `add-music-to-collaborative-playlist` · Outreach · Booking Agent · about 15 minutes with the artist.

## What the artist gets

- Target list of curators from the live directory
- Pitch messages per curator type
- Follow-up and tracking sheet

## Ask first

- The track, genre, and mood
- Release date and links
- Comparable artists

## Steps

1. Search the directory for fitting curators
2. Qualify each target
3. Write the pitches
4. Track responses

## Guardrails

- Only real curators from the directory
- Steers you away from pay-for-play and bot playlists

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: scoped playlist research or drafts, never guaranteed placement.
1. Preserve supplied genre, mood, release status and links; unknown ISRC, schedule, rights or assets remain unknown, not none. A draft-only no-search request saves readiness questions without searching, contacting, CRM writes or playlist changes. No account facts for a separate case.
2. Distinguish collaborative-access playlists, independent curators and platform editorial. Do not say every public collaborative playlist lets anyone add tracks, or that pre-save establishes editorial eligibility. Access, permissions, current deadlines and feature rules need current official sources for the selected platform.
3. Preliminary directory research does not universally require mastered audio, live release, ISRC, confirmed distribution, EPK or a fixed number of comparable artists. Mark only the inputs the requested next step actually needs. Do not invent eligibility gates or set an unknown pitch budget to zero.
4. When search is requested, name only actual returned records, verify fit/activity/submission route, and retain uncertainty. No invented curator names, links, fees, placements or guarantees. Draft pitches are not sent, and paid placement or bot-risk claims must match applicable verified terms rather than an unsourced universal rule.
5. Call create_document (type "target_list", skill "add-music-to-collaborative-playlist"). Keep optional future research/pitching separate from completed work; user-approved scope is required before contacts, accounts, sends, payments or playlist changes.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- The live Artispreneur industry directory (`search_directory`) is app-only: never invent contacts; work from contacts the artist supplies, or point them to the Artispreneur app.
- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me pitch my song to playlists. Ask me the genre, mood, and release date, then search the directory for curators.
