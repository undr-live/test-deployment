# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T05:32:48Z
- **Source Commit**: [`dcfb3ebce1ab37566eb252231911e57b71cdb387`](https://github.com/keunwoochoi/seoulunderground.live/commit/dcfb3ebce1ab37566eb252231911e57b71cdb387)
- **Branch**: `feat/pr-e-venue-map`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23422945586)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix(map): use VenueMaster locations[0] coords for venues missing lat/lon

39 of 72 masters have lat/lon in locations[0] that were being ignored.
Adds venuesForMap memo that merges master coordinates + i18n address text
into filteredVenues before passing to VenueMap, bringing mapped count
from ~18 to ~39.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
