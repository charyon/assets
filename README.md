# assets

Public brand and badge assets for charyon templates.

The PR templates synced from `charyon/repository-kit` (`baseline/manifest.yml`, `assets.base`) link to these files
by **SHA-pinned raw URL**: `https://raw.githubusercontent.com/charyon/assets/<commit>/<path>`. A change here never
alters a rendered template until the kit moves `assets.base` to the new commit by PR. Don't edit or delete
published files in place; add new ones.

| Path | Size | Notes |
| --- | --- | --- |
| `badges/risk-low.svg`, `risk-medium.svg`, `risk-high.svg` | 20 px tall; 61 / 87 / 67 px wide | One file works in both themes: white 11 px semibold text on `#59636e` plus `#1a7f37` / `#9a6700` / `#cf222e`, which are GitHub's own emphasis colors |
| `buttons/<service>-dark.svg`, `<service>-light.svg` | 20 px tall | github-actions "PR checks", linear "Linear issue", cloudflare "Cloudflare deploy", vercel "Vercel preview". Shown with `<picture>` only on PRs that touch that service |
| `logos/*.svg` | — | Upstream Simple Icons 16.35.0 marks. Licenses and trademark notes are in [`logos/LICENSES.md`](logos/LICENSES.md) |

The SVGs are generated; don't hand-edit them. Text uses `textLength`, so widths hold in any font. In a template,
use `<img … height="20" align="absmiddle">`, which keeps the badge inline with the text.

This repo has no workflows and runs no CI.
