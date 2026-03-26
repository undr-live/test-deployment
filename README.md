# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-26T05:10:38Z
- **Source Commit**: [`686c4c969b0eb95440722b1436e3a89dd4f4216e`](https://github.com/keunwoochoi/seoulunderground.live/commit/686c4c969b0eb95440722b1436e3a89dd4f4216e)
- **Branch**: `fix/seo-germany-disable-lang-routes`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23578584935)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: disable germany/jazz and create static files for Seoul lang routes

- config.py: set germany-jazz enabled=False so it's excluded from
  sitemap, JSON export, and SEO page generation
- deploy-pages.yml: after Vite build, copy dist/index.html to each
  /{locality}/{genre}/{lang}/index.html so GitHub Pages returns 200
  instead of 404 for SPA language routes that Google is trying to index

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
