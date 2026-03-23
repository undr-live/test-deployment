# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T00:05:29Z
- **Source Commit**: [`8c4815e2756dc7b545951dc7e18db255eccd201d`](https://github.com/keunwoochoi/seoulunderground.live/commit/8c4815e2756dc7b545951dc7e18db255eccd201d)
- **Branch**: `feat/pr-c-performer-instruments`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23415760044)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: show performer instruments in event cards

Add instruments field to musicians_inline in export_static_json.py so
per-musician instrument data flows through to the frontend. Update
EventMusicianSummary type in EventCard.tsx and App.tsx, and render
instruments in parentheses after each performer name in event cards.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
