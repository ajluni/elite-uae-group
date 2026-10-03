# Elite UAE Group Website

Produktionsquelle für **eliteuaegroup.ae** und **eliteuaegroup.com**.

## Struktur
- `public/` – veröffentlichte Website
- `wrangler.json` – Cloudflare-Konfiguration

## Veröffentlichung
Die Website ist direkt mit **Cloudflare Workers Builds** und dem GitHub-Repository `ajluni/elite-uae-group` verbunden.

- Produktionszweig: `main`
- Änderungen auf `main` stoßen automatisch einen Cloudflare-Build und eine Veröffentlichung an.
- Lokal bleibt eine manuelle Veröffentlichung mit `npx wrangler deploy --config wrangler.json` möglich.

Es wird kein separates GitHub-Actions-Secret für Cloudflare benötigt.
