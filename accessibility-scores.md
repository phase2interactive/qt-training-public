# Accessibility Scores

Lighthouse 12.6.1 accessibility audit (headless Chrome, default mobile config), run 2026-11-09 against the local app at `http://localhost:5268`.

| Page | URL | Score |
|------|-----|-------|
| Customer ordering | `/` | 100 |
| Kitchen | `/kitchen` | 94 |

## Failing audits

- **`/kitchen` — color-contrast:** the "Ready" status badge (`.badge-ready`, `#438945` on `#e8f3e7`) has a contrast ratio of 3.75:1; WCAG AA requires 4.5:1 for this text size.
