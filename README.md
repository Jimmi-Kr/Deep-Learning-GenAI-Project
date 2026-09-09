# DL & GenAI Project Course — GitHub Pages Site

Built with Jekyll's default `minima` theme, which GitHub Pages supports natively (no build setup needed on your end).

## File map

```
.
├── _config.yml       ← site title, description, nav bar order
├── _data/term.yml    ← ALL per-term dynamic values (dates, links, cutoff score)
├── index.md          ← Home / overview
├── registration.md   ← Step-by-step registration
├── grading.md        ← Grading formula, deadlines, forms
├── milestones.md     ← Week-by-week plan (rewritten each term — content, not just numbers, changes)
├── viva.md           ← Viva process
└── faq.md            ← FAQ
```

## Updating for a new term

1. Open `_data/term.yml` and update the dates, links, cutoff score, and term code.
2. If the actual project topic/milestones changed, rewrite `milestones.md`.
3. If the grading weightage or deadline structure changed structurally (not just dates), edit `grading.md` directly.
4. Commit and push — GitHub rebuilds the site automatically within ~1 minute.

## Archiving old terms

If a term's guidelines differ enough that you want to preserve the old version, copy the whole set of `.md` files (and the `term.yml` values) into an `archive/<term-name>/` folder before overwriting them for the new term.
