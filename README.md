# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-05-13T20:18:27Z
- **Source Commit**: [`3c1dccf5097c42d49b53a60884e1cf397efd890b`](https://github.com/keunwoochoi/seoulunderground.live/commit/3c1dccf5097c42d49b53a60884e1cf397efd890b)
- **Branch**: `fix/export-cutoff-timezone`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/25824058411)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: always switch to keunwoochoi account before gh workflow trigger

Multiple gh accounts are configured. The active account drifted to
keunwoo-ortet, causing `gh workflow run` to return 404 and silently
breaking all deploys for ~2 weeks (May 9–13). The auth status check
passes for any authenticated account, so it didn't catch the wrong account.

Switch explicitly to keunwoochoi and treat failure as fatal (exit 1) so
a bad account state aborts loudly rather than silently deploying to the
wrong place.

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
