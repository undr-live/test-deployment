# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-29T17:42:02Z
- **Source Commit**: [`5d7e751c1728ecdde09be5918c6c3a3418629763`](https://github.com/keunwoochoi/seoulunderground.live/commit/5d7e751c1728ecdde09be5918c6c3a3418629763)
- **Branch**: `feat/musician-connections`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23715035723)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: venue nav → venues tab; fade upcoming date badge by days away

- Musician profile venue links now navigate to ?tab=venues&q=handle
  (was going to events tab)
- Upcoming show badge on musician cards fades based on days until show:
  today/tomorrow=100%, 2-3d=80%, 4-7d=65%, 8-14d=50%, 15+d=35%

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
