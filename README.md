# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-18T22:09:05Z
- **Source Commit**: [`8c8cce39baf85d300552378f07577d58de27a532`](https://github.com/keunwoochoi/seoulunderground.live/commit/8c8cce39baf85d300552378f07577d58de27a532)
- **Branch**: `fix/venue-context-loading`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23269483420)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: full ETL pipeline audit — subgenres, sets crash, age_limit, and schema gaps

- Add genres column to Event DB model + SQLite migration for subgenres data
- EventData.genres field maps LLM subgenres through import → DB → export
- import_events: extract ann['subgenres'] → EventData.genres; use _pick_bilingual
  for age_limit (was silently dropped when stored as {en, ko} dict)
- export_static_json: add genres to event export; replace bare json.loads(sets)
  with safe _parse_sets() helper (was an unhandled crash path)
- crud._to_event_schema: add genres field; replace bare json.loads(obj.sets) with
  safe _parse_sets_json() helper (same crash risk in API path)
- schemas.EventBase: add genres field
- CLAUDE.md: add working philosophy — fix the pipeline not the data; trace the
  full data path; full automation is the goal

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
