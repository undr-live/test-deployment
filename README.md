# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-07-04T03:54:44Z
- **Source Commit**: [`2a58ad89b54dec848c7d77b42620f072bf9fa16f`](https://github.com/keunwoochoi/seoulunderground.live/commit/2a58ad89b54dec848c7d77b42620f072bf9fa16f)
- **Branch**: `fix/verify-pages-deployment`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/28694129043)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: verify GitHub Pages deployment after push to external repo

The deploy workflow considered its job done once the push to
undr-live/undr-live.github.io landed, but the actual Pages deployment
runs as GitHub's automatic "pages build and deployment" workflow in the
external repo. On 2026-07-03 12:08 UTC that build failed transiently
("Page build failed" / "Deployment failed, try again later") while every
workflow here stayed green — the site served stale data for ~3h with no
alert, and nothing retried.

Add a post-push verification step that polls the Pages builds API until
the build for our commit completes, requests one rebuild on failure, and
fails the workflow loudly if it still fails — which triggers the existing
slack-notify.yml deployment-failure alert.

Claude-Session: https://claude.ai/code/session_01XdCMM4Hosjw8jdzuJyUdyP

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
