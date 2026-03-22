# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-22T18:55:46Z
- **Source Commit**: [`700aa957855ed64e230752106c2d8aac55c98499`](https://github.com/keunwoochoi/seoulunderground.live/commit/700aa957855ed64e230752106c2d8aac55c98499)
- **Branch**: `feat/pr-a-filter-pills-group-by`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23410100082)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: auto-switch to card view when group-by-venue is selected

In table view clicking 공연장별 set the URL param but the venue-grouped
render was gated behind viewMode === 'card', so nothing changed visually.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
