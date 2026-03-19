# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-19T04:54:14Z
- **Source Commit**: [`7fdff4441f1af2658bec3fe079bdc0c4301569b5`](https://github.com/keunwoochoi/seoulunderground.live/commit/7fdff4441f1af2658bec3fe079bdc0c4301569b5)
- **Branch**: `fix/stale-highlight-titles`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23280437211)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: refresh highlight titles from DB on export to prevent stale cache

weekly_highlights.json caches event titles at selection time (Monday).
When the ETL later corrects an event, the cached title goes stale and
the wrong title shows up in the screenshot cover.

export_highlights() now re-fetches title/translations from the DB for
each event_id before writing to frontend/public/api/highlights.json,
so the exported file always reflects the current DB state.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
