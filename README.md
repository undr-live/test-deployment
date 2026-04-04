# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-04-04T03:06:34Z
- **Source Commit**: [`1d07c31f0f0ba4ac75f23d9e16b61c5280028ada`](https://github.com/keunwoochoi/seoulunderground.live/commit/1d07c31f0f0ba4ac75f23d9e16b61c5280028ada)
- **Branch**: `fix/highlight-wider-pool`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23970023548)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: widen highlight pool — top_n 15→25, time window 18:00-22:00→23:00

7 eligible venues → 9 eligible venues for this week.
Tier-based weighted sampling already handles prioritization;
the hard top-15 cutoff was unnecessarily squeezing the pool.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
