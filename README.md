# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-17T23:29:37Z
- **Source Commit**: [`ec3b9cc3b96d54c467c50a151957d42c87f77984`](https://github.com/keunwoochoi/seoulunderground.live/commit/ec3b9cc3b96d54c467c50a151957d42c87f77984)
- **Branch**: `fix/ig-story-highlight`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23221314870)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: title extraction, set labels, iCloud sync, and highlight URL params

- events_extract.py: store title_ko/title_en from v4.0.x LLM response
  instead of legacy title field (which was always null); fix has_musician
  check to use name_ko/name_en; fix is_title_empty to handle all schema variants
- screenshot_table_view.py: pass today_kst as arg to get_today_highlight
  instead of recalculating inside; refactor to avoid redundant date calc
- ig_story_notify.py: remove icloud_sync step and its Slack notification
- App.tsx: fix formatSets to return primary time only (no label) for time
  column and showTime comparison; add formatSetSchedule for labeled sets
- EventTableView.tsx: render setSchedule as secondary text below title

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
