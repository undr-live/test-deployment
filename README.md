# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-30T13:12:23Z
- **Source Commit**: [`8adda9f0013ea7b0697c4a2f41637697745eb82d`](https://github.com/keunwoochoi/seoulunderground.live/commit/8adda9f0013ea7b0697c4a2f41637697745eb82d)
- **Branch**: `fix/jsonld-offers-fields`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23746468737)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: refactor: remove redundant isNaN check in parsePriceKRW

match[0] is always a digit string when match is non-null.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
