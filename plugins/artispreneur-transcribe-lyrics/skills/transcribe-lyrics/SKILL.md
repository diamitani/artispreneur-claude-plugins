---
name: transcribe-lyrics
description: "Lyric Transcriber for independent musicians and artist managers. Clean, formatted lyrics ready for DSPs, videos, and liner notes. Use when an artist asks for help with Lyric Transcriber (Catalogue). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Lyric Transcriber

Clean, formatted lyrics ready for DSPs, videos, and liner notes.

Artispreneur skill `transcribe-lyrics` · Catalogue · Content Director · about 10 minutes with the artist.

## What the artist gets

- Formatted lyric sheet with sections
- DSP lyric-guideline pass
- Timing cues for lyric videos

## Ask first

- Your rough lyrics or a transcript
- Song structure (verses, hooks)
- Explicit content flags

## Steps

1. Take your draft
2. Correct and format sections
3. Apply DSP formatting rules
4. Add timing cues

## Guardrails

- Works from lyrics you paste — direct audio transcription is coming soon

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: DSP-ready lyrics.
1. Ask them to paste lyrics/transcript. Be clear audio isn't transcribed in this version.
2. Format: section labels, line breaks per sung phrase, consistent capitalization, no extra punctuation, repeated sections written out.
3. Flag explicit content and unclear words for the artist to confirm — never guess lyrics.
4. Add approximate timing cues per line if they give timestamps.
5. Call create_document (type "doc"). Offer the Lyric Video skill next.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Format my lyrics for streaming and a lyric video. I'll paste them — ask me about the song structure first.
