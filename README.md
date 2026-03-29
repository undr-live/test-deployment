# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-29T06:56:23Z
- **Source Commit**: [`86b29bb0ad83051d8769d0dd2cc1c41f2acd7d52`](https://github.com/keunwoochoi/seoulunderground.live/commit/86b29bb0ad83051d8769d0dd2cc1c41f2acd7d52)
- **Branch**: `feat/musician-connections`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23703617408)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: musician connection export + profile sections (phase 2)

- export_static_json.py: add export_musician_connections() — top-5 venues
  and top-5 co-musicians per musician written to connections.json; call it
  in run_export_static_json() for each locality/genre
- App.tsx: add MusicianConnections type; add /api/connections static route
- MusicianList: fetch connections; show venue count badge on each card
- MusicianProfile: fetch connections; add "Venues" section (top venues,
  clickable → events tab filtered by venue) and "Musicians" section
  (top co-musicians, clickable → their profile); fix hardcoded Back button
  to use t(lang, 'back') and navigate back to /musicians list

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
