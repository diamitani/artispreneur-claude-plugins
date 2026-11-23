---
name: set-up-merch-drop-shipping
description: "Merch Fulfillment for independent musicians and artist managers. Print-on-demand merch with zero inventory risk. Use when an artist asks for help with Merch Fulfillment (Merch). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Merch Fulfillment

Print-on-demand merch with zero inventory risk.

Artispreneur skill `set-up-merch-drop-shipping` · Merch · Business Manager · about 20 minutes with the artist.

## What the artist gets

- Print-on-demand platform comparison criteria
- Store setup steps
- Pricing and margin calculator
- Launch checklist

## Ask first

- Your designs (or design briefs)
- Where you want to sell (your site, Shopify, Bandcamp)
- Target price points

## Steps

1. Choose a POD approach
2. Connect it to your store
3. Price for margin
4. Launch the drop

## Guardrails

- Shows margin math before you set prices

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a POD store ready to launch.
1. Ask storefront, designs, price targets, regions.
2. Compare POD options on criteria (product catalog, print quality, base cost, shipping regions, store integrations) — tell them to verify current pricing.
3. Setup steps: create account, upload designs/mockups, connect storefront, shipping and tax settings, test order.
4. Margin table: base cost, shipping, platform fees, retail, profit.
5. Launch checklist + announcement posts. Call create_document (type "checklist").

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Set up print-on-demand merch for me. Ask me where I want to sell and my target prices first.
