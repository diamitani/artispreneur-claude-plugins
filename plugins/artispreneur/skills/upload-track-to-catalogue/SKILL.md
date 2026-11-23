---
name: upload-track-to-catalogue
description: "Catalog Upload for independent musicians and artist managers. Build one complete catalog record per track: metadata, credits, splits, rights and registration status. Use when an artist asks for help with Catalog Upload (Catalogue). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Catalog Upload

Build one complete catalog record per track: metadata, credits, splits, rights and registration status.

Artispreneur skill `upload-track-to-catalogue` · Catalogue · Release Manager · about 10 minutes with the artist.

## What the artist gets

- Catalog entry per track (metadata with sources, credits, splits, status)
- Audio analysis (tempo, key, loudness, brightness) for WAV files
- Rights and registration status
- Next actions per track

## Ask first

- The audio file (MP3, WAV, FLAC, AAC/M4A, OGG)
- Credits and splits
- Registration status (PRO, MLC, SoundExchange)

## Steps

1. Upload the audio
2. Extract metadata and analyse
3. Record rights and splits
4. Log registration status
5. List next actions

## Guardrails

- Your catalog is private to your account
- Duplicate detection depends on the upload path and an actual hash comparison; never guarantee it without a returned match
- No invented genre, artist or year

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: a source-labeled catalog save or audit, not rights registration.
1. New-file uploads use Catalogue or ingest_catalog_audio with an actual accessible audio URL. For an existing saved record use export_master_catalogue format json with trackId; never re-upload or demand a public URL just to read its fields. Only a successful returned row establishes a save. Do not claim extraction did not run merely because this chat did not call ingest_catalog_audio.
2. Preserve returned container facts, artist-supplied overrides, tags, filename guesses and uncertain analysis separately. Unknown identifiers, credits, splits and registration remain unknown, never unregistered, unclaimed or no agreement on file. Account-level PRO intake does not prove a particular recording's registration status. Do not let a roadmap override supplied private-demo scope.
3. BPM/key estimates need actual returned sources and caveats. No invented LUFS from RMS, genre, date, owner or credits. Use the artist's local date for audit date. A local catalog save is not a PRO filing, release, registration, rights verification or clearance.
4. No universal private-demo gates for ISRC/UPC, two100% split pools, PRO/MLC/SoundExchange, public release, EPK or assets. Request only what the next authorized step needs; jurisdiction and destination rules require current sources. Later possible release work is optional, never completed work or a required checklist now.
5. Duplicate detection is confirmed only by an actual full-content hash comparison and returned match. Direct uploads and URL ingestion may differ; never promise dedupe universally. A failed or absent dedupe check remains unverified. No reanalysis, external checks, registration or account mutations outside scope.
6. Save the requested source table/audit via create_document (type "doc", skill "upload-track-to-catalogue") or return an actual export. State what was read, saved and left unknown without claiming the record was unchanged unless that was checked.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Add a track to my catalog: metadata, credits, splits, and registration status. I'll upload the file.
