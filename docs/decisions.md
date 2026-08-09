# Decision Log

Running log of meaningful choices and *why*, newest first.

## 2026-08-09 — Project kicked off

- **Goal:** publish recipes (mostly adapted from other sites, tweaked to taste) somewhere easy
  for the user and his wife to find, and browsable by friends for inspiration. Updated every few
  weeks, with a changelog of tweaks per recipe.
- **No backend needed.** Static content, infrequent updates, no accounts/interactivity — ruled
  out Vercel/a framework with a server. Static site + GitHub Pages fits, and reuses the hosting
  pattern already proven on [Sunday Best](https://github.com/rohanswami92/sunday-best)
  (`sundaybest.rohanswami.com`, GitHub Pages + custom subdomain).
- **Jekyll chosen over Eleventy or a custom script.** GitHub Pages builds Jekyll natively — no
  GitHub Actions workflow required (Sunday Best needed one only because its prototype isn't
  Jekyll). Recipes modeled as a Jekyll *collection* (`_recipes/`) with frontmatter for source
  attribution, tags, and a `changelog` array — chosen so tweaks are recorded as structured,
  dated entries rather than lost in prose or git history alone.
- **Public repo.** Unlike Sunday Best (private product bet), this is just content meant to be
  shared — public repo means friends can browse it directly and free GitHub Pages hosting has no
  plan requirement.
- **Domain:** `recipes.rohanswami.com`, same CNAME pattern as `sundaybest.rohanswami.com`.
- **Attribution stance:** every recipe links back to its original source site; content here is
  adapted/rewritten in the user's own words, not copy-pasted verbatim.
