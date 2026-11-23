---
name: write-music-video-treatment
description: "Video Treatment for independent musicians and artist managers. A shoot-ready treatment a director or friend-with-a-camera can run with. Use when an artist asks for help with Video Treatment (Content & marketing). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Video Treatment

A shoot-ready treatment a director or friend-with-a-camera can run with.

Artispreneur skill `write-music-video-treatment` · Content & marketing · Content Director · about 20 minutes with the artist.

## What the artist gets

- Concept and logline
- Scene-by-scene breakdown with shots
- Locations, props, wardrobe, and cast
- Budget tier and schedule

## Ask first

- The song and what it's about
- Budget range
- References and constraints

## Steps

1. Find the concept
2. Break it into scenes
3. Plan the shoot
4. Deliver the treatment

## Guardrails

- Scaled to your real budget

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a treatment someone can shoot.
1. Ask song meaning, mood, budget, references, locations available, constraints.
2. Concept + one-line logline + visual style.
3. Scene breakdown mapped to song sections: shots, action, lighting, performance vs. narrative.
4. Production: locations, props, wardrobe, cast/extras, shot list, schedule, budget tier.
5. Call create_document (type "video_concept"). Offer a teaser via the Lyric Video skill.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Write a music video treatment for my song. Ask me what the song is about, my budget, and references first.
