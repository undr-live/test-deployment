# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-02-05T04:57:42Z
- **Source Commit**: [`43da4528e5c0ebaf764173c45c515c96b263e063`](https://github.com/keunwoochoi/seoulunderground.live/commit/43da4528e5c0ebaf764173c45c515c96b263e063)
- **Branch**: `fix/highlights-static-export`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/21699391128)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: Export highlights to static JSON for GitHub Pages

Two issues were preventing highlighted events from showing:

1. Missing weekly_job.sh - the launchd plist referenced this file but
   it didn't exist, so highlight selection never ran on Mondays

2. Highlights not exported to static JSON - frontend in static mode
   (GitHub Pages) couldn't fetch highlights because:
   - export_static_json.py didn't include highlights
   - App.tsx api() function didn't handle /api/highlights path

Fixes:
- Add weekly_job.sh that runs highlight_job.sh on Mondays
- Add export_highlights() to export weekly_highlights.json
- Add /api/highlights routing in static mode frontend

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
