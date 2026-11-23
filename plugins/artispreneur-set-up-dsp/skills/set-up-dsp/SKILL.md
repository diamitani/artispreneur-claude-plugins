---
name: set-up-dsp
description: "DSP Setup for independent musicians and artist managers. Claim and polish your artist profiles on every streaming service. Use when an artist asks for help with DSP Setup (Release & DSP). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# DSP Setup

Claim and polish your artist profiles on every streaming service.

Artispreneur skill `set-up-dsp` · Release & DSP · Release Manager · about 15 minutes with the artist.

## What the artist gets

- Claim steps for Spotify, Apple Music, Amazon Music, YouTube (Official Artist Channel)
- Profile copy and image specs
- Pitching tools checklist

## Ask first

- Your distributor
- Whether you have a release live
- Bio, photos, and links

## Steps

1. Confirm a release is live
2. Claim each profile
3. Polish bio, images, and links
4. Set up pitching access

## Guardrails

- Claims need at least one release delivered by your distributor

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: every artist profile claimed and polished.
1. Ask distributor, released music, bio, photos, socials.
2. Explain claiming usually requires a release delivered through a distributor.
3. Steps per platform: Spotify for Artists, Apple Music for Artists, Amazon Music for Artists, YouTube Official Artist Channel (usually via distributor).
4. Profile polish: bio (use create-an-artist-bio), image guidance, links, artist pick.
5. Checklist including editorial pitching access. Call create_document (type "checklist").

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me set up my artist profiles on Spotify, Apple Music, Amazon, and YouTube. Ask me my distributor and whether I have music out first.
