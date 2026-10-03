# Elite UAE Group Website

Produktionsquelle für **eliteuaegroup.ae** und **eliteuaegroup.com**.

## Struktur
- `public/` – veröffentlichte Website
- `wrangler.json` – Cloudflare-Konfiguration
- `.github/workflows/deploy.yml` – automatische Veröffentlichung nach Änderungen auf `main`

## Veröffentlichung
Lokal:
`npx wrangler deploy --config wrangler.json`

Automatisch über GitHub:
Benötigt einmalig das Repository-Secret `CLOUDFLARE_API_TOKEN`.
Danach wird jeder Push auf `main` automatisch zu Cloudflare veröffentlicht.
