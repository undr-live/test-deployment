# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-02-14T15:54:55Z
- **Source Commit**: [`0cde41d81393526adbb197702087912064b7f8fa`](https://github.com/keunwoochoi/seoulunderground.live/commit/0cde41d81393526adbb197702087912064b7f8fa)
- **Branch**: `feat/dynamic-events-per-page`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/22020178606)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: Dynamic events per page (7 or 8) with cascading trim logic

- Auto-select 7 events/page when ≤63 events, 8 when >63 (max 72)
- Add cascading trim when >72 events: drop no-datetime → dedupe venues → truncate tail
- Support epp URL param override for explicit control
- Compact InstagramFooter padding when epp=8
- Match Python screenshot pipeline to pass epp param to frontend

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
