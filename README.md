# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-16T01:29:58Z
- **Source Commit**: [`29cc0fbf65c34f7dcfd3eb2c9e1e76fa90ddb1b9`](https://github.com/keunwoochoi/seoulunderground.live/commit/29cc0fbf65c34f7dcfd3eb2c9e1e76fa90ddb1b9)
- **Branch**: `feat/musician-pipeline-phase2`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23124172047)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: address Gemini code review — dead code, regex strictness, lang param

- name_match.py: remove dead `overlap` assignment that was immediately overwritten
- link_events.py: remove trailing \s*$ from _NAME_INST_RE so segments with
  trailing punctuation (e.g. "Lee Han-jin (trombone).") still match
- App.tsx MusicianList + MusicianProfile: use typedLang from route params
  instead of hardcoded 'en' for API calls

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
