# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-26T21:43:48Z
- **Source Commit**: [`8ffd7f2d338a4911771c224e288647173373a275`](https://github.com/keunwoochoi/seoulunderground.live/commit/8ffd7f2d338a4911771c224e288647173373a275)
- **Branch**: `feat/filter-fixes-ga-tracking`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23619511732)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: filter fixes, layout swap, GA tracking

- Fix 'this week'/'next week' overlap: endOfWeekFrom now ends on Sunday (Mon–Sun week)
- Fix 'all' filter URL param: encode as all=1 so urlParamsToFilter can distinguish it from default
- Fix GA ID: was G-3E3NPW57WD, now matches index.html (G-6T1KPG2K45)
- Move view/map toggle buttons left of search bar
- Add trackEvent helper and GA4 event tracking on: filter pills, group-by toggle, view mode buttons, search

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
