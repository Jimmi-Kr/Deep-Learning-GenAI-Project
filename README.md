# DL & GenAI Project Course — GitHub Pages Site

Built with plain Jekyll (GitHub Pages runs this automatically, no setup needed) using a fully custom layout instead of a pre-built theme — this gives full control over header height, buttons, and a title that stays fixed across every page.

## File map

```
.
├── _config.yml                ← site title, description, nav bar order, no theme dependency
├── _data/term.yml             ← ALL per-term dynamic values (dates, links, cutoff score)
├── _layouts/default.html      ← the page shell: header (title/tagline/buttons), footer, all CSS
├── _includes/nav.html         ← shared top navigation, shown on every page
├── _includes/eval_banner.html ← shared "latest evaluation policy" callout, shown on every page
├── index.md                   ← Home / overview
├── registration.md            ← Step-by-step registration
├── grading.md                 ← Grading formula, deadlines, forms
├── milestones.md               ← Week-by-week plan (rewritten each term — content, not just numbers, changes)
├── viva.md                    ← Viva process
└── faq.md                     ← FAQ
```

## Customizing the header

Open `_layouts/default.html`:
- The title/tagline (`{{ site.title }}` / `{{ site.description }}`) come straight from `_config.yml` — they stay the same on every page regardless of which nav link you click.
- The two header buttons pull `kaggle_competition_link` and `portal_link` from `_data/term.yml` — edit those values there, not in this file.
- Header height/colors are plain CSS inside the `<style>` block at the top — change `padding` on `header.hero` to make it taller/shorter, or the `--grad-start`/`--grad-end` variables to change the gradient colors.

## Adding a page to the nav bar

Edit the `nav_pages` list in `_config.yml` — the nav on every page is generated from it automatically via `_includes/nav.html`.

## Updating for a new term

1. Open `_data/term.yml` and update the dates, links, cutoff score, and term code.
2. If the actual project topic/milestones changed, rewrite `milestones.md`.
3. If the grading weightage or deadline structure changed structurally (not just dates), edit `grading.md` directly.
4. Commit and push — GitHub rebuilds the site automatically within ~1 minute.

## Archiving old terms

If a term's guidelines differ enough that you want to preserve the old version, copy the whole set of `.md` files (and the `term.yml` values) into an `archive/<term-name>/` folder before overwriting them for the new term.
