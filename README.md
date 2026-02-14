# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-02-14T17:14:39Z
- **Source Commit**: [`c35666027725fe6c43ee30373140e2874ac8c33e`](https://github.com/keunwoochoi/seoulunderground.live/commit/c35666027725fe6c43ee30373140e2874ac8c33e)
- **Branch**: `feat/dynamic-events-per-page`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/22021220809)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: refactor: Address code review - named constants + simplify trim loop

- Extract EVENTS_PER_PAGE_STANDARD=7, EVENTS_PER_PAGE_COMPACT=8 in Python
- Extract EPP_STANDARD=7, EPP_COMPACT=8, MAX_CONTENT_PAGES=9 in TypeScript
- Simplify busiest-venue removal using findLastIndex + Object.keys().find()

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
