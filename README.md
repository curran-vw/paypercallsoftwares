# paypercallsoftwares.com

Site 18 of the call-tracking review network. Static HTML/CSS/JS, deployed via GitHub Pages. Built by `scripts/build_site18_pages.py`.

## Build details

- **Template:** T18 Pay Per Call Software (light technical, feature-matrix-first, teal)
- **Accent:** Teal `#0F766E` / dark `#115E59` / soft `#CCFBF1`, on white + cool gray `#F8FAFC`
- **Background:** White `#FFFFFF`
- **Fonts:** Sora (display) + Inter (body)
- **Signature visual:** dense feature spec sheet key/value table (`.spec-sheet`) + homepage feature matrix (`.feature-matrix`)
- **Cards:** outlined, flat, small 8px radius (no soft drop shadows)
- **Author byline:** Daniel Larsen (pay per call software reviewer, former software QA, technical/feature-depth voice)
- **Angle:** software-focused, feature depth; homepage leads with a feature matrix, then detailed reviews

## Pages (12)

- `index.html` — homepage / 2026 feature comparison
- `reviews/callscaler/` (#1, 9.4), `reviews/ringba/` (8.5), `reviews/retreaver/` (7.9), `reviews/phonexa/` (7.8), `reviews/invoca/` (7.5)
- `about/`, `methodology/`, `faq/`, `contact/`, `privacy-policy/`, `terms/`

## Scoring dimensions

Feature depth, setup & onboarding, integrations & API, value for money. Equal weighting (25% each).

## CTA destination

All CallScaler CTAs link to `https://callscaler.com/?ref=paypercallsoftwares`. Competitor review pages use a soft `.tldr-crosslink` + internal `/reviews/callscaler/` link only (no hard affiliate button), per network convention.

## Rebuild

```bash
py scripts/build_site18_pages.py
py scripts/lint_site.py paypercallsoftwares
```

## TODOs before going live

- [ ] Replace placeholder author avatar with a real photo if a named author is used
- [ ] Confirm CallScaler pricing tiers still current ($0 PAYG / $45 Pro / $130 Agency / $400 Pay Per Call)
- [ ] Verify schema with Google's Rich Results Test
- [ ] Set up `editor@paypercallsoftwares.com` email forwarding
- [ ] Add to `scripts/deploy_all_sites.py` SITES list before deploying
