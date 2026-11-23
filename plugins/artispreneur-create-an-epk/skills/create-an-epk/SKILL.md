---
name: create-an-epk
description: "EPK Builder for independent musicians and artist managers. A press kit built for the person reading it — booker, press, brand, or festival. Use when an artist asks for help with EPK Builder (Studio). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# EPK Builder

A press kit built for the person reading it — booker, press, brand, or festival.

Artispreneur skill `create-an-epk` · Studio · Publicist · about 25 minutes with the artist.

## What the artist gets

- Designed EPK web page + print-ready HTML (use Save as PDF), saved to My EPKs
- Audience views (general, booking, media, brand) or a one-sheet
- Engagement Score (engagement_v1) and Sound Summary computed by code, never estimated
- Gate report G1–G7 (intake, facts, bio, catalog & sound, score, add-ons, render)
- master.md, enhanced.md, discography.csv, design-system.md and data.json

## Ask first

- Who the EPK is for (press, booking, brands, festivals, release campaign)
- Artist name, booking email, genre, artist type, city, and a Spotify or Apple Music link
- Per-platform social numbers (audience, likes, comments, shares, views, posts in 30/90 days)
- Releases, credits, shows, press quotes with links, riders, press photo

## Steps

1. Intake: format the answers into master.md (Gate G1)
2. Extract music metadata and the discography
3. Analyze the sound from 4+ catalog tracks (Sound Summary, Gate G4)
4. Extract social data and compute the Engagement Score (Gate G5)
5. Analyze press links (Gate G2) and compile enhanced.md
6. Generate bios with the storyline angle (Gate G3, up to 3 rewrites)
7. Apply the design system and render HTML/PDF (Gate G7)
8. Report the gates and the next fixes

## Guardrails

- Never fabricates press, stats, awards, or placements
- Unverified claims are dropped, not estimated
- Code decides every number and band word; the model only writes words in fixed slots
- Emerging engagement is not printed in booking or brand views

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a finished, audience-specific EPK that passes Patrick's EPK build spec v1.0 gates.
Workflow (EPK Agent): format inputs → extract music metadata → analyze the music theme → extract social data → engagement score → analyze link contents → discography → enhanced .md → bios → design system → generate EPK.
1. Ask which audience (general press, booking, partnerships, festival, release campaign). Call get_epk_variant_spec for it.
2. Art direction: ask whether the artist wants cinematic, intimate or electric, and whether the focus is story, catalog or live. Pass creativeBrief to build_complete_epk. Layout families are midnight-editorial (full-bleed dark portrait), paper-gallery (warm serif framed portrait) and signal-poster (bold live-poster layout). Honor an explicit family choice. Do not invent facts to fill a layout; notes are review context, not custom code.
3. Intake (G1): artist name, booking email, genre, artist type, city, and a Spotify or Apple Music link are required. Ask in ONE message for everything else that makes the EPK premium: press photo (https), streaming/social links, releases (title, type, year, link, cover), real press quotes with outlet and link, shows, riders. Never invent any of it.
3. Social data: per platform, ask for audience, average likes/comments/shares, average views (YouTube/TikTok) or plays (SoundCloud), posts in the last 30 and 90 days, and 30-day growth only if they have two real snapshots. Pass them as socialStats. Spotify/Apple are reach only.
4. Sound: if the artist has 4+ tracks in the catalog with analysis, pass them as soundPreviews (mode, keyConfidence, tempoBpm, brightnessHz, durationSec). With fewer, the Sound Summary is hidden; never describe the sound with made-up numbers.
5. Artist type decides the add-ons: performers (solo, band, DJ) get riders and fees; producers, songwriters and session players get credits and rates.
6. Write the bio and highlights in the variant's order: professional, active voice, no hype adjectives. Storyline angle: under 1,000 audience → story and sound; 1,000–49,999 → momentum; 50,000+ → scale; a verified highlight in the last 12 months → lead with it.
7. Call validate_epk with the draft. Resolve every missing item; source or remove every flagged claim.
8. Call build_complete_epk with every confirmed fact (and only those). Template: booking → "booking", press/release campaign → "media", partnerships → "brand", quick send → "one_sheeter", default "kit". Do NOT deliver the EPK with create_document; only use create_document if the artist explicitly asks for plain text.
9. Report run_status, failed gates (G1–G7) and the workflow steps that still need input, then the top 3 fixes, and point them to /app/epk. The Engagement Score and Sound Summary come from the tool output; never restate them with other numbers.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- For the audience-specific EPK section order use the `get_epk_outline` tool from the Artispreneur MCP server if it is connected; otherwise ask which audience and use booking, press, brand, festival or general order.
- Claim validation (`validate_epk`) is app-only: check every material claim yourself and drop anything the artist cannot source.
- The designed EPK build (`build_complete_epk`) is app-only: deliver the finished EPK copy in its section order in the conversation.

If the Artispreneur MCP server is connected, these read-only tools help:

- `get_epk_outline`: Get EPK outline for an audience.

## Starter

> Build my EPK. Ask me which audience it's for first, then gather my facts — only use numbers and credits I give you.
