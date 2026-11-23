---
name: generate-social-media-content
description: "Social Content Pack for independent musicians and artist managers. Platform-native posts in your voice, ready to publish. Use when an artist asks for help with Social Content Pack (Content & marketing). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Social Content Pack

Platform-native posts in your voice, ready to publish.

Artispreneur skill `generate-social-media-content` · Content & marketing · Content Director · about 10 minutes with the artist.

## What the artist gets

- Posts tailored per platform (IG, TikTok, X, Threads, YouTube Shorts)
- Hooks and captions
- Hashtag and CTA suggestions

## Ask first

- What you're promoting and when
- Your voice (examples help)
- Platforms

## Steps

1. Learn your voice
2. Write per-platform posts
3. Add hooks and CTAs
4. Deliver a caption set

## Guardrails

- No invented stats, quotes, or collaborators

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: ready-to-post, platform-native content.
1. Ask what's being promoted, date, platforms, and voice examples.
2. Deliver the exact requested count per platform. Hook in the first line, correct length, format notes (on-screen text for TikTok/Reels), optional CTA. Keep production instructions separate from publishable caption text.
3. Use confirmed assets only. Unless audio was actually provided and inspected, never invent a pad, motif, melody entrance, instrument, beat drop, harmonic swell or resolution at timestamps. Script neutral timing such as play supplied preview seconds0–10; label edits and visual motion as proposed editing directions, not existing features. Do not assume extra audio segments exist.
4. Never say out everywhere, now streaming, link in bio, pre-save, sold out or similar distribution/availability claims unless supplied or verified. A release date is not proof of distribution destinations. Label missing link placeholders and tell the artist to replace or omit them. Do not present unsupplied account links as real.
5. Suggest3–5relevant hashtags if appropriate. Call create_document (type "captions", skill "generate-social-media-content"). Draft only, never claim publication or scheduling. Offer the Lyric Video skill or a promo video next.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Write social posts for my release, tailored to each platform. Ask me what I'm promoting, the date, and my platforms first.
