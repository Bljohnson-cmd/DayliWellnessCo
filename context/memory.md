# Dayli legacy website memory

## Decisions

- 2026-02-21 | Site launched on Vercel via GitHub auto-deploy; multi-page static HTML with cleanUrls routing; DM Serif Display and Inter; cream, charcoal, terracotta, golden, sage palette.
- 2026-06-04 | Reworked for the GTM pipeline (JamPact plus Electrolytes + Fiber; NO WHEY! removed from copy); last content commit 7bca0ce.
- 2026-08-24 | Retired from the domain by the Shopify cutover; kept as a rollback artifact.

## Preferences

- 2026-08-20 | Any variant of this copy wants a branch or a separate file, never an in-place edit on main, because a push deploys.

## Gotchas

- 2026-08-24 [startup] Pushing to main still auto-deploys the Vercel project, but dayliwellness.com has served the Shopify store since 2026-08-24 and DNS stays at GoDaddy; nothing here reaches the public domain, and the retired pages carry disease-claim headings that must not return.
- 2026-08-24 | The `.env` in this folder is real (Shopify custom-app client id and secret, USDA key) and gitignored; it was one add-all from being served at a public path before the ignore was added.
- 2026-08-20 | Audit numbers at retirement: 93 em-dashes, 1 en-dash, 24 bare line breaks inside h1 to h3 (which concatenate words on extraction), five disease-claim headings, zero JSON-LD, zero canonicals, no robots.txt or sitemap, zero img tags. The compliant replacements are in the voice guide Part VIII if any of this copy is ever reused.
