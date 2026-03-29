# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-29T06:27:12Z
- **Source Commit**: [`6e9a7fa147f25cc0b30957f432ca419598b74750`](https://github.com/keunwoochoi/seoulunderground.live/commit/6e9a7fa147f25cc0b30957f432ca419598b74750)
- **Branch**: `feat/musician-list-ui`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23703115851)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: musician list 2D grid with upcoming show info and filters

- Replace 1-column list with responsive 2-column grid (minmax 160px)
- Remove confidence score display
- Add instrument filter chips (composer, piano, bass, vocals, drums, sax, guitar)
- Add "playing soon" toggle to filter to musicians with upcoming shows
- Show next show date/time/venue on each card (e.g. "● 오늘 8pm · Oleo Jazz Pub")
- Sort: upcoming-first by soonest show, then completeness, show count, alpha
- Mute @handle to text-secondary; all labels i18n'd

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
