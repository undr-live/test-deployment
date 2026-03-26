# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-26T22:18:40Z
- **Source Commit**: [`5f21d88b1d9a1f0258427b47a18f92728b6efa6a`](https://github.com/keunwoochoi/seoulunderground.live/commit/5f21d88b1d9a1f0258427b47a18f92728b6efa6a)
- **Branch**: `feat/filter-fixes-ga-tracking`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23620808160)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: smooth search bar animation, stable height, no focus ring

- Input always in DOM; width 26→200 via cubic-bezier transition (no pop-in)
- Input fades in via opacity transition, slightly delayed after width starts
- Fixed height 26px matches button group — zero layout shift when opening
- Removed border from active state; background change alone signals active
- outline:none + border:none on input removes browser focus ring (the reddish glow)
- tabIndex=-1 when closed to prevent accidental keyboard focus

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
