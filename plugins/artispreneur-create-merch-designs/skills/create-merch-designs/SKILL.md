---
name: create-merch-designs
description: "Merch Designs for independent musicians and artist managers. Merch your fans actually want to wear. Use when an artist asks for help with Merch Designs (Merch). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Merch Designs

Merch your fans actually want to wear.

Artispreneur skill `create-merch-designs` · Merch · Content Director · about 15 minutes with the artist.

## What the artist gets

- Product line plan (what, how many, price points)
- Design briefs per item
- Print specs and Canva-ready notes

## Ask first

- Your brand, lyrics, and inside jokes fans love
- Budget and audience
- Where you'll sell (shows, online)

## Steps

1. Plan the product mix
2. Brief each design
3. Set prices and margins
4. Deliver design briefs

## Guardrails

- Describes designs — image generation isn't part of this tool yet
- Flags trademark and lyric/artwork rights

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: the requested merch design brief with honest economics.
1. Preserve requested item count, materials, colors, exact words and exclusions. One tote does not become a3–5item product line. Unknown audience, demand, preorder data, vendor, price, rights or available cash remain unknown. A budget ceiling is not available cash.
2. Design choices may be optional proposals, not existing brand facts. Do not invent unit costs, sales volumes, profit forecasts or demand. Mark rights and trademark clearance unknown, never verified by originality alone. No image generation or purchases unless separately requested and authorized.
3. An empty margin worksheet keeps all unknown inputs blank. Separate per-unit costs from batch/setup costs and quantity: landed unit cost = variable unit cost + allocated batch costs/quantity. Unknown quantity prevents a unit-cost total. Include tax/duties, shipping/packaging, selling/payment fees and returns as applicable unknowns; distinguish gross margin from contribution and profit.
4. Do not make known retail price, demand or final cost a prerequisite for requesting a vendor quote. Proposed research steps are not performed actions. No vendor accounts, sends, uploads, production or spending for draft-only work.
5. Call create_document (type "plan", skill "create-merch-designs"). Never recommend a nonexistent Export to Canva control or imply a design brief is a generated print-ready image.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Plan my merch line and write design briefs. Ask me about my brand, fans, and budget first.
