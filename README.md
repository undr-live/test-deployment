# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-01-31T06:40:53Z
- **Source Commit**: [`63ce0fa8a27e1a80cec3ed64c98c3d10f6d64bbb`](https://github.com/keunwoochoi/seoulunderground.live/commit/63ce0fa8a27e1a80cec3ed64c98c3d10f6d64bbb)
- **Branch**: `k/refactor-frontend`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/21540387610)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: Add padding to cover overlay top section to prevent date text crop

- Added paddingTop: '60px' to top section in EnhancedCoverOverlay.tsx
- Fixes issue where date text '01-31 (토)' was cut off at top
- Applies to cover page (scr_idx=0) when no highlighted event
- Tested with production screenshots - date now fully visible

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
