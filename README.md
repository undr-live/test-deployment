# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T05:12:39Z
- **Source Commit**: [`06c395a97bdd7ece668e64712848105877339326`](https://github.com/keunwoochoi/seoulunderground.live/commit/06c395a97bdd7ece668e64712848105877339326)
- **Branch**: `feat/pr-e-venue-map`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23422488172)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix(map): markers missing on page refresh + address localization

Split single map useEffect into two:
- Effect 1: map init + tile layer (deps: [lang])
- Effect 2: marker management (deps: [venues, lang])

Effect 1 ran at mount with empty venues; Effect 2 now correctly fires
when the async venues API response arrives, adding all markers.

Address in the popup panel already uses i18n_data.address_text[lang]
with location_text fallback — confirmed correct for all languages.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
