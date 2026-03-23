# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T00:29:06Z
- **Source Commit**: [`c86fe753760b28c88875ca06658a9cc62b452798`](https://github.com/keunwoochoi/seoulunderground.live/commit/c86fe753760b28c88875ca06658a9cc62b452798)
- **Branch**: `feat/pr-c-performer-instruments`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23416261496)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: filter empty strings from instruments split; deduplicate EventMusicianSummary type

- export_static_json: filter empty strings after split/strip (review suggestion)
- App.tsx: import EventMusicianSummary from EventCard instead of duplicating the type

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
