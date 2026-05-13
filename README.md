# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-05-13T20:01:13Z
- **Source Commit**: [`aab1625c6d0e44b56a5de06e8585d7f49e91c409`](https://github.com/keunwoochoi/seoulunderground.live/commit/aab1625c6d0e44b56a5de06e8585d7f49e91c409)
- **Branch**: `fix/export-cutoff-timezone`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/25823191748)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: extend export cutoff to yesterday KST so today's events are always visible

The export was using midnight KST as the cutoff. Since the pipeline runs on
a machine in EDT, late-day KST events (stored as ~11:00 UTC) fall before the
midnight-KST cutoff and get dropped from the export. A user in any non-KST
timezone viewing 'today' would see 0 events for the current date.

Fix: subtract 1 day from the KST cutoff so yesterday (KST) events are always
included, covering all timezones.

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
