# Artispreneur

All 48 Artispreneur music business skills and all 7 Artispreneur desks as agents, plus the read-only Artispreneur MCP server, for independent musicians and artist managers: EPKs and bios, LLC, EIN and taxes, split sheets and contracts, PRO and royalty registration, release planning and distribution, content, merch, playlist, press and booking outreach. Drafts only; nothing is filed, sent, published or paid.

Published by Artispreneur Inc. (https://www.artispreneur.com). Version 1.1.1.

## What's inside

- 48 skills in `skills/`, one per Artispreneur skill, each loaded by its description or run as `/artispreneur:<skill>`.
- 7 desk agents in `agents/` (Claude Code and Cowork) and the same 7 desks as `<desk>-desk` skills, so they also work in claude.ai chat, which ignores agents.
- `.mcp.json` pointing at the public, read-only Artispreneur MCP server.

Skills:

- `create-an-epk`: EPK Builder
- `create-an-artist-bio`: Artist Bio Writer
- `create-brand-logo`: Brand Logo
- `write-brand-guidelines`: Brand Guidelines
- `create-split-sheet-agreement`: Split Sheet Agreement
- `license-music`: Music Licensing Brief
- `get-ein`: EIN Registration
- `create-llc`: LLC Formation
- `create-c-corp`: C-Corp Formation
- `open-business-bank-account`: Business Bank Account
- `manage-business-expenses`: Expense Manager
- `file-business-taxes`: Business Tax Filing
- `track-royalties-on-dsps`: Royalty Tracker
- `write-a-business-plan`: Business Plan
- `register-with-pro`: PRO Registration
- `register-tracks-with-pro`: Track Registration
- `claim-tracks-with-pro`: Unclaimed Royalties
- `set-up-dsp`: DSP Setup
- `release-music-with-dsp`: Release Engine
- `extract-metadata-from-track`: Metadata Extractor
- `transcribe-lyrics`: Lyric Transcriber
- `upload-track-to-catalogue`: Catalog Upload
- `create-content-calendar`: Content Calendar
- `generate-social-media-content`: Social Content Pack
- `create-lyric-video`: Lyric Video
- `write-music-video-treatment`: Video Treatment
- `upload-music-video-to-youtube`: YouTube Upload
- `analyze-social-media-engagement`: Engagement Audit
- `create-merch-designs`: Merch Designs
- `set-up-merch-drop-shipping`: Merch Fulfillment
- `add-music-to-collaborative-playlist`: Playlist Pitching
- `artist-profile`: Artist Profile
- `artist-goals`: Goal Setting
- `weekly-win-plan`: Weekly Win Plan
- `brand-positioning`: Brand Positioning
- `pr-campaign`: PR Campaign
- `media-outreach`: Media Pitching
- `playlist-outreach`: Playlist Curator Pitching
- `booking-outreach`: Booking Outreach
- `directory-search`: Industry Contact Finder
- `distribution-readiness`: Distribution Readiness
- `royalty-readiness`: Royalty Readiness
- `budget-planning`: Budget & Runway
- `contract-intake`: Contract Explainer
- `legal-business-checklist`: Business Setup Checklist
- `knowledge-ingestion`: Teach Your Agent
- `build-an-agent`: Build an Agent
- `build-a-skill`: Build a Skill

## What it connects to and sends

The plugin declares one remote MCP server, `https://www.artispreneur.com/mcp` (Artispreneur public MCP, version 1.2.1), over HTTPS with no sign-in. Its tools are read-only: they return public playbooks, desk starters, pricing, an EPK outline and computed release checklists. When Claude calls a tool it sends only that tool's arguments, such as a skill slug, an EPK audience or a release date. The plugin has no hooks, scripts or executables, reads no files or credentials, and stores nothing. Skills work without the server; they then run from the instructions in this folder.

Legal, tax and financial content is general information, not professional advice. Have a lawyer, accountant or other professional review anything binding before you rely on it.

## Install

In Claude Code:

```
/plugin marketplace add diamitani/artispreneur-claude-plugins
/plugin install artispreneur@artispreneur
```

On claude.ai or in Claude Desktop, upload this folder as a zip from Customize > Plugins (Add > Upload plugin), or upload a single skill zip from Customize > Skills.

## Example prompts

- Build my release plan for a single coming out on 2027-03-06.
- Write my artist bio in 50, 150 and 400 words.
- Walk me through forming an LLC for my music business.

## Support

https://www.artispreneur.com/support · pat@artispreneur.com · Privacy: https://www.artispreneur.com/legal/privacy · Terms: https://www.artispreneur.com/legal/terms
