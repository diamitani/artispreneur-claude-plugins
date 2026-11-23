---
name: weekly-win-plan
description: "Weekly Win Plan for independent musicians and artist managers. Your top 3 moves this week, ranked by what actually moves the needle. Use when an artist asks for help with Weekly Win Plan (Career). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Weekly Win Plan

Your top 3 moves this week, ranked by what actually moves the needle.

Artispreneur skill `weekly-win-plan` · Career · Manager · about 5 minutes with the artist.

## What the artist gets

- Top 1–3 actions for the week, ranked
- Who (which team) handles each
- What's overdue or blocked and how to unblock it

## Ask first

- Your current goals (or set them first)
- Open projects and deadlines
- Hours you have this week

## Steps

1. Review goals and open work
2. Find what's overdue or blocked
3. Rank by impact vs effort
4. Hand off the top action

## Guardrails

- Never more than 3 actions — fewer, better actions

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a short, ranked weekly plan that ends with action.
1. Use supplied goals and constraints. For a separate fictional case never pull the real artist's account goals, deadlines, collaborators or resources. Missing collaborators means unknown, not none.
2. Use supplied hours or ask once. Respect the requested horizon: next7days is a rolling7-day span anchored to the request date, not next Monday. For tomorrow, use the next calendar day in the artist's explicit timezone, never the server UTC day. If the current date/timezone is unavailable, use relative Day1–Day7labels rather than invent calendar dates. State the anchor convention if using exact dates.
3. Mark only source-supported overdue/blocked states; propose needed dependencies without claiming the artist owns a DAW, plugins, backup drive, reference files or installed apps. Label suggested folder paths and export settings as proposals, never actual saved files. Do not prescribe universal fader resets, high-pass cutoffs or EQ/compressor settings without source/audio evidence; use listening-based checks instead.
4. Rank at most3core actions by impact and effort. Add duration estimates and buffer so their sum fits available minutes; optional stretch is outside that budget. Session breakdown must agree with action durations and not reuse buffer for stretch. A daily cap remains a cap in fallback plans: never combine into a longer session without approval. After missed days, reallocate or drop enough work to fit the actual remaining sessions, preserving the minimum done outcome.
5. For each action: measurable done criterion, duration, dependencies, and only a real available team/skill or artist-manual work. Do not invent a Songwriting Partner tool or claim a mix/spec was verified without audio.
6. Offer action#1, do not start a booking or send. Call create_document (type "plan", skill "weekly-win-plan") titled by the actual requested horizon.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> What should I focus on this week? Look at my goals and open projects and give me my top 3 moves.
