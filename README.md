# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-01-31T06:47:42Z
- **Source Commit**: [`0a5dce9cef3b64d606b979a9ccbae23dde143866`](https://github.com/keunwoochoi/seoulunderground.live/commit/0a5dce9cef3b64d606b979a9ccbae23dde143866)
- **Branch**: `k/refactor-frontend`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/21540477103)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: Adjust flex proportions in cover overlay to prevent date text crop

- Changed top section from 30% to 40% height
- Changed middle section from 60% to 50% height
- Removed paddingTop hack (was pushing content too low)
- Date '01-31 (토)' now fully visible in center-cropped 1170x1170 output
- Tested with local build screenshot generation

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
