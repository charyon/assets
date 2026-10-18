# Service logos: source and license

All four marks come from **Simple Icons 16.35.0** (git tag `16.35.0`, commit `4d29a35c954699b389a834aacc97dd6e7e74143c`). Each file is the upstream SVG, byte for byte.

- **License for the SVG data:** CC0-1.0 (Simple Icons `LICENSE.md`).
- **Trademarks:** CC0 covers only the drawing. Each mark is still its owner's trademark. We use them only to label a link to that service, unmodified apart from a fill color, with no suggestion of endorsement. The buttons in `../buttons/` are generated from these paths by the charyon template build.

| File | Mark | Brand hex | Owner's brand source / guidelines | sha256 |
| --- | --- | --- | --- | --- |
| `logos/cloudflare.svg` | Cloudflare | `F38020` | https://www.cloudflare.com/logo/; guidelines https://www.cloudflare.com/trademark/ | `408096d99907fd99…` |
| `logos/githubactions.svg` | GitHub Actions | `2088FF` | https://github.com/features/actions; GitHub logo policy https://github.com/logos | `e8b23379b4d89e96…` |
| `logos/linear.svg` | Linear | `5E6AD2` | https://linear.app (Simple Icons' listed source) | `90b91b61090f4f9c…` |
| `logos/vercel.svg` | Vercel | `000000` | https://vercel.com/geist/brands (source and guidelines) | `57f1e4135486c566…` |

Colors used on buttons:
- The brand hex on the light variant.
- On the dark variant, Linear and GitHub Actions use a lighter tint of the same hue (`#8b93ff`, `#4493f8`) so they stay readable on `#21262d`.
- Vercel is black on light and white on dark, as its guidelines allow.
- Cloudflare's orange is the same in both.

A button appears only on a PR that touches a service the repo allowlists in `.github/repo-override.yml` `services:`. The pilot allowlists github-actions, linear and cloudflare. `vercel` is in the catalog but no enrolled repo uses it.

Layout ideas came from the Cursor Bugbot and Qodo PR-comment buttons: a small rounded pill, the logo before the label, `<picture>` with dark and light sources, and an explicit height. None of their markup or art was copied. The size (20 px), colors, label text, and spacing are our own.
