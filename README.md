# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-27T12:34:28Z
- **Source Commit**: [`370bd08e45a2c76ce943b18618c9e226c022c8ff`](https://github.com/keunwoochoi/seoulunderground.live/commit/370bd08e45a2c76ce943b18618c9e226c022c8ff)
- **Branch**: `feat/musician-highlight-slack-frontend`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23646412401)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: musician highlight — Slack notification + frontend display (#141)

- SlackNotifier.send_musician_highlight(): posts weekly musician card
  with name, instruments, score, top venues, collaborators
- select_highlight.select(): calls Slack after writing JSON (not dry-run)
- export_static_json: copies musician_highlight.json → static API dir
- routers.py: GET /musician-highlight endpoint
- MusicianHighlight TypeScript type in types/highlights.ts
- FeaturedMusician component: accent-bordered banner above events list
- App.tsx: loads /api/musician-highlight, renders FeaturedMusician in
  events tab (hidden in screenshot mode)
- i18n: musician_of_week + instruments keys in en/ko/de

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
