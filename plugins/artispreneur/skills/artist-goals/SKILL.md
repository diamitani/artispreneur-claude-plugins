---
name: artist-goals
description: "Goal Setting for independent musicians and artist managers. Turn \"I want to blow up\" into 1–3 dated goals you can actually hit. Use when an artist asks for help with Goal Setting (Career). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Goal Setting

Turn "I want to blow up" into 1–3 dated goals you can actually hit.

Artispreneur skill `artist-goals` · Career · Manager · about 10 minutes with the artist.

## What the artist gets

- 1–3 measurable goals with a target number and a date
- Parked goals list
- The first concrete step toward the top goal

## Ask first

- What you want to happen (in your own words)
- Your timeframe
- Where you are today (numbers you know)

## Steps

1. Reflect the ambition in concrete terms
2. Pick 1–3 goals
3. Give each a number and a date
4. Name the first step

## Guardrails

- Never invent facts, numbers, contacts, or credits — ask, or leave it out.
- Goals use the artist's own baseline numbers, never assumed ones

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: 1–3 goals that are definite, measurable and dated (One Must Act: name the 100 first).
1. Ask what they want in their own words, their timeframe, and where they are today (streams, list size, shows, income — only what they know).
2. Translate vague ambitions into concrete outcomes: "more fans" → mailing list size, monthly listeners, ticket sales; ask which matters most.
3. Keep at most 3 active goals, supporting the artist's actual requested outcome. Two unfinished tracks do not mean both must be completed for one private demo. Proposed targets are unapproved; preserve scope and ask which track rather than adding mastering, commercial-release specs or ownership requirements.
4. For each goal: target, relative deadline or correctly calculated local date, measurement and optional fallback. Do not anchor local deadlines to the server UTC day when timezone is unknown. A private demo need not be mastered or a particular file format. Leave resources unknown and do not assume project files, plugins, backups or monitoring exist.
5. Name a first step with an explicit estimate. Include supporting tasks and buffer in the same weekly time budget before claiming feasibility. Suggested checklist and decision-log targets must be labeled optional, not new obligations. Park only goals the artist actually mentioned; missing audience data is not proof no audience exists.
6. Call create_document (type "plan", skill "artist-goals") titled "Goals — <name>". Draft only unless profile/roadmap changes are separately approved.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me set real goals for my music career. I'll tell you what I want — turn it into something I can measure.
