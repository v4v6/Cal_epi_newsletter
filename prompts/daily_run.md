You are generating the **Infectious Disease Epidemiology Brief**.

Hard requirements:
- Time window: most recent 7–10 days prior to edition date.
- California is the primary focus (CDPH + key counties: LA, SD, Alameda, Santa Clara, SF, Sacramento).
- Secondary: rest of US; tertiary: rest of world.
- Reputable sources only; provide citations/links for every major claim.
- Label preliminary evidence.
- 900–1,300 words, professional neutral, action-oriented.

Output targets:
1) Write today’s edition to: `docs/editions/YYYY-MM-DD.md`
2) Update `docs/index.md` to point to the latest edition.
3) Commit + push to `main`.

Source acquisition (hardened workflow):
- Use the curated seed list in `sources/seeds.json` (and documentation in `sources/SEEDS.md`) as your **starting point**.
- Prefer endpoints that are reliably fetchable (static HTML, PDF advisories, MMWR pages, CDC outbreak pages).
- If a key county/CDPH page is blocked (Cloudflare) or fails TLS chain delivery, consult `sources/fallback_matrix.md` and use the **approved substitute**.
- **Do not guess**: cite what you can, and clearly record the limitation/substitution in **Data Notes & Caveats**.

Operational emphasis:
- Prefer official situation updates, advisories, outbreak investigation pages, surveillance summaries.
- Include occupational epi where available (healthcare worker exposure guidance, nosocomial clusters, lab/diagnostic alerts).
