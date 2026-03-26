# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-26T21:54:12Z
- **Source Commit**: [`3ccb7d81adb84e260ac0f1474c18d66ebc026ddf`](https://github.com/keunwoochoi/seoulunderground.live/commit/3ccb7d81adb84e260ac0f1474c18d66ebc026ddf)
- **Branch**: `feat/filter-fixes-ga-tracking`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23619904011)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: update timezone tests for Mon-Sun week; add local test rule to CLAUDE.md

Tests were written for old Sun-Sat week definition. Updated to reflect
Mon-Sun week (Sunday = end of week) and added year-boundary case.

Also added rule to CLAUDE.md: run tests locally before pushing.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
