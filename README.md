# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-02-03T04:23:35Z
- **Source Commit**: [`b1d13d1711a264518df36621ad90a60dfda3f2a3`](https://github.com/keunwoochoi/seoulunderground.live/commit/b1d13d1711a264518df36621ad90a60dfda3f2a3)
- **Branch**: `fix/cover-date-color-kst`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/21616898917)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: Use UTC-based weekday calculation for cover date color

The previous implementation used .getDay() which returns the weekday
in the local timezone of the machine running the code. This caused
incorrect coloring when the GitHub Actions runner is in a different
timezone than KST - e.g., Monday in KST was being colored red (Sunday)
because the runner's local time was still Sunday.

Fix: Use .getUTCDay() with a UTC-based timestamp to ensure we get the
weekday for the actual calendar date regardless of local timezone.

Color scheme (unchanged):
- Sunday: red (#FF6B9D)
- Saturday: blue (#6BB6FF)
- Friday: gold (#FFD700)
- Weekdays: white (#fff)

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
