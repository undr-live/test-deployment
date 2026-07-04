# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-07-04T13:31:54Z
- **Source Commit**: [`b3057056bdfef976d8c45f697c0b32783eee2ccf`](https://github.com/keunwoochoi/seoulunderground.live/commit/b3057056bdfef976d8c45f697c0b32783eee2ccf)
- **Branch**: `fix/verify-imgs-pages-deployment`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/28707747609)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: use Actions run conclusion in deploy-pages.yml verify; surface gh errors

The 2026-07-04 21:40 KST failure proved the legacy pages/builds API also
lies on the site repo: it stayed stuck at "building" after the failed
deployment, so the verify step's errored-triggered rebuild never fired
and it could only time out. Port the Actions-runs-API approach from
ig_deploy_images.sh, with the retry as an empty-commit push using the
deploy token (the POST /pages/builds rebuild was never exercised and the
builds API can't be trusted to report the state it keys on).

Also address review: stop redirecting gh api stderr to /dev/null in
ig_deploy_images.sh so real errors reach the job log.

Claude-Session: https://claude.ai/code/session_01XdCMM4Hosjw8jdzuJyUdyP

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
