# Chemin Légal

Source of [cheminlegal.com](https://cheminlegal.com): a free French-language guide to the legal routes for studying, training and working abroad, the main scholarships, and the scams to avoid.

## How it's built

- One static page: `index.html` (HTML, CSS and JavaScript, no build step).
- The routes, scholarships and deadlines live in the `ROUTES`, `SCHOLARSHIPS` and `DEADLINES` arrays in the page's script. Update those to change the content.
- Hosted on Cloudflare Pages: every push to `main` goes live automatically.

## Keeping it accurate

Every fact on the page is dated. Re-check each route and scholarship against its official link at least every 3 months, and update the "Dernière vérification" date in the footer and the hero.

## Visitor statistics

Click tracking is wired in through `track()` and reports to GoatCounter once the script tag in `<head>` is uncommented with the account code. Tracked events: profile filter (`profil/...`), level filter (`niveau/...`), official links (`lien-officiel/...`) and the WhatsApp button (`whatsapp-bientot`).
