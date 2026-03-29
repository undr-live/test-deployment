# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-29T06:32:41Z
- **Source Commit**: [`ad458ed695577ef028ebc81a87f9348da8155ef5`](https://github.com/keunwoochoi/seoulunderground.live/commit/ad458ed695577ef028ebc81a87f9348da8155ef5)
- **Branch**: `feat/musician-list-ui`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23703198099)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: refactor: address code review feedback on MusicianList

- Use shiftDate() for tomorrow calculation instead of manual date math
- Extract processMusicianData() as a standalone pure function (testable)
- Simplify filter: remove IIFE, compute needle once outside the boolean

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
