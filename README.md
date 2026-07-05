# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-07-05T05:30:13Z
- **Source Commit**: [`bd7ca74c2b6b7f654eb8590e05458c51738d91ce`](https://github.com/keunwoochoi/seoulunderground.live/commit/bd7ca74c2b6b7f654eb8590e05458c51738d91ce)
- **Branch**: `fix/pages-deploy-retry-backoff`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/28730736009)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: retry Pages deploy verification up to 3x with backoff

GitHub Pages deployments on both external repos have failed daily since
2026-07-03 with the transient "Deployment failed, try again later"
(site repo: 07-03 12:08Z, 07-04 12:40Z, 07-05 01:09Z; images repo:
02:2xZ on all three days). A GitHub Pages incident on 07-02 preceded
the streak; flakiness has stayed elevated since.

The single-retry logic from #178/#179 fires ~3s after detecting the
failure, so on 07-05 both the original attempt and the retry landed
inside the same blip window and the site deploy failed outright. The
evidence says short waits win: the images repo's retry ~1 min later
succeeded on both 07-04 and 07-05.

Retry up to 3 times with escalating waits (60/120/180s) in both the
deploy-pages.yml verify step and ig_deploy_images.sh, and extend the
polling deadline from 600s to 1500s to fit the extra attempts. Failure
after the last retry still exits 1 loudly (slack-notify.yml alert /
ig_story_job.sh abort).

Claude-Session: https://claude.ai/code/session_015v4p2qKzNBshy1FMKt6KYM

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
