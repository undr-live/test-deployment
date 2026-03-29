# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-29T07:11:52Z
- **Source Commit**: [`1773c06678d0b4f1ab52c99b38a5255dcb7da0d2`](https://github.com/keunwoochoi/seoulunderground.live/commit/1773c06678d0b4f1ab52c99b38a5255dcb7da0d2)
- **Branch**: `feat/musician-connections`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23703823896)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: venue links always show all events (add &all=1)

- Musician profile venue links: navigate to ?q=handle&all=1
- VenueCard '공연일정 보기': add &all=1 so all future events shown,
  not just this week's default

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
