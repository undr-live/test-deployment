# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-22T05:23:36Z
- **Source Commit**: [`f065a361edfb15c2c112aac62a52c503ecfdf805`](https://github.com/keunwoochoi/seoulunderground.live/commit/f065a361edfb15c2c112aac62a52c503ecfdf805)
- **Branch**: `fix/export-venue-tier`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23396430435)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: export venue tier field in static JSON

tier was missing from the venues export, causing all venues to default
to tier 1 in static mode. Tier-3 venues like @gc_jazzpicnic were ranking
as high as tier-0/1 venues since the frontend sort fell back to event
count alone.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
