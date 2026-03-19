# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-19T04:56:48Z
- **Source Commit**: [`b7289729140e4c253c10eb7df8048dabe961a486`](https://github.com/keunwoochoi/seoulunderground.live/commit/b7289729140e4c253c10eb7df8048dabe961a486)
- **Branch**: `fix/stale-highlight-titles`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23280498649)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: perf: batch-fetch events and translations in export_highlights

Fixes N+1 query pattern: was doing 2 queries per highlight inside the
loop. Now fetches all events and translations in 2 queries total using
IN clauses.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
