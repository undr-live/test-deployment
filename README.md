# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-21T22:01:17Z
- **Source Commit**: [`2e994b3601941a8aec269efbd42fed941b1383be`](https://github.com/keunwoochoi/seoulunderground.live/commit/2e994b3601941a8aec269efbd42fed941b1383be)
- **Branch**: `feat/seo-llm-optimization`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23389734755)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: static HTML pages for SEO crawlability + Naver/Google SC prep

- generate_seo_pages.py: generates events.html (full listing) and
  digest/YYYY-MM-DD/index.html (weekly digest) from exported JSON.
  Both are plain HTML — readable by Naver Yeti and other non-JS crawlers.
  Hooked into deploy workflow after JSON export, before npm build.
- sitemap.xml: add events.html entry
- index.html: add commented placeholders for Google SC + Naver verification
  meta tags (fill in after registering properties)
- Ship current week's events.html and digest page with this commit

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
