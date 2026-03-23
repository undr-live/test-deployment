# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-23T00:09:39Z
- **Source Commit**: [`382a848c011fa907cdf5f4e2fb9f061562de6ea5`](https://github.com/keunwoochoi/seoulunderground.live/commit/382a848c011fa907cdf5f4e2fb9f061562de6ea5)
- **Branch**: `feat/pr-c-performer-instruments`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23415846300)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: use i18n for musicians/featuring label in EventCard

Hardcoded 'Musicians'/'Featuring' strings were showing in English
regardless of the active language. Now routes through t(lang, key).

Added musicians/featuring keys to en/ko/de in i18n.ts.
Added rule to CLAUDE.md: all UI labels must respect the active language.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
