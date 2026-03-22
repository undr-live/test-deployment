# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-22T04:32:18Z
- **Source Commit**: [`e18cbdb9ecbe3ac454b003f3c3808bcce5b5e538`](https://github.com/keunwoochoi/seoulunderground.live/commit/e18cbdb9ecbe3ac454b003f3c3808bcce5b5e538)
- **Branch**: `refactor/remove-hardcoded-paths`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23395702696)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: locale-aware SEO pages + regenerate stale HTML

- Add _UI dict for ko/de/en: html lang, CTA text, last-updated label,
  performers label, service description
- Add _fmt_date() for locale-aware date headers (Korean / English)
- _render_event: add lang param; uses locale performers label
- _render_page: use primary_lang to drive all UI strings; html lang attr
- generate(): load events.{primary_lang}.json (not hardcoded ko); generate
  locale-appropriate title/subtitle/description for non-ko localities
- Regenerate all HTML with corrected output:
  - Germany: <html lang="de">, German CTA/labels, English event text,
    correct CTA URL (/germany/jazz/de), correct IG handle
- Add 11 new tests covering i18n (45 total, all pass)

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
