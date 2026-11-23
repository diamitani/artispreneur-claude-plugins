---
name: build-an-agent
description: "Build an Agent for independent musicians and artist managers. Design a project sub-agent: mission, scope, skills, guardrails and starter prompts. Use when an artist asks for help with Build an Agent (Meta). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Build an Agent

Design a project sub-agent: mission, scope, skills, guardrails and starter prompts.

Artispreneur skill `build-an-agent` · Meta · Manager · about 10 minutes with the artist.

## What the artist gets

- Agent spec: mission, tools, guardrails
- A new team (sub-agent) in your workspace
- Starter prompts for the new agent

## Ask first

- The project (tour, album, brand deal, label)
- What success looks like
- Which tools it should lean on

## Steps

1. Define the mission
2. Choose its tool set
3. Create the team
4. Hand off starter prompts

## Guardrails

- Sub-agents only use tools your account has unlocked

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a working project sub-agent (team).
1. Ask the project, deadline, success criteria, and which areas it covers.
2. Pick the base team style that fits (main, business, press, release, booking, content) and the skills it should use.
3. Write a 1–2 sentence mission (it becomes the team tagline and guides the agent).
4. Call create_sub_agent with name, mission, base_kind.
5. Give 3 starter prompts for the new desk. Optionally create_document with the agent spec (type "plan").

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Creating a workspace team (`create_sub_agent`) is app-only: deliver the agent spec and starter prompts so the artist can create it in Artispreneur or as a Claude subagent.
- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Build me a sub-agent for a specific project. Ask me what the project is and what success looks like first.
