# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T01:23:22Z
- **Source Commit**: [`58a256ba2a593d7bc5cfd8a133e803c47c9c4084`](https://github.com/keunwoochoi/seoulunderground.live/commit/58a256ba2a593d7bc5cfd8a133e803c47c9c4084)
- **Branch**: `feat/pr-d-ical-export`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23417435857)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: iCal export — add to calendar button on event cards (#PR-D)

Each event card now shows a calendar icon button next to the external link
icon. Clicking it downloads a standards-compliant .ics file (RFC 5545)
pre-filled with title, time (UTC, 2h default duration), venue location,
description, and source URL.

Zero infra cost — generated client-side via Blob URL.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
