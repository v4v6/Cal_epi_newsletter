# Certificate note (CDPH)

Some CDPH pages intermittently fail automated HTTPS verification because the server does not always provide the needed intermediate certificate in the TLS handshake.

Workaround used by the pipeline:
- Use `sources/certs/SectigoPublicServerAuthenticationCAOVR36.pem` as an **untrusted intermediate** when validating the leaf certificate, or append it to a custom CA bundle when using low-level fetchers.

If you change or update the cert file, verify it is the real Sectigo intermediate (DER/PEM) and not a placeholder.

