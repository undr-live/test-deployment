# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-07-05T18:17:46Z
- **Source Commit**: [`6b02fad23f18d5d26ea3e29e9074677b84ca5e25`](https://github.com/keunwoochoi/seoulunderground.live/commit/6b02fad23f18d5d26ea3e29e9074677b84ca5e25)
- **Branch**: `fix/verify-live-site-stamp`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/28750327414)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: verify deploys against the live site, not GitHub build metadata

Two deploy failures on 2026-07-05 (10:14Z, 13:24Z) got past the
3x-backoff retry from #180: GitHub ran the Pages build against the
PREVIOUS head after our push, so no run ever existed for our SHA — the
verify polled run conclusions, found nothing completed, and waited
passively to its deadline while the site served one-cycle-stale data.

Verify v2 uses ground truth instead of build metadata:
- deploy-pages.yml: success = undr.live/README.md serves THIS workflow
  run's ID (cache-busted; retry commits are empty so the stamp
  survives). Actions conclusions only trigger retries; 420s with no
  confirmation also triggers a retry nudge — covering stuck, skipped,
  and wrong-head builds. Deadline 1500s -> 2400s to fit stall windows.
- ig_deploy_images.sh: success = today's first image URL returns 200
  (the date folder only exists in this deploy); same retry/stall logic.

Also: rename scripts/test_slack_notifications.py ->
scripts/slack_notifications_smoke.py. It is a manual smoke script that
sends REAL webhook messages, but its test_* names meant pytest
collected and executed it — the 2026-07-05 01:35 EST fake 'Weekly:
jazz' and 'ETL Pipeline ConnectionError' Slack alerts were its
fixtures firing during a full-suite run. scripts/ now collects zero
tests.

Claude-Session: https://claude.ai/code/session_015v4p2qKzNBshy1FMKt6KYM

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
