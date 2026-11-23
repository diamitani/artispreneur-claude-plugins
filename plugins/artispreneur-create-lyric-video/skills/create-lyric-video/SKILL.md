---
name: create-lyric-video
description: "Lyric Video for independent musicians and artist managers. Plan a kinetic lyric video: timed lyric lines, format, style and a scene list ready for an editor or the Artispreneur app to render. Use when an artist asks for help with Lyric Video (Content & marketing). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Lyric Video

Plan a kinetic lyric video: timed lyric lines, format, style and a scene list ready for an editor or the Artispreneur app to render.

Artispreneur skill `create-lyric-video` · Content & marketing · Content Director · about 15 minutes with the artist.

## What the artist gets

- Lyric video (HyperFrames) previewed in chat
- MP4 render in the cloud or on your computer
- Vertical, square, or landscape

## Ask first

- The lyrics for the section you want (hook or verse)
- Artist name and release date
- Format and vibe

## Steps

1. Pick the section
2. Break lyrics into timed lines
3. Build the video
4. Render the MP4

## Guardrails

- Uses your exact lyrics
- Short-form sections (6–40 seconds) for social

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a short kinetic lyric video.
1. Ask for the exact lyric section (hook/verse), artist name, release date, format (portrait default), vibe.
2. Split lyrics into lines of 2–7 words; time each 1.5–4s to match delivery (ask for rough timings if they have them).
3. When create_video is available on the artist's route, call it: title, format, style matching the vibe, artist, scenes = lyric lines, cta like "Out now" only if they gave a date.
4. When create_video is not available (free route), call create_document (type "doc", skill "create-lyric-video") with the timed lyric-line storyboard instead, and say plainly that video rendering is not available on the free plan. Never claim a video was previewed, rendered or saved when it was not.
5. Next steps point to the app UI (open the video in the Library to render the MP4, or upgrade for in-chat rendering), never to internal tool or function names.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Video rendering (`create_video`) is app-only: deliver the timed lyric lines, format and scene list so an editor or the Artispreneur app can render it.
- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Make a lyric video for my hook. Ask me for the lyrics, my artist name, the format, and the vibe first.
