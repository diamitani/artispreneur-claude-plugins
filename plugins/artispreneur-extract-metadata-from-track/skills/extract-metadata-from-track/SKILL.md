---
name: extract-metadata-from-track
description: "Metadata Extractor for independent musicians and artist managers. Clean, complete metadata for every track in your catalog. Use when an artist asks for help with Metadata Extractor (Catalogue). Works draft-first in the conversation: it does not file, send, publish, sign or pay for anything."
---

# Metadata Extractor

Clean, complete metadata for every track in your catalog.

Artispreneur skill `extract-metadata-from-track` · Catalogue · Release Manager · about 10 minutes with the artist.

## What the artist gets

- Metadata read from the file (tags, format, duration, sample rate) with the source of every field
- Tempo and key from audio analysis (WAV) with confidence
- Completeness score and missing-field report
- Distributor-ready metadata sheet

## Ask first

- The audio file (MP3, WAV, FLAC, AAC/M4A, OGG) or a link
- Credits and splits
- Release details (ISRC, UPC, date) if not in the tags

## Steps

1. Upload or ingest the track
2. Read embedded tags and the container
3. Analyse tempo and key (WAV)
4. Look up the ISRC on MusicBrainz
5. Score completeness and list fixes
6. Deliver the sheet

## Guardrails

- Every value carries its source (tag, file, analysis, MusicBrainz); nothing is defaulted or guessed
- Keys under 60% confidence are left blank
- Compressed formats use tags for BPM/key until the analysis service is set up

## Playbook

This is the Artispreneur agent playbook for this skill, unchanged from the app.

Goal: source-labeled metadata from an actual file or saved owned catalog record.
1. For an existing record, call export_master_catalogue with format json and trackId to read the owned record inline. Do not send private export endpoints to fetch_web_page or require a new public audio URL/re-upload merely to read saved metadata. A failed public fetch does not prove account access unavailable. If the record is not found, report that specific limit.
2. For a new file use the Catalogue upload, or ingest_catalog_audio only with an accessible actual audio URL and permission to add the record. Streaming-page links are not master audio. Report actual returned container/tag fields, artist-supplied facts, filename guesses and analysis separately.
3. BPM/key are estimates only where actually returned. A constant tone or silence cannot establish a pulse or major/minor key. Never predict the actual returned confidence from an input description. Confidence/profile correlation is not a calibrated probability. Do not invent technical values, genre, release dates, identifiers, writers or rights.
4. Unknown credits/identifiers/rights are unknown, not unregistered, unpaid or absent. ISRC/UPC/PRO data are not universal prerequisites for a private demo; mark readiness requirements only for the requested destination with current sources. Any MusicBrainz lookup must actually run; no silent external enrichment.
5. Save the requested source table, analysis caveats, unknowns and relevant next checks via create_document (type "doc", skill "extract-metadata-from-track"). Retrieval is not reanalysis, upload, ownership verification, registry search or clearance. No mutations or new actions beyond authorized scope.

## Running it inside Claude

Return a draft in the conversation using supplied facts only. Mark missing facts [CONFIRM]. Do not call app-only tools, access accounts, save, send, publish, file, sign or pay. Catalog tools retrieve instructions only; planning tools (release readiness, release plan, EPK outline) compute checklists from what the artist supplies, not approvals. No tool executes a skill or builds an artifact. Legal and tax content is general information for professional review.

- Saving to the Artispreneur Library (`create_document`) is app-only: deliver the finished document in the conversation instead.

## Starter

> Extract the metadata from my track. I'll upload it or send a link — tell me what's missing after.
