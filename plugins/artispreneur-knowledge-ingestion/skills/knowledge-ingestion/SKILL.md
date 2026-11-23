---
name: knowledge-ingestion
description: "Teach Your Agent for independent musicians and artist managers. Turn pasted bios, contracts and past EPKs into confirmed, structured facts and a list of conflicts to resolve. Use when an artist asks for help with Teach Your Agent (Meta). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Teach Your Agent

Turn pasted bios, contracts and past EPKs into confirmed, structured facts and a list of conflicts to resolve.

Artispreneur skill `knowledge-ingestion` · Meta · Manager · about 10 minutes with the artist.

## What the artist gets

- Facts extracted from your document, for your artist record
- Summary routed to the right team
- List of conflicts with what's already on file

## Ask first

- The document (paste the text)
- What it should be used for (EPK, contract, brand, finances)

## Steps

1. Classify the document
2. Extract the facts
3. Check for conflicts
4. Confirm and save

## Guardrails

- You confirm every fact before it's saved
- Sensitive data (SSNs, bank numbers) is never stored

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: the artist's existing documents become reusable, confirmed facts.
1. Ask them to paste the document and say what it's for.
2. Classify only supplied purpose/domain; if no use is stated, label as general reference rather than inventing EPK needs.
3. Extract structured facts with their source note: names, credits, release status, dates, links, exact press quotes and terms. Keep working titles distinct from released titles, plans/ideas distinct from agreements, and budget ceilings distinct from available cash. Missing consent means consent unknown, never no agreement exists. Skip sensitive personal data.
4. Compare only authorized case sources, not the signed-in profile for a separate fictional artist. Preserve older/newer values and source ordering; mark a clearly newer revision as current proposed value without silently overwriting original notes. Conflicting undated values need confirmation.
5. Show extracted facts as a review draft, not independently verified truth. Keep unknowns explicit; do not invent recording methods, rights, author identity or source dates. Ask at most the requested number of confirmation questions.
6. Call create_document (type "note", skill "knowledge-ingestion") titled "Knowledge — <document>". Saving a note is not updating profile, persistent memory or roadmap. Final reply should point to the actual download card/link, never a generated internal document ID. Do not impose an EPK next step or prerequisite unless requested.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> I want to teach you about me. I'll paste a bio, old EPK, or contract — pull out the facts.
