# Infectious Disease Epidemiology Brief (California-focused)

This repo hosts a concise, policy-relevant newsletter focused on infectious disease epidemiology and infectious disease *occupational* epidemiology, with a major focus on **California**.

## Publishing
- Website: GitHub Pages (from `/docs`)
- Latest edition: `/docs/index.md`
- Archive: `/docs/editions/YYYY-MM-DD.md`

## Automation
A daily 8:00 AM **America/Los_Angeles** OpenClaw cron job can generate and publish the latest edition.

### Required configuration
To generate citable updates automatically, OpenClaw needs web search enabled:
- Set `BRAVE_API_KEY` in the OpenClaw Gateway environment (recommended), or
- Run: `openclaw configure --section web`

## Editorial standards
- Evidence-first; neutral tone.
- Reputable sources only (CDPH, county health departments, CDC/MMWR, WHO, peer-reviewed journals).
- Citations (links) for every major claim/outbreak/numerical trend.
