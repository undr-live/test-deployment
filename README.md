# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T04:39:59Z
- **Source Commit**: [`9622e58daaac33cc7a6f7d84c3f2bf18ecace56e`](https://github.com/keunwoochoi/seoulunderground.live/commit/9622e58daaac33cc7a6f7d84c3f2bf18ecace56e)
- **Branch**: `feat/pr-e-venue-map`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23421728208)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix(pr-e): replace hand-drawn SVG map with Leaflet + OSM tiles

- Rewrites VenueMap to use Leaflet.js with OpenStreetMap tiles
  (free, no API key, proper rendered map with zoom/pan)
- Fixes type mismatch: Venue.ig_handle is now optional to match App.tsx
- Removes unused pts() function
- Fixes onVenueClick scroll bug: strip leading @ from handle
- Fixes onVenueClick timing: useEffect + venueToScrollTo state instead of setTimeout
- Fixes preferences.ts: getViewModePreference/saveViewModePreference now support 'map'
- Tightens geocode_venues.py exception handling to specific exception types

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
