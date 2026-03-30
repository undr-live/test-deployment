# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-30T13:09:24Z
- **Source Commit**: [`767af7a835ec99d72577c5777b5b48ba7d99ccd4`](https://github.com/keunwoochoi/seoulunderground.live/commit/767af7a835ec99d72577c5777b5b48ba7d99ccd4)
- **Branch**: `fix/jsonld-offers-fields`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23746346546)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: add missing JSON-LD offers fields for Google Search Console

Fixes 5 structured data warnings:
- price: parse free-text KRW string to number (e.g. "20,000원" → 20000; "무료" → 0)
- priceCurrency: always "KRW" (was omitted when no price)
- availability: always InStock
- validFrom: event startDate
- Remove conditional offers — always emit all fields

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
