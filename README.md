# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-02T04:20:33Z
- **Source Commit**: [`21d754ae6bf2e675c8c6b0e219676df535dc6fb1`](https://github.com/keunwoochoi/seoulunderground.live/commit/21d754ae6bf2e675c8c6b0e219676df535dc6fb1)
- **Branch**: `feat/tier-based-venue-sampling`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/22561250245)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: Add tier-based venue sorting

Add tier field to venues table and update frontend to sort venues by tier
first (0=great, 1=real jazz bar, 2=hybrid, 3=not recommended), then by
event count within each tier.

Backend changes:
- Add tier column to Venue model (Integer, default=1)
- Update Venue schema to include tier field
- Include tier in API responses from list_venues endpoint
- Create migration script to populate tier from venue_handles.csv

Frontend changes:
- Add tier field to Venue type
- Update venue sorting logic to sort by tier (ascending), then event count (descending)

Migration:
- Run scripts/db_add_venue_tier_column.py to add column and populate data
- Reads from venue_handles.csv (if exists) or venue_handles.txt (defaults to tier 1)

Made-with: Cursor

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
