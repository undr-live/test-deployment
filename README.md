# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-26T22:07:55Z
- **Source Commit**: [`41c0975a7591ef45809c741e2f6abae5feab93da`](https://github.com/keunwoochoi/seoulunderground.live/commit/41c0975a7591ef45809c741e2f6abae5feab93da)
- **Branch**: `feat/filter-fixes-ga-tracking`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23620362307)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: collapsible search bar — icon-only by default, expands on click

- Default: shows magnifier icon only
- Click/tap: expands with animated width + border + placeholder text
- Click outside (with empty input): collapses back to icon
- Escape: clears query and collapses
- If URL has ?q=...: opens pre-expanded with query

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
