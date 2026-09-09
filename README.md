# DL & GenAI Project Course — GitHub Pages Site

Built with Jekyll's `jekyll-theme-cayman` theme, one of GitHub Pages' natively supported themes (no build setup, no gems to install — just the `theme:` line in `_config.yml`).

## File map

```
.
├── _config.yml               ← site title, description, theme, nav bar order
├── _data/term.yml            ← ALL per-term dynamic values (dates, links, cutoff score)
├── _includes/nav.html        ← shared top navigation, shown on every page
├── _includes/eval_banner.html← shared "latest evaluation policy" callout, shown on every page
├── index.md                  ← Home / overview
├── registration.md           ← Step-by-step registration
├── grading.md                ← Grading formula, deadlines, forms
├── milestones.md             ← Week-by-week plan (rewritten each term — content, not just numbers, changes)
├── viva.md                   ← Viva process
└── faq.md                    ← FAQ
```

## Changing the theme

To try a different look, edit the single `theme:` line in `_config.yml`. Other themes GitHub Pages supports natively without any extra setup:

- `jekyll-theme-cayman` (current) — clean gradient header, professional
- `jekyll-theme-slate` — dark, technical
- `jekyll-theme-architect` — minimal, no sidebar
- `jekyll-theme-minimal` — simple sidebar layout

## Adding a page to the nav bar

Edit the `nav_pages` list in `_config.yml` — the nav on every page is generated from it automatically via `_includes/nav.html`.

## Updating for a new term

1. Open `_data/term.yml` and update the dates, links, cutoff score, and term code.
2. If the actual project topic/milestones changed, rewrite `milestones.md`.
3. If the grading weightage or deadline structure changed structurally (not just dates), edit `grading.md` directly.
4. Commit and push — GitHub rebuilds the site automatically within ~1 minute.

## Archiving old terms

If a term's guidelines differ enough that you want to preserve the old version, copy the whole set of `.md` files (and the `term.yml` values) into an `archive/<term-name>/` folder before overwriting them for the new term.
