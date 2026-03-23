# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T05:21:26Z
- **Source Commit**: [`937f58e8dc1ca06ef5143facb9653791029a89f5`](https://github.com/keunwoochoi/seoulunderground.live/commit/937f58e8dc1ca06ef5143facb9653791029a89f5)
- **Branch**: `feat/pr-e-venue-map`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23422668085)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat(map): map as overlay toggle + geocoder floor-prefix fix

Map is now an independent toggle above the venue list (card/table always
visible below). Clicking the pin icon in the toolbar shows/hides the map;
the card/table view mode is unaffected.

Removes 'map' from venuesViewMode type — back to 'card' | 'table'.

Also fixes geocode_venues.py: retries with floor/basement prefix stripped
("B1, ", "2F, ", "3층, ") when the first Nominatim attempt fails.
Geocoded oleojazzpub and teddy.valley as a result.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
