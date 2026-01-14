# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-01-14T15:27:34Z
- **Source Commit**: [`2ac8a122ecae523d1de0d7e0d971a86895156963`](https://github.com/keunwoochoi/seoulunderground.live/commit/2ac8a122ecae523d1de0d7e0d971a86895156963)
- **Branch**: `k/seoul-jazz-only`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/20999641234)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: Focus on Seoul/jazz only: disable Germany/jazz ETL and frontend

- Comment out Germany/jazz sections in event_job.sh and venue_job.sh
- Remove 'germany' from SUPPORTED_LOCALITIES in frontend
- Keep all Germany data and code intact for future reactivation
- Immediate cost savings by stopping Germany ETL pipeline

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
