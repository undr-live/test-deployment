# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-30T00:11:13Z
- **Source Commit**: [`cebd3f70c8d6affbe38ee1d5319bad1b0ae61e05`](https://github.com/keunwoochoi/seoulunderground.live/commit/cebd3f70c8d6affbe38ee1d5319bad1b0ae61e05)
- **Branch**: `feat/musician-fetch-links`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23722417350)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: refactor: links.json cache + code review fixes

- links.json per musician replaces linktree_resolved.json:
  structured with {updated_at, links: [{kind, url, source, via?}],
  linktree_fetched_at: {url: timestamp}}
- Fix N+1: batch-fetch all existing YouTube Link rows before musician loop
- export_static_json: select only (entity_id, url) columns from Link table
- Specific exceptions: json.JSONDecodeError/OSError/RequestException
  instead of broad Exception
- dict.fromkeys() for deduplication in _fetch_linktree_youtube_urls

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
