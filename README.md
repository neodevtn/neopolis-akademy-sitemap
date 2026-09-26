# Neopolis Akademy — sitemap mirror

This public repository serves a plain-text sitemap for the canonical public pages of [Neopolis Akademy](https://akademy.neodev.click/).

- Public sitemap: `https://neodevtn.github.io/neopolis-akademy-sitemap/sitemap.txt`
- Source: `https://akademy.neodev.click/sitemap-index.xml`
- Format: UTF-8, one fully qualified canonical URL per line
- Scope: public indexable pages only; authenticated training, administration, account, API, search-query, and assessment routes are rejected

A deterministic GitHub Actions workflow refreshes the mirror every six hours and can also be run manually. It validates the host, protocol, uniqueness, URL count, and private-path exclusions before committing an update.
