# Infectious Disease Epidemiology Brief (California-focused)

This repo hosts a concise, policy-relevant newsletter focused on infectious disease epidemiology and infectious disease *occupational* epidemiology, with a major focus on **California**.

## Publishing
- Website: GitHub Pages (from `/docs`)
- Latest edition: `/docs/index.md`
- Archive: `/docs/editions/YYYY-MM-DD.md`

## Automation
A daily 8:00 AM **America/Los_Angeles** OpenClaw cron job generates and publishes the latest edition.

### Source strategy (no paid search required)
This pipeline is designed to run **without** a paid web search API:
- Start from a curated, fetch-first seed list: `sources/seeds.json` (documented in `sources/SEEDS.md`).
- Prefer official static pages and PDF advisories.
- If an endpoint is blocked (e.g., Cloudflare) or fails TLS/intermediate-chain delivery, the edition must note the limitation in **Data Notes & Caveats**.

(If you later add a search API key, it can be used as a supplement—but seeds remain the baseline.)

## Editorial standards
- Evidence-first; neutral tone.
- Reputable sources only (CDPH, county health departments, CDC/MMWR, WHO, peer-reviewed journals).
- Citations (links) for every major claim/outbreak/numerical trend.
