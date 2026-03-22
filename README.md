# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-22T04:20:16Z
- **Source Commit**: [`de036df811d98662485c068f76eb265e86212b78`](https://github.com/keunwoochoi/seoulunderground.live/commit/de036df811d98662485c068f76eb265e86212b78)
- **Branch**: `refactor/remove-hardcoded-paths`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23395536088)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: resolve runner.home error + opt into Node.js 24 across all workflows

runner.home is not available in job-level env: expressions; move
DEV_WORKSPACE resolution to a dedicated setup step using $GITHUB_ENV
with vars.DEV_WORKSPACE as override and $HOME/Codes/seoul.music as
fallback. Apply to both deploy-pages.yml and deploy-test.yml.

Also fix hardcoded /Users/keunwoo path in deploy-test.yml (uses
$DEV_WORKSPACE now like deploy-pages.yml).

Add FORCE_JAVASCRIPT_ACTIONS_TO_NODE24: true to all jobs to opt in
before the June 2026 forced migration; bump node-version 20 → 24
in all setup-node steps.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
