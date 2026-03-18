# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-18T16:13:56Z
- **Source Commit**: [`1e0ea6e15e307233f26ea17b096576e8b558231e`](https://github.com/keunwoochoi/seoulunderground.live/commit/1e0ea6e15e307233f26ea17b096576e8b558231e)
- **Branch**: `fix/venue-context-loading`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23254763034)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: add warning logging to silent exception handlers

- extract_core.py: _parse_llm_json now logs warning + returns {} instead of {"raw": text}
- events_extract.py: log meta.json read failures and venue context load failures
- base_fetcher.py: log profile snapshot index.json load failures
- import_events.py: use EventMusician.model_validate() when extracting IG handles;
  log ValidationError as warning and fall back to raw dict access
- import_musicians.py: call enr.get("name") once, assign to variable before isinstance check
- build_connections.py: add type annotation for shared_venues JSON parse and validate
  the parsed value is a list before constructing a set

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
