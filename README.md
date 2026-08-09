# Recipes

Recipes I actually cook — usually adapted from other sites with some tweaks for how we like to
eat. Published so I stop losing them, and so friends can browse for inspiration.

**Live at:** https://recipes.rohanswami.com

## How it works

- Built with [Jekyll](https://jekyllrb.com/) and hosted on GitHub Pages — no build step to run
  yourself, GitHub builds it on every push to `main`.
- Each recipe is a Markdown file in `_recipes/`, with frontmatter for the source it's adapted
  from, tags, and a changelog of tweaks over time.
- `docs/decisions.md` — running log of setup choices + rationale (same pattern as the
  [Sunday Best](https://github.com/rohanswami92/sunday-best) project).

## Adding a recipe

Copy `_recipes/sticky-chinese-chicken-wings.md` as a starting template. Frontmatter fields:

```yaml
title: Recipe Name
source_name: Site it's adapted from
source_url: https://...
date_added: YYYY-MM-DD
tags: [chicken, mains, asian]
servings: 4
changelog:
  - date: YYYY-MM-DD
    note: What changed and why.
```

When you tweak a recipe later, add a new `changelog` entry rather than silently editing —
that's the point of keeping the log.

## Local preview

```
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Attribution

These are adaptations, not reproductions — each recipe links back to its original source. Please
don't scrape or bulk-republish this content elsewhere.
