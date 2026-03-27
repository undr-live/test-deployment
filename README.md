# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-27T12:44:32Z
- **Source Commit**: [`08e0c6533892d1a9ac451b88bd3cd70602ed7e41`](https://github.com/keunwoochoi/seoulunderground.live/commit/08e0c6533892d1a9ac451b88bd3cd70602ed7e41)
- **Branch**: `feat/musician-highlight-slack-frontend`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23646784409)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: address code review on musician highlight PR

- routers.py: move global config import to module level (import config as
  global_config), narrow exception to JSONDecodeError + Exception
- export_static_json.py: narrow exception to JSONDecodeError + Exception
- App.tsx: log console.warn on musician highlight load failure
- FeaturedMusician.tsx: extract getDisplayName() helper for clarity

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
