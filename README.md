# Voetbalkaart (Pim) op voetbalkaart.cluppieasv33.nl

Eén bestand (`index.html`), geen inlog, geen server. Alles blijft in de browser van de gebruiker (localStorage).

## Eenmalig opzetten (Paul)
1. DNS (bij de beheerder van cluppieasv33.nl): voeg een record toe
   - Type `CNAME`, naam `voetbalkaart`, waarde `pclijten.github.io` (zonder repo-naam, zonder https).
2. GitHub: nieuwe publieke repo `voetbalkaart`. Upload `index.html`, `CNAME`, `robots.txt`, `sitemap.xml` (en later `preview.png`).
3. Settings > Pages: Deploy from a branch > `main` / root. Custom domain: `voetbalkaart.cluppieasv33.nl` > Save.
4. Wacht tot de DNS-check groen is (minuten tot uren), vink dan **Enforce HTTPS** aan.
5. Aanrader: Account settings > Pages > Verify domain (tegen subdomain-overname).
6. Google Search Console: voeg `https://voetbalkaart.cluppieasv33.nl/` toe en dien `sitemap.xml` in.

## Updaten (Pim + Paul)
Pim past `index.html` aan en test lokaal. Paul vervangt het bestand in de repo (Upload files > Commit). Binnen ± 1 minuut live. Terugdraaien kan via History. Verhoog bij grote wijzigingen `lastmod` in `sitemap.xml`.

## Privacy
Geen accounts, geen cookies, geen analytics. Fonts komen van Google Fonts (IP gaat naar Google); zelf hosten kan later.
Eigen origin: localStorage en service worker zijn gescheiden van Cluppie.
