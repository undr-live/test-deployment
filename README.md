# Seoul Underground Live - TEST DEPLOYMENT

⚠️ **This is a TEST/STAGING environment** ⚠️

## Build Information

- **Environment**: TEST
- **Build Time**: 2026-03-26T14:47:59Z
- **Source Commit**: [`1bafe85e25e53bd7610d4b0fb0e21a11fa19155d`](https://github.com/keunwoochoi/seoulunderground.live/commit/1bafe85e25e53bd7610d4b0fb0e21a11fa19155d)
- **Branch**: `fix/qwen-merge-no-hallucination`
- **Workflow Run**: [View logs](https://github.com/keunwoochoi/seoulunderground.live/actions/runs/23600738171)

## Commit Details

- **Author**: Keunwoo Choi <gnuchoi+github@gmail.com>
- **Message**: fix: Qwen merge prompt must never hallucinate — union only, no synthesis

The old merge prompt instructed Qwen to "write a NEW synthesized
description" combining "atmosphere/narrative" from both sources. This
caused Qwen to generate vivid marketing copy ("Experience the vibrant
atmosphere...", "unforgettable night of live jazz") even when both
source descriptions were null.

New prompt rule: output is the union of A and B only. Never invent,
infer, or embellish. If a field is null in both, output null. Tested
across 4 null/non-null scenarios + 20 random real-data pairs + all
once-bad event pairs — 0 hallucinations.

Also add principle to CLAUDE.md and dept-engineering.md: when debugging
bad data, audit every step that can write that field, not just the first
plausible one.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>

## Deployment URLs

- **Test Site**: https://test.undr.live
- **Production Site**: https://undr.live

## Data Snapshot

The static JSON files in `/api/` were exported from the local backend at build time.
Events shown are from the crawler's database as of the build timestamp above.

---

*This README is auto-generated during deployment. Do not edit manually.*
