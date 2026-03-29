# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-29T07:07:40Z
- **Source Commit**: [`1472e79cbef05e18f9b39cf5cb550dabfcc3e030`](https://github.com/keunwoochoi/seoulunderground.live/commit/1472e79cbef05e18f9b39cf5cb550dabfcc3e030)
- **Branch**: `feat/musician-connections`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23703796682)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: remove venue count badge from musician cards; fix venue nav on profile

- Remove "N venues" badge from musician list cards (was confusing)
- Venue links on musician profile now navigate to ?tab=venues&q=handle
  so the user lands on the venues tab with that venue pre-filtered,
  instead of the broken ?venue= param that showed all events

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
