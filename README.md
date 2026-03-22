# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-22T03:43:06Z
- **Source Commit**: [`913be3ad1637a21cf19ace655dd4252afee38ab0`](https://github.com/keunwoochoi/seoulunderground.live/commit/913be3ad1637a21cf19ace655dd4252afee38ab0)
- **Branch**: `refactor/remove-hardcoded-paths`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23395010848)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: address code review on install.sh and sitemap

- install.sh: fix argument parsing — was using positional $1 so
  --project-dir flag was assigned literally as the path. Now parses
  --project-dir <value> correctly with an error if value is missing.
- generate_seo_pages.py: add generate_sitemap() — rewrites sitemap.xml
  automatically from enabled LOCALITY_GENRE_REGISTRY entries, including
  all app routes (with hreflang), events.html, and digest pages per locality.
  Sitemap is now always in sync with config; no manual edits needed.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
