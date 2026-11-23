---
name: create-an-artist-bio
description: "Artist Bio Writer for independent musicians and artist managers. One story, told at every length you'll ever need. Use when an artist asks for help with Artist Bio Writer (Studio). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Artist Bio Writer

One story, told at every length you'll ever need.

Artispreneur skill `create-an-artist-bio` · Studio · Publicist · about 10 minutes with the artist.

## What the artist gets

- One-line tagline
- 50-word short bio
- 150-word Spotify bio
- 400-word press bio

## Ask first

- Artist name, genre, and city
- Origin story and influences
- Biggest credits (releases, shows, collaborators, press)

## Steps

1. Interview you for the story and credits
2. Find the through-line
3. Write all four lengths in one voice
4. Deliver to your Library

## Guardrails

- Uses only facts you provide
- No hype adjectives or invented milestones

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: four bios that tell one consistent story.
1. Use confirmed name, genre, city, origin, influences, and real credits already supplied. Do not infer pronouns. A fictional example does not authorize invented biography.
2. Find one through-line from those facts. Never invent track titles, gear/software, recording locations or methods, influences, collaborators, production duties, deals, future releases, or submission history. No press/awards/metrics is not evidence of never submitting work.
3. Target: tagline (≤15 words), 50-word, 150-word (Spotify), 400-word (press). Third person, present tense. Count words before labeling lengths. Accuracy wins over length: when facts are sparse, deliver shorter factual versions clearly labeled as shorter drafts, and ask ONE focused question after delivery. Do not add factual filler or pretend the target was met.
4. Review every factual sentence against the supplied or retrieved sources; remove unsupported details. Call create_document with all four under headings (type "bio", skill "create-an-artist-bio"). For shorter drafts label the heading by actual word count or as "Shorter factual draft", not the unmet target length. Keep missing-input questions outside the bios.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Write my artist bio in every length: tagline, 50-word, 150-word Spotify bio, and 400-word press bio. Ask me for my name, genre, and biggest credits first.
