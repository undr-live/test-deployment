# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-12T02:08:38Z
- **Source Commit**: [`510fdb9dad4bf16019a1467fff37b65e8ba41109`](https://github.com/keunwoochoi/seoulunderground.live/commit/510fdb9dad4bf16019a1467fff37b65e8ba41109)
- **Branch**: `feat/event-schema-v2-and-evals`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/22983401180)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: move golden dataset from data/golden/ to evals/golden/

The deploy workflow creates a symlink: ln -s .../data ./data
With data/golden/ tracked in git, checkout materializes data/ as a real
directory before ln -s runs, placing the symlink at data/data/ instead.
This broke the DB path (data/app.db not found).

Moving to evals/golden/ keeps the dataset clear of the symlink.
Also update .gitattributes LFS pattern and all path references.

Made-with: Cursor

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
