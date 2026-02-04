# TLS / access limitations (operational note)

Some official public health sites may intermittently fail automated retrieval due to:
- missing intermediate certificate delivery during TLS handshake (notably seen on some SharePoint-backed CDPH paths)
- bot protection / Cloudflare blocks on certain county sites
- redirects to HTTP-only endpoints

Policy for the newsletter:
- Do not fabricate missing numbers.
- Use alternative official sources when available (e.g., SFDPH PDF advisories; CDC MMWR; CDC outbreak pages).
- Record gaps clearly in **Data Notes & Caveats**.
