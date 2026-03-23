# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T02:04:56Z
- **Source Commit**: [`02a46ce98449a9816e34d7389db539669c961234`](https://github.com/keunwoochoi/seoulunderground.live/commit/02a46ce98449a9816e34d7389db539669c961234)
- **Branch**: `feat/pr-d-ical-export`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23418332671)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: RFC 5545 line folding + robust UID fallback in iCal export

- foldLine(): fold lines exceeding 75 octets with CRLF+space per RFC 5545 §3.1;
  uses TextEncoder for accurate UTF-8 byte counting (Korean titles are 3 bytes/char)
- UID fallback: use datetime+title+venue_name composite instead of datetime alone
  to avoid collisions when two events share the same start time

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
