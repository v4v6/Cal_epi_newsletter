# Curated seed sources (fetch-first)

Purpose: provide a **stable, reputable, and usually machine-fetchable** set of endpoints for the daily newsletter. These are preferred over ad-hoc searching.

Use these in priority order. If a seed is blocked (Cloudflare), redirects to HTTP, or fails TLS chain delivery, note it in **Data Notes & Caveats** and move to the next seed.

## California (primary)

### CDPH (California Department of Public Health)
- CDPH COVID-19 hub (stable HTML):
  - https://www.cdph.ca.gov/Programs/CID/DCDC/Pages/Immunization/ncov2019.aspx
- CDPH communicable disease control landing (directory-style):
  - https://www.cdph.ca.gov/Programs/CID/DCDC/Pages/CommunicableDiseaseControl.aspx

**Note (TLS chain issues):** some CDPH pages intermittently fail automated verification because the site may not provide a needed intermediate certificate. If that occurs, use the bundled intermediate in `sources/certs/` to build a custom CA bundle.

### San Francisco Department of Public Health (SFDPH)
- SFDPH health alerts (includes PDFs with publication dates):
  - https://www.sf.gov/resource/2024/health-alerts

### CDC (national, but high relevance)
- MMWR index:
  - https://www.cdc.gov/mmwr/index.html
- CDC Current Outbreak List:
  - https://www.cdc.gov/outbreaks/index.html

## Counties (secondary CA coverage)

These may be intermittently blocked for automated fetch. Prefer static pages and PDF endpoints.

### Los Angeles County DPH
- Newsroom / media (may redirect):
  - https://publichealth.lacounty.gov/media/

### Alameda County Public Health Department
- Health alerts:
  - https://acphd.org/health-alerts/

### Santa Clara County Public Health
- News:
  - https://publichealth.sccgov.org/news

### San Diego County
- Communicable disease / epi pages (URL structure changes periodically):
  - https://www.sandiegocounty.gov/content/sdc/hhsa/programs/phs/community_epidemiology/dc/communicable_disease.html

### Sacramento County
- Latest news landing (AEM; sometimes path changes):
  - https://www.saccounty.gov/news/latest-news/

## World (tertiary)
- WHO Disease Outbreak News:
  - https://www.who.int/emergencies/disease-outbreak-news

