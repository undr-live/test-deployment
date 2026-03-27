# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-27T14:04:26Z
- **Source Commit**: [`f7ef0b6aa1b9122b7b6d610f1999ae2ba7117e52`](https://github.com/keunwoochoi/seoulunderground.live/commit/f7ef0b6aa1b9122b7b6d610f1999ae2ba7117e52)
- **Branch**: `fix/jsonld-missing-fields`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23650047130)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: add missing JSON-LD fields for Google Search Console warnings

Adds all 6 missing fields to MusicEvent schema:
- endDate: same as startDate (best available — no end time in data)
- eventStatus: EventScheduled (always true for upcoming events)
- image: og-image.png fallback (no per-event images available)
- offers: price + ticket_link if available, else source URL
- performer: omit field entirely when empty (was [])
- description: already present, was already omitted when null

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
