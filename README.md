# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-22T03:34:43Z
- **Source Commit**: [`4eb7366454ca789ce492489c83652bb330b7a0fa`](https://github.com/keunwoochoi/seoulunderground.live/commit/4eb7366454ca789ce492489c83652bb330b7a0fa)
- **Branch**: `refactor/remove-hardcoded-paths`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23394892932)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: refactor: remove hardcoded paths and inline config values

1. deploy-pages.yml: replace /Users/keunwoo/... with $DEV_WORKSPACE
   (configurable via GitHub Actions variable, defaults to $HOME/Codes/seoul.music)
   and $HOME for the github_actions temp dir sweep.

2. launchd plists: replace /Users/keunwoo/... with __PROJECT_DIR__ and
   __HOME_DIR__ placeholders. Add config/launchd/install.sh to stamp in
   real paths and load into ~/Library/LaunchAgents/ on any machine.

3. ig_post_daily.py: replace inline {"jazz": "재즈", ...} dict with
   config.GENRES[genre]["display_name_ko"].

4. generate_seo_pages.py: replace hardcoded LOCALITIES = [("seoul","jazz")]
   with a derivation from config.LOCALITY_GENRE_REGISTRY (enabled entries).
   Fix output path collision: now writes to public/{locality}/{genre}/.
   Add display_name/display_name_ko to config.LOCALITIES and config.GENRES.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
