<!-- BEGIN projected-context | sources: fiber@62af9e,dayli@39de38,fiber/memory@1c867b,dayli/memory@f33674 | rendered: f76944 | 2026-09-06 | do not edit -->
## Inherited: Fiber (engagement)

## Fiber: engagement scope

Zygo's portfolio of two consumer nutrition brands on one thesis: fiber is the missing input that restores human resilience (digestive, immune, metabolic, neuro-affective, physical). Dayli Wellness Co sells the daily ritual to health-conscious adults, GTM tilt women 25 to 45 ("Health in Full Color."). Staple Performance Nutrition sells performance digestion to Marcus Filly's Functional Bodybuilding audience ("Nutrition isn't extra. It's Staple."). Ben is founder and operator of both: strategy, build, formation, finance, paid media. Universal rules come from the user layer; this file holds only what is specific to the portfolio.

### Read first

- `../../context/memory.md` before your first non-trivial action; `../../context/memory-inbox.md` is provisional.
- Portfolio-level work: `../../research/00-index.md`, then `../../research/01-thesis-fiber-and-resilience.md`, then the brand scopes `../AGENTS.md` and `../../Staple/AGENTS.md`.
- `../../context/accounts.md` for ids, domains, repositories, and env-var names (dated facts, never values). `../../context/contacts.md` for people and vendors (confidential, never exported). `../../context/team.md` for roles and lanes.
- Entity formation for both LLCs and the Blasto holding structure: `../../context/legal.md` (confidential) and the per-entity resume files it names.

### Invariants

- **Staple was renamed from Persist on 2026-06-15. Never call the brand Persist.** Older files, memory records, and the shortform skill still say Persist and mean Staple.
- **Science lives in `../../research`**; brand-specific research lives in each brand's own research folder. Any mechanistic claim in copy cites a specific file in `../../research/mechanisms` by path. New evidence goes into the mechanism file and `../../research/00-index.md`, never pasted into brand docs. Editorial standards and known library defects: `../../context/research-library.md`.
- **Never mix brand voices in one asset.** Routing when a request arrives without brand context: daily life, women, aesthetics, mass market is Dayli; performance, training, male-skewed, Marcus's audience is Staple; the underlying science is the library, brand-agnostic; when in doubt, ask.
- Brand precedence: Dayli and Staple copy follow each brand's own voice documents; Ben's own messages follow the user-layer voice, playful with this crew. Never mix the two.
- The founder story (`../../founder-story.md`) is internal until Ben publishes it.
- Published pages never mention "our research library" or "our evidence base"; translate to "no trial we could find" without upgrading the claim.

### Working here

- This folder is a git repository with a private GitHub remote. The nested repositories under both brands are independent, never submodules. Ben's pre-existing uncommitted work (the Persist rename, legal drafts, research edits, untracked working folders) stays unstaged unless he says otherwise; never `git add .` inside a legal folder.
- Cross-brand programs, one reference doc each in `../../context`: the SEO and AEO content program, the two ops boards and GTM ownership, research library health, legal. The current state of each is a dated line in `../../context/memory.md`.

## Inherited: DayliWellnessCo (brand)

## Dayli Wellness Co (brand)

Fiber-first daily nutrition brand for health-conscious adults, GTM tilt women 25 to 45. Tagline "Health in Full Color."; manifesto close "This is health, in full color. This is the Dayli way." Amy Buchstaber leads brand and marketing; Primarch manufactures. Portfolio rules come from the scope above; this file adds what is specific to Dayli.

### Invariants

- **dayliwellness.com serves the Shopify store since 2026-08-24** (waitlist phase, zero products by design, email capture native). `.` is the retired static site and a rollback artifact only; site copy work targets the theme (snapshot in `../shopify-theme-backup`). Store, DNS, and publishing facts: `../context/site-and-store.md`.
- **Two launch SKUs:** Electrolytes + Fiber (Raspberry Lemonade; 5 g SoFiber soluble tapioca fiber, magnesium glycinate) and JamPact (seven whole plants, 18.5 g scoop, 11 g fiber, confirmed and printable 2026-08-24). NO WHEY! is dropped; PHGG and Sunfiber are Staple's fiber, never Dayli's. Formulas and COGS state: `../context/products.md`.
- **Voice authority is `../research/10-voice-and-tone-guide.md`** (Register B for web, email, SMS, social: no em-dash at all; ration devices, load specificity; never invent brand history, founder biography, customer anecdotes, or Amy's experiences, leave a NEEDS placeholder). `../research/04-copywriting-guide.md` is superseded and teaches the wrong fiber; never write from it. Summary: `../context/brand.md`.
- Structure-function claims only; compliant replacement pairs are in voice guide Part VIII. Before content ships, run the citation audit and the ration audit named in `../context/content-program.md`.
- Mechanistic claims cite `../../research/mechanisms` by path (portfolio rule).

### Read on task

- Content program (roadmap, sprints, gates, the open RD hire, tooling): `../context/content-program.md`. Products and formulation: `../context/products.md`. Store, theme, DNS, Journal publishing, Google Workspace: `../context/site-and-store.md`. Brand kit and voice doctrine: `../context/brand.md`.
- Operating-agreement work starts at `../legal/HANDOFF.md` (confidential, untracked); the portfolio entity summary is the engagement's legal.md.
- Memory: `../context/memory.md`; propose to `../context/memory-inbox.md`.

### Working here

- `.` and `../shopify-theme-backup` are independent git repositories with their own scope files. `../content`, `../site-copy-variant-b`, `../docs`, and the SEO_AEO Dayli folder are Ben's working folders, some untracked.

## Inherited gotchas

- 2026-08-31 [startup] The shared research library carries known errors that both brands inherit: mechanisms/08-motility-transit.md prescribes water at 250 mL per gram where it means about 25 mL (unpatched in the library, fixed only in Dayli article 13); three ingredient files (zinc-carnosine, bacillus-coagulans-gbi30, solnul) carry correction banners the sections below them never adopted; 13 wrong DOIs were fixed in August but the wrong author names (Marciani for Gunn, Park 2015 for Jung 2003) remain in library prose; a wrong rectal-distension figure reached a live article. Verify figures and citations against the primary source before they reach copy for either brand, and fix the library first, then the articles, then check whether the other brand inherited it.  (from fiber)
- 2026-08-24 [startup] dayliwellness.com is attached to two Vercel projects, dayli-wellness-co (the retired site) and dayli-ops (the live ops board): removing the domain with the Vercel CLI is account-wide and would take the ops board down. Use the project-scoped REST domains endpoint, apex before www (deleting www first returns 409 while the apex redirects to it). The domain itself now resolves to Shopify; DNS stays at GoDaddy.  (from dayli)
<!-- END projected-context -->

<!-- BEGIN startup-gotchas | sources: dayli-website/memory@0509d8 | rendered: 156d8f | 2026-09-06 | do not edit -->
## Startup gotchas (generated from context/memory.md)

- 2026-08-24 [startup] Pushing to main still auto-deploys the Vercel project, but dayliwellness.com has served the Shopify store since 2026-08-24 and DNS stays at GoDaddy; nothing here reaches the public domain, and the retired pages carry disease-claim headings that must not return.
<!-- END startup-gotchas -->

# Dayli legacy website (project repository): retired static site

The four-page static site (index, fiber, pcos, menopause; Tailwind via CDN, vanilla JS, no build step, cleanUrls in vercel.json) that served dayliwellness.com from 2026-02-21 until the Shopify cutover on 2026-08-24. GitHub Bljohnson-cmd/DayliWellnessCo (public); Vercel project dayli-wellness-co still auto-deploys pushes to `main`, but the domain no longer points here. The inherited blocks above carry the portfolio and brand rules.

- This repository is a rollback artifact. Do no copy work here: the live site is the Shopify theme (brand scope, site-and-store.md). When retired, these pages carried five disease-claim headings, 93 em-dashes, and 24 broken headings; a push would republish them to the Vercel alias only, never to the domain.
- `.env` here holds the Shopify custom-app client id and secret and the USDA key used by the content tooling; it is gitignored (added 2026-08-24 after nearly being committed). Never commit it, never echo a value; reference the variable names in the engagement's accounts.md.
- The NO WHEY! renders in `images/` are obsolete; the Electrolytes and JamPact pouches were CSS placeholders.
- Rollback state (pre-cutover DNS snapshot and runbook) lives in the brand folder's docs; the domain is attached to two Vercel projects, so never remove it with the CLI.
- Memory: `context/memory.md`; propose to `context/memory-inbox.md`.
