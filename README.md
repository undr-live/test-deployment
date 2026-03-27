# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-27T12:55:22Z
- **Source Commit**: [`cdaf173ef6baa2a2abe2eb5cbba4c2f993faeec4`](https://github.com/keunwoochoi/seoulunderground.live/commit/cdaf173ef6baa2a2abe2eb5cbba4c2f993faeec4)
- **Branch**: `feat/musician-highlight-slack-frontend`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23647194373)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: revert: remove premature musician highlight frontend feature

Remove API endpoint, static export, FeaturedMusician component, App.tsx
wiring, i18n keys, and MusicianHighlight type. Keep only the Slack
notification (send_musician_highlight) added in this branch.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
