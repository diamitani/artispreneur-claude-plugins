---
name: analyze-social-media-engagement
description: "Engagement Audit for independent musicians and artist managers. See what's working, what's not, and what to post next. Use when an artist asks for help with Engagement Audit (Content & marketing). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Engagement Audit

See what's working, what's not, and what to post next.

Artispreneur skill `analyze-social-media-engagement` · Content & marketing · Content Director · about 15 minutes with the artist.

## What the artist gets

- Engagement audit by platform and format
- Top and bottom posts with reasons
- Five concrete changes for next month

## Ask first

- Your insights numbers (paste them) for recent posts
- Goals (followers, streams, ticket sales)
- Posting frequency

## Steps

1. Collect your numbers
2. Compare formats and topics
3. Find patterns
4. Recommend changes

## Guardrails

- Only analyzes numbers you provide — never invents benchmarks as your data

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: an honest audit with next steps.
1. Use only this sample's supplied platform numbers and confirmed goal. If it is fictional, synthetic or a separate client, do not fill its identity, genre, goals or bottleneck from the account profile. Ask for missing inputs only when needed.
2. Compute engagement rates with explicit numerators, denominator, unit and period. Per-post audience rates, per-video view rates and monthly total rates are different; never call an average a monthly total. Do not rank platforms by mismatched denominators or infer reach from followers.
3. Without per-post rows, top/bottom content, format/topic/time effects and causes are unknown. Without two dated snapshots, growth is unknown. State that rather than inventing a ranking or trend.
4. Offer optional measurement experiments tied to missing evidence, with metrics to record. Do not claim Reels outperform Feed, Shorts convert better/cheaper, or any format is a proven winner without supplied evidence or a current cited source. A suggested cadence is an untested proposal, not a benchmark or prediction. Do not force five recommendations when only one or two are grounded.
5. Call create_document (type "doc", skill "analyze-social-media-engagement"). Separate supplied data, calculated results, unknowns and optional hypotheses. Never add an unsupported claim then assert that no benchmarks were invented.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Audit my social media engagement. I'll paste my recent post numbers — ask me which platforms and goals first.
