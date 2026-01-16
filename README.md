# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-01-16T20:46:30Z
- **Source Commit**: [`00cd87cd7a1361ccf5f188f2903b4dcbc15333a6`](https://github.com/keunwoochoi/seoulunderground.live/commit/00cd87cd7a1361ccf5f188f2903b4dcbc15333a6)
- **Branch**: `cleaning98`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/21080351142)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: address code review issues

CRITICAL:
- Remove .env.bak with secrets from git (add *.bak and .env* to .gitignore)
- Fix bash syntax error: else: → else in upload_post_job.sh

Medium:
- Handle bytes in subprocess_utils.py (decode before logging)
- Remove stderr suppression in deploy_daily_images.sh for better debugging
- Fix sync_venue_manual_info.py to use proper JSONL format (line-by-line)

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
