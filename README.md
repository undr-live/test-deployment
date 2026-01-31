# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-01-31T17:44:29Z
- **Source Commit**: [`f7b373bb9f6cc513688a589b1a741446e5c4f624`](https://github.com/keunwoochoi/seoulunderground.live/commit/f7b373bb9f6cc513688a589b1a741446e5c4f624)
- **Branch**: `fix/cover-screenshot-alignment`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/21548366446)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: Fix cover screenshot alignment for center-crop

- Replace flexbox percentage sections with absolute centering technique
- Use transform: translate(-50%, -50%) for bulletproof centering
- Content now appears correctly in the center 1170px crop area
- Works for both non-highlighted days (genre title) and highlighted days (event card)
- Add test script for manual screenshot generation with date/highlight override
- Add App.tsx support for test_date and test_highlight URL parameters

Fixes the issue where date text was half trimmed off after the highlighted
shows feature was added (commit 2080775).

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
