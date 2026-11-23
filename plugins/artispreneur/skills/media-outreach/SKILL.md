---
name: media-outreach
description: "Media Pitching for independent musicians and artist managers. Personal pitch emails for every journalist and blog on your list. Use when an artist asks for help with Media Pitching (Outreach). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Media Pitching

Personal pitch emails for every journalist and blog on your list.

Artispreneur skill `media-outreach` · Outreach · Outreach Manager · about 20 minutes with the artist.

## What the artist gets

- One personalized draft per contact
- Tracking sheet: contact, outlet, stage, date sent, next follow-up
- Follow-up schedule

## Ask first

- Your PR hook or campaign (or run PR Campaign first)
- Your target list — or let the agent build one from the directory
- Your EPK link

## Steps

1. Load the hook and list
2. Personalize each draft
3. Review together
4. Track and follow up

## Guardrails

- Nothing sends without your approval: each email waits for your OK
- Never invent facts, numbers, contacts, or credits — ask, or leave it out.

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: the requested press draft or authorized outreach workflow.
1. Preserve supplied artist facts, working-title and release status. Unknown press history, assets, dates, links or audience remain unknown, never debut/no assets. No account facts for a separate case. Do not promise to share full tracks, photos, artwork or other material unless availability and permission are confirmed.
2. A generic template request needs no recipient, directory research, contact record or connected-app access. Use clear placeholders only for necessary choices; optional fields stay optional. Do not invent a city, sonic details, biography, coverage reference or mandatory EPK/fact-count/bio-length prerequisite.
3. Personalization requires an actual verified recipient/outlet and source-grounded reason for fit. Placeholder examples are not artist facts. Keep proposed future offers and follow-up schedules optional rather than commitments or completed actions.
4. Draft-only work calls create_document (type "pitch", skill "media-outreach") and stops. Do not search, read apps, mutate CRM, queue sends or offer an account connection unless the artist's requested scope needs it. Existing connections never authorize outreach.
5. Actual outreach requires approval of recipient, sending identity and exact words; verify duplicate-pitch state only within authorized research. Any supported app send is separately reviewed, never reported as sent from a queued action.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.
- The live Artispreneur industry directory (`search_directory`) is app-only: never invent contacts; work from contacts the artist supplies, or point them to the Artispreneur app.
- Contact storage (`manage_contacts`) is app-only: keep contacts in the conversation.
- App actions (`find_app_actions`, `run_app_action`) are app-only: describe the next step instead of running it.

## Starter

> Write personalized pitch emails for my press list. Use my PR hook and help me find outlets if I don't have a list.
