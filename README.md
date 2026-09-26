# Neopolis Akademy — sitemap mirror

This public repository serves a plain-text sitemap for the canonical public pages of [Neopolis Akademy](https://akademy.neodev.click/).

- Public sitemap: `https://raw.githubusercontent.com/neodevtn/neopolis-akademy-sitemap/main/sitemap.txt`
- Source: `https://akademy.neodev.click/sitemap-index.xml`
- Freshness status: `https://raw.githubusercontent.com/neodevtn/neopolis-akademy-sitemap/main/status.json`
- Format: UTF-8, one fully qualified canonical URL per line
- Scope: public indexable pages only; every route must match the explicit public allowlist. Authenticated training, administration, account, API, diagnostic, application, search-query, and assessment routes are rejected.

A deterministic GitHub Actions workflow refreshes the mirror every six hours and can also be run manually. It retries transient source failures, validates the host, protocol, uniqueness, URL count, and public route allowlist, then records the generation timestamp and SHA-256 checksum. A failed refresh opens or updates a monitoring issue; the next successful run closes it.
