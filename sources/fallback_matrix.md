# Fallback matrix (California-first)

Goal: keep daily production stable when a preferred county/CDPH endpoint is blocked (Cloudflare), redirects unexpectedly, or fails TLS chain delivery. This matrix defines **approved substitutes** that remain reputable.

Principles
- Prefer **the same jurisdiction’s official content** (alternate URL, PDF library, RSS) before substituting another jurisdiction.
- If substituting outside jurisdiction, clearly label as a **proxy signal** (e.g., CDC national guidance relevant to CA).
- Never infer missing numbers. If data cannot be retrieved, document the gap in **Data Notes & Caveats**.

## CDPH (statewide)
**Primary**
- CDPH COVID-19 hub: https://www.cdph.ca.gov/Programs/CID/DCDC/Pages/Immunization/ncov2019.aspx
- CDPH Communicable Disease Control landing: https://www.cdph.ca.gov/Programs/CID/DCDC/Pages/CommunicableDiseaseControl.aspx

**If CDPH respiratory surveillance pages fail (TLS/intermediate chain or 404):**
1) Use **SFDPH clinician updates** as a California sentinel for provider-facing priorities (explicitly label as SF-only): https://www.sf.gov/resource/2024/health-alerts
2) Use **CDC MMWR** for methods/guidance changes affecting CA operations: https://www.cdc.gov/mmwr/index.html
3) Use **CDC respiratory/seasonal guidance pages** if needed (not a substitute for CA-specific trends; cite as national guidance): https://www.cdc.gov/ (navigate to the relevant program page)

## Santa Clara County (SCC)
**Primary**
- SCC Public Health News (often Cloudflare-blocked): https://publichealth.sccgov.org/news

**If SCC blocks automated fetch:**
1) Attempt SCC **site search / alternate public endpoints** (still official):
   - https://publichealth.sccgov.org/ (home page; sometimes fetchable even if /news blocks)
2) If still blocked, substitute **SFDPH alerts** + **CDPH statewide hubs** for clinician-facing issues likely to be shared regionally.
3) If the item is likely to be a multi-county event (e.g., foodborne cluster), use CDC outbreak investigations as the authoritative cross-jurisdiction substitute:
   - https://www.cdc.gov/outbreaks/index.html

## Los Angeles County DPH
**Primary**
- LA County DPH media/news: https://publichealth.lacounty.gov/media/

**If LA County endpoint redirects to HTTP or fails TLS/SNI:**
1) Try the county root domain (same jurisdiction) and navigate to Public Health news:
   - https://lacounty.gov/
2) Use CDC outbreak pages (foodborne) or CDC HAN/MMWR (health alerts) as the stopgap, with a clear note that LA-specific advisories could not be retrieved.

## Alameda County Public Health
**Primary**
- Health Alerts: https://acphd.org/health-alerts/

**If blocked:**
1) Try ACPHD homepage “Health Alerts” links (same domain): https://acphd.org/
2) Substitute SFDPH alerts for Bay Area clinical signals; note jurisdiction difference.

## San Diego County
**Primary**
- Communicable disease page (URL can change): https://www.sandiegocounty.gov/content/sdc/hhsa/programs/phs/community_epidemiology/dc/communicable_disease.html

**If 404:**
1) Use site root and navigate to Public Health → Epidemiology/Communicable Disease:
   - https://www.sandiegocounty.gov/
2) Use CDC MMWR/HAN for clinician guidance and CDC outbreaks for foodborne.

## Sacramento County
**Primary**
- Latest News: https://www.saccounty.gov/news/latest-news/

**If 404:**
1) Sacramento County news landing (root): https://www.saccounty.gov/
2) Substitute CDPH hubs for statewide items; note missing county-specific advisories.

## World
**Primary**
- WHO Disease Outbreak News: https://www.who.int/emergencies/disease-outbreak-news

**If WHO DON is temporarily unavailable:**
1) Use CDC travel notices (high relevance for importation risk): https://wwwnc.cdc.gov/travel/notices

