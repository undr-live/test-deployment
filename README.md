# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-22T18:20:31Z
- **Source Commit**: [`8cb61e7cf7e27c1a8a09327991364b0a1fa0d4d2`](https://github.com/keunwoochoi/seoulunderground.live/commit/8cb61e7cf7e27c1a8a09327991364b0a1fa0d4d2)
- **Branch**: `feat/pr-a-filter-pills-group-by`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23409442386)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: human-readable filter pills, group-by toggle, fix musician_ig_handles crash

- Replace D+0/D+1/W+0/W+1 pills with Today/Tomorrow/This week/Next week labels
- Add group-by toggle (date ↔ venue) in card view, URL param ?group=venue
- Two-row filter bar: pills on row 1, group-by right-aligned on row 2 (mobile-friendly)
- API: parse musician_ig_handles JSON string → list[str] in crud._to_event_schema
- Schema: EventBase.musician_ig_handles str|None → list[str]|None
- EventCard: defensive normalization in case of stale cached string value
- Header: fix missing key prop on language switcher fragment
- timezone.ts: add WEEKDAYS, formatShortDate, formatShortDateWithDay, formatShortDateRange
- i18n: add group_by_date, group_by_venue, unknown_venue for en/ko/de

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
