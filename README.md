# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-21T23:52:37Z
- **Source Commit**: [`5c349a1ffdacec343c4de960e30067d2a1bd7381`](https://github.com/keunwoochoi/seoulunderground.live/commit/5c349a1ffdacec343c4de960e30067d2a1bd7381)
- **Branch**: `feat/seo-llm-optimization`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23391547375)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: address code review on JSON-LD structured data

- Fix performer name: was using m.name (doesn't exist); now uses
  getI18nValueWithFallback(name_ko/name_en) || name_irl || ig_handle
- Fix SearchAction target and MusicEvent url fallback: were hardcoded to
  /seoul/jazz/ko; now use locality/genre/lang route variables
- Fix addressLocality/addressCountry: were hardcoded to 서울/KR; now derive
  from LOCALITY_GEO map in locality.ts (seoul→서울/KR, germany→Germany/DE)
- Sync canonical and og:url to current route in same useEffect
  (was hardcoded to root in index.html, wrong for /seoul/jazz/en etc.)
- Add LOCALITY_GEO to locality.ts dependency array

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
