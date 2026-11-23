---
name: build-a-skill
description: "Build a Skill for independent musicians and artist managers. Turn your workflow into a tool you can reuse, share, or sell. Use when an artist asks for help with Build a Skill (Meta). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Build a Skill

Turn your workflow into a tool you can reuse, share, or sell.

Artispreneur skill `build-a-skill` · Meta · Manager · about 20 minutes with the artist.

## What the artist gets

- A complete SKILL.md (name, description, playbook)
- Inputs, steps, and guardrails
- Packaging notes for Claude and other AI harnesses

## Ask first

- The workflow you repeat (step by step)
- What a great result looks like
- Mistakes to avoid

## Steps

1. Interview you on the workflow
2. Structure it into a playbook
3. Add guardrails
4. Deliver a SKILL.md

## Guardrails

- Keeps your private data out of the published tool

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a scoped, testable reusable workflow draft, not an installation claim.
1. Preserve supplied workflow, inputs, output, quality bar and failure modes. Respect a plain-text-only request instead of imposing packaging. Otherwise write portable SKILL.md with lowercase-hyphenated name and description frontmatter, Goal, Ask first, Steps, Deliverable and Never sections.
2. For numeric workflows, validate finite nonnegative inputs and required name/value pairs. Missing task estimates are unknown, never silently discarded or zeroed. Reject invalid negative/time inputs and ask only for the correction needed. Make priority assumptions explicit and overridable.
3. Never automatically split an indivisible task: splitting needs supplied permission; mark a permitted partial allocation unfinished. Proposed time allocations do not change original estimates. Include a worked example plus missing/invalid/zero and over-capacity cases, checking arithmetic exactly within permitted tools.
4. Strip personal data and secrets. Distinguish a saved document from installed instructions, persistent memory, custom tools, account entitlements or background automation. Packaging instructions need a verified target harness/version; do not promise universal compatibility.
5. Call create_document (type "doc", skill "build-a-skill") with the actual requested workflow. Final reply names the save accurately; never claim no tools were used after creating a document. No installs, account changes or external actions without their own approval.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Help me turn one of my workflows into a reusable AI tool. Ask me what the workflow is and what a great result looks like first.
