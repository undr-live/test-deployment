# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-27T20:09:19Z
- **Source Commit**: [`c3620b212e6635c30fb7a7ba792484155e2a9662`](https://github.com/keunwoochoi/seoulunderground.live/commit/c3620b212e6635c30fb7a7ba792484155e2a9662)
- **Branch**: `fix/map-cleaner-tiles-subway`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23665384821)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: switch map to CartoDB Voyager for all languages

Replaces noisy OSM standard tiles (used for Korean) with CartoDB Voyager
across all languages. Voyager shows Seoul subway lines natively, has
Korean labels, and is visually much cleaner. Map no longer reinitializes
on language switch since tiles are now language-independent.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
