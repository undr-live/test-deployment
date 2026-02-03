# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-02-03T04:27:49Z
- **Source Commit**: [`6bb602091079cd63ee9a617ef1342a8c5124dddf`](https://github.com/keunwoochoi/seoulunderground.live/commit/6bb602091079cd63ee9a617ef1342a8c5124dddf)
- **Branch**: `fix/cover-date-string-utc`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/21616986425)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: Use UTC-based dateStr for cover overlay

Apply the same timezone-agnostic technique to dateStr creation.
The previous implementation had:
- Hardcoded -05:00 for America/New_York (incorrect during DST)
- Only handled America/New_York, defaulting to +09:00 for all else

Since formatDateHeader already takes the timezone parameter and handles
conversion internally, we can simply pass a UTC timestamp.

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
