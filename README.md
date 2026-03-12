# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-12T16:29:09Z
- **Source Commit**: [`2c9e6a887a331876862903a5027ee1336be10774`](https://github.com/keunwoochoi/seoulunderground.live/commit/2c9e6a887a331876862903a5027ee1336be10774)
- **Branch**: `eval-multi-model-dashboard`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23012555180)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: chore: clean up git tracking + add eval documentation

- Gitignore LOCAL_*.md (local working notes, never for commit)
- Gitignore evals/*/*/results/*/events/ and venues/ — per-case prediction
  files are regenerable with evals.run; only aggregate summaries committed
- Remove already-tracked LOCAL_*.md and 759 per-case JSON files from index
  (all files remain on disk)
- Add docs/EVALS.md: eval system architecture, directory layout, usage,
  metrics reference, and current model comparison results
- Whitelist docs/EVALS.md from the docs/*.md gitignore pattern

Made-with: Cursor

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
