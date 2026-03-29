# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-29T22:31:05Z
- **Source Commit**: [`b3b106800fc230f34daf3a743eea0725297470ce`](https://github.com/keunwoochoi/seoulunderground.live/commit/b3b106800fc230f34daf3a743eea0725297470ce)
- **Branch**: `feat/musician-fetch-links`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23720642346)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: extract YouTube channel links from musician bios (step 5c)

- New etl/musicians/fetch_links.py: reads biography_links from
  profile/latest.json, extracts YouTube channel URLs (not video URLs),
  resolves Linktree pages via HTTP GET with 30-day disk cache,
  writes results to Link table
- export_static_json.py: export_musicians() now reads Link table to
  populate websites field (was always empty before)
- musician_job.sh: add step 5c after extract_instruments

Result: 131 of 814 seoul/jazz musicians now have YouTube channel links
in the exported JSON, rendered as "YouTube" cards in the 링크 section.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
