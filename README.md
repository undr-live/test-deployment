# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-02T04:27:18Z
- **Source Commit**: [`5db417319d5c4920649c131afb0f2c54b933ee8b`](https://github.com/keunwoochoi/seoulunderground.live/commit/5db417319d5c4920649c131afb0f2c54b933ee8b)
- **Branch**: `feat/tier-based-venue-sampling`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/22561396770)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: Add tier migration to deployment workflows

Both production and test deployments now run the tier migration script
to populate venue tier information after importing data.

Changes:
- deploy-pages.yml: Run migration after venue/event imports
- deploy-test.yml: Run migration before exporting static JSON

This ensures tier-based venue sorting works on deployed sites.

Made-with: Cursor

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
