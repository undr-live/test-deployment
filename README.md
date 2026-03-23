# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T04:51:23Z
- **Source Commit**: [`8aae3f99bf6d5568c6b1fc56aedac7e9a7b06c4e`](https://github.com/keunwoochoi/seoulunderground.live/commit/8aae3f99bf6d5568c6b1fc56aedac7e9a7b06c4e)
- **Branch**: `feat/pr-e-venue-map`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23421995062)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat(map): standout pins, in-map popup panel, language-specific tiles

- Pins: changed to bright orange-red (#e85d26) for high visibility
- Click behavior: clicking a pin shows an inline popup panel on the map
  (name, address, subway, IG link, Google Maps link) — no longer navigates
  to venue card
- Language-specific tiles: ko → OSM standard (Korean labels); en/de → Carto
  Voyager (Latin-script labels)
- Popup panel localized via t(lang, key)
- Removes onVenueClick prop and venueToScrollTo state (no longer needed)

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
