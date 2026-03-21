# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-21T21:10:25Z
- **Source Commit**: [`de823bfee5ad9eabad4c9cb2599bd729029ac469`](https://github.com/keunwoochoi/seoulunderground.live/commit/de823bfee5ad9eabad4c9cb2599bd729029ac469)
- **Branch**: `fix/screenshot-footer-visibility`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23388864404)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: per-page adaptive event count to keep footer visible in screenshots

Each story page now independently probes from 7 down to 3 events to find
the maximum count that keeps the @undr.live footer within the 593px crop
boundary. This preserves 1부/2부 set detail while ensuring the footer is
never clipped, regardless of row height variation across pages.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
