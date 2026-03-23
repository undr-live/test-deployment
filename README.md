# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T04:12:18Z
- **Source Commit**: [`0b224bac0fe14652e09d0d1585c069ee82efa98b`](https://github.com/keunwoochoi/seoulunderground.live/commit/0b224bac0fe14652e09d0d1585c069ee82efa98b)
- **Branch**: `feat/pr-e-venue-map`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23421101142)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: venue map — SVG map with pins + Nominatim geocoding (PR E draft)

- etl/geocode_venues.py: batch-geocode venue addresses via Nominatim (free,
  no API key); 18/72 Seoul venues now have lat/lon
- VenueMap.tsx: pure SVG map — Seoul bounds, Han River polygon, neighborhood
  labels, venue pins from lat/lon; hover tooltip; click pin → switch to card
  view + scroll to venue
- MapPinIcon.tsx: new map pin SVG icon
- App.tsx: venuesViewMode extended to 'card' | 'table' | 'map'; map button
  in view toggle (venues tab only); venue cards get id for scroll-to
- i18n.ts: map_view key (en: Map, ko: 지도, de: Karte)

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
