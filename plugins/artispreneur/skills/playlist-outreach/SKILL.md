---
name: playlist-outreach
description: "Playlist Curator Pitching for independent musicians and artist managers. Short, curator-friendly pitches matched to playlists in your genre. Use when an artist asks for help with Playlist Curator Pitching (Outreach). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Playlist Curator Pitching

Short, curator-friendly pitches matched to playlists in your genre.

Artispreneur skill `playlist-outreach` · Outreach · Outreach Manager · about 15 minutes with the artist.

## What the artist gets

- Curator pitch template (link + 2 lines)
- Matched curator/playlist list from the directory
- Spotify editorial pitch draft (if pre-release)
- Tracking sheet

## Ask first

- Track link (or release date if pre-release)
- Genre and mood tags
- Comparable artists

## Steps

1. Write the curator pitch
2. Match playlists by genre
3. Draft the editorial pitch
4. Track responses

## Guardrails

- Never pay for placements — pay-for-play violates platform rules
- Never invent facts, numbers, contacts, or credits — ask, or leave it out.

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: requested curator draft or authorized, verified outreach.
1. Preserve artist, unreleased status and working-title qualifiers. Unknown links, comparables, sound details, target playlist and assets remain unknown. Draft templates must include requested unknowns notes, not only bracketed copy.
2. An independent-curator template is not an editorial pitch. Use only supplied facts, with clear placeholders for missing sound/mood/links. Fit is a hypothesis to verify, never a claim based on a placeholder name. Do not invent debut status, availability or promises to share assets.
3. Do not introduce universal release gates, current editorial deadlines, pay-for-placement rules or feature eligibility without applicable current sources. No fixed number of comparables or live track is a universal prerequisite for drafting or preliminary research.
4. Generic draft-only/no-research work calls create_document (type "pitch", skill "playlist-outreach") and stops. No directory, CRM, connected-app reads, send queue, sends or follow-up commitments unless requested. Existing app access is not outreach approval.
5. Actual researched outreach requires verified recipient/playlist fit, source-backed route, and artist approval of recipients, sending identity and exact words. Keep proposed actions, queued actions and actual sends distinct.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.
- The live Artispreneur industry directory (`search_directory`) is app-only: never invent contacts; work from contacts the artist supplies, or point them to the Artispreneur app.
- Contact storage (`manage_contacts`) is app-only: keep contacts in the conversation.
- App actions (`find_app_actions`, `run_app_action`) are app-only: describe the next step instead of running it.

If the Artispreneur MCP server is connected, these read-only tools help:

- `plan_release`: Plan a music release timeline.

## Starter

> Help me pitch my song to playlist curators. I'll give you the link and genre.
