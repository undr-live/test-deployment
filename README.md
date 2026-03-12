# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-12T15:40:01Z
- **Source Commit**: [`6dbfa29b643f5b7a50621d9ba84bb7f4f0b50326`](https://github.com/keunwoochoi/seoulunderground.live/commit/6dbfa29b643f5b7a50621d9ba84bb7f4f0b50326)
- **Branch**: `eval-multi-model-dashboard`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23010360626)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: feat: restructure evals/ to seoul/jazz locality layout + multi-model eval dashboard

- Add evals/paths.py: centralized path helpers parameterized by locality/genre,
  mirroring the data/seoul/jazz/ directory structure
- Move evals/golden/, evals/results/, evals/manifest.json →
  evals/seoul/jazz/{golden,results,manifest.json}
- Update .gitattributes LFS pattern to evals/*/*/golden/events/**/*.jpg
- Update all eval scripts (run, analyze, inspect, compare, collect_baseline,
  labeler/server, scripts/collect_golden_data) to use evals.paths helpers
- Fix evals/compare.py: split title_match_rate → title_match_strict + title_match_fuzzy,
  add TP/FP/FN/TN confusion matrix rows
- Add evals/seoul/jazz/DASHBOARD.md: full comparison of three models on 58 labeled cases
  (v4.0.3 prompt + post-date + venue context)

Results (58-case ground truth, v4.0.3 prompt):
  gemini-2.5-flash:          is_event 98.3%, date 100%, title fuzzy 90.2%
  gemini-3-flash-preview:    is_event 96.6%, date 100%, title fuzzy 96.4% (best title)
  gemini-3.1-flash-lite:     is_event 94.8%, date 100%, title fuzzy 96.3% (most FN)

Made-with: Cursor

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
