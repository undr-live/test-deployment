# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-22T01:12:52Z
- **Source Commit**: [`3d03b7b2bb218b3ceb7c8d274cb25d30ef2698b5`](https://github.com/keunwoochoi/seoulunderground.live/commit/3d03b7b2bb218b3ceb7c8d274cb25d30ef2698b5)
- **Branch**: `chore/cleanup-actions-temp-dirs`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23392790210)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: chore: move actions-gh-pages temp dirs to ~/github_actions after each deploy

peaceiris/actions-gh-pages creates actions_github_pages_* dirs in $HOME
with no config option to change the location. This step moves them to
~/github_actions/ after every deploy run (even on failure).

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
