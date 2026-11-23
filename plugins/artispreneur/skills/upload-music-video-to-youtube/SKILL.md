---
name: upload-music-video-to-youtube
description: "YouTube Upload for independent musicians and artist managers. Everything ready to upload your video to YouTube. Use when an artist asks for help with YouTube Upload (Content & marketing). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# YouTube Upload

Everything ready to upload your video to YouTube.

Artispreneur skill `upload-music-video-to-youtube` · Content & marketing · Content Director · about 10 minutes with the artist.

## What the artist gets

- Title, description, and tags
- Chapters and end-screen plan
- Thumbnail brief
- Premiere and Official Artist Channel checklist

## Ask first

- Video details and release date
- Links (streaming, merch, socials)
- Credits

## Steps

1. Write the metadata
2. Plan thumbnail and end screens
3. Set premiere and settings
4. Upload checklist

## Guardrails

- You publish from your own channel

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a truthful upload-kit draft for the actual video type.
1. Preserve supplied title, artist, duration, video type and status. A visualizer is not automatically an Official Music Video. Unknown file, thumbnail, credits, links, rights, audience classification or channel status remain unknown, not missing or absent. No account facts for separate cases.
2. Draft title and description using only supplied facts; no invented URLs, lyrics, releases or collaborators. Audience made-for-kids classification is the artist's unresolved decision, never a default. Use placeholders for unknown optional details, not false content.
3. Verify current applicable platform sources before asserting upload specs, limits, eligibility or feature requirements. Do not invent thumbnail dimensions, tag/hashtag limits or chapter/end-screen/card availability. An8-second item does not inherit every long-form feature.
4. Separate possible optional improvements (thumbnail, links, premiere, playlist, credits where applicable) from source-verified upload requirements. Do not make all unknowns complete-before-upload gates. Do not recommend a publish/schedule action as already approved by a draft request.
5. Call create_document (type "checklist", skill "upload-music-video-to-youtube"). No account sign-in, upload, scheduling, publishing or other external changes for draft-only work.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Get my music video ready for YouTube: title, description, tags, thumbnail brief, and a premiere plan. Ask me about the video first.
