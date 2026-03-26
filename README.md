# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-26T23:27:13Z
- **Source Commit**: [`4f513c708eb06a8f5ef2c6052f6a6c15936b8cf8`](https://github.com/keunwoochoi/seoulunderground.live/commit/4f513c708eb06a8f5ef2c6052f6a6c15936b8cf8)
- **Branch**: `fix/unknown-event-time`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23623079898)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: unknown event time — display '—', retry image fetch, safer delays

ETL:
- Retry image fetch for posts saved without images (files=None): on next
  run, posts with metadata but no files will re-attempt web.post() detail
  fetch instead of being skipped — auto-backfill once session is restored
- Add DOWNLOAD_DELAY pause before web.post() detail fetch (was missing)
- Bump post delay default 1-3s → 2-5s; download delay 0.5-1.5s → 1.5-3.5s

Frontend:
- formatSets() now returns null when no set time is known (was falling
  back to datetime field, which is midnight sentinel — not a real time)
- EventCard and EventTableView show '—' when displayTime is null,
  instead of the raw ISO datetime string or a misleading "12:00 AM"

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
