# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-02T04:08:00Z
- **Source Commit**: [`35aa98478a91485c5a864572b46432a8a18d1ec7`](https://github.com/keunwoochoi/seoulunderground.live/commit/35aa98478a91485c5a864572b46432a8a18d1ec7)
- **Branch**: `feat/tier-based-venue-sampling`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/22560973622)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: Remove venue_handles.csv from git tracking

The CSV file should remain local-only (like venue_handles.txt) and not be
tracked in git. This prevents triggering the deployment workflow on PRs.

Made-with: Cursor

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
