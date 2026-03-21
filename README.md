# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-21T17:20:12Z
- **Source Commit**: [`662cba241094eee1ce26828dc9caba098a3f6c5d`](https://github.com/keunwoochoi/seoulunderground.live/commit/662cba241094eee1ce26828dc9caba098a3f6c5d)
- **Branch**: `fix/screenshot-footer-visibility`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23384709343)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: ensure Instagram footer is always visible in screenshot pages

Rows with 1부/2부 set schedules are taller than single-set rows,
pushing the footer below the viewport crop window. Fix:

1. Add data-ig-footer attribute to InstagramFooter for reliable
   Playwright targeting.
2. Before taking screenshots, probe page 1 and measure whether the
   footer is within the viewport. If clipped, reduce epp by 1 and
   re-probe until it fits (min epp: 5).

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
