# Accessibility Scores

Lighthouse 12.6.1 accessibility audit (headless Chrome, default mobile config) against the local app at `http://localhost:5268`, run with `.claude/skills/accessibility-check/scripts/audit.sh`.

## Latest — 2026-11-09 (after adding per-pizza special instructions)

| Page | URL | Score |
|------|-----|-------|
| Customer ordering | `/` | 100 |
| Kitchen | `/kitchen` | 94 |

### Failing audits

- **`/kitchen` — color-contrast:** the "Ready" status badge (`.badge-ready`, `#438945` on `#e8f3e7`) has a contrast ratio of 3.75:1; WCAG AA requires 4.5:1 for this text size. Unchanged from the previous run.

## History

| Date | Change | `/` | `/kitchen` |
|------|--------|----:|-----------:|
| 2026-11-09 | Baseline | 100 | 94 |
| 2026-11-09 | Per-pizza special instructions | 100 | 94 |
