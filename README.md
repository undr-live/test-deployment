# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-21T21:39:07Z
- **Source Commit**: [`429d3e555dce624f757a4de4e5b7cfbe77e11862`](https://github.com/keunwoochoi/seoulunderground.live/commit/429d3e555dce624f757a4de4e5b7cfbe77e11862)
- **Branch**: `feat/seo-llm-optimization`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23389358066)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: SEO and LLM optimization — meta tags, structured data, GA4 update

- Update GA4 measurement ID to G-6T1KPG2K45 (new undr.live stream)
- Add descriptive <title>, <meta description>, Open Graph, Twitter Card tags
- Set lang="ko" (site is Korean-first)
- Add canonical URL
- Add robots.txt (allow all, sitemap reference)
- Add sitemap.xml with hreflang alternates for ko/en
- Inject dynamic JSON-LD structured data (schema.org WebSite + MusicEvent)
  so search engines and LLMs can cite individual upcoming events
- Fix 404.html title (was "Seoul Underground Live")

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
