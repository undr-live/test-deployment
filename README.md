# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-22T05:46:01Z
- **Source Commit**: [`2eceaba058a79ce7a45d0aa215201febeb59ee85`](https://github.com/keunwoochoi/seoulunderground.live/commit/2eceaba058a79ce7a45d0aa215201febeb59ee85)
- **Branch**: `fix/frontend-copy-fixes`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23396749532)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: remove duplicate CET, drop germany IG handle, clean Korean copy

- CET appeared twice (approxCET() already appends ' CET', call sites
  were appending it again)
- Remove @undr.live_germany.jazz from footer (account doesn't exist)
- Korean welcome: remove '(이하 sul)', replace 'sul' with 'undr.live'

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
