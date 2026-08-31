# RabenBrau Website – Vorbereitungsversion

Statische Website für GitHub Pages.

## Wichtig vor Veröffentlichung

Diese Version ist bewusst als **Vorbereitung/Preview** markiert:

- Es gibt **keine `CNAME`-Datei**. Die Domain `rabenbrau.ch` wird dadurch nicht mit diesem Repository verbunden.
- `robots.txt` und der `robots`-Meta-Tag stehen auf `noindex`, damit eine optionale GitHub-Pages-Vorschau möglichst nicht von Suchmaschinen indexiert wird.
- Die definitive Standortadresse muss im Kontakt/Impressum ergänzt werden.
- Das definitive Biersortiment muss vor der Veröffentlichung ergänzt werden.
- Erst beim Go-Live die SEO-Sperre entfernen und danach die Custom Domain konfigurieren.

## GitHub Pages Preview

1. Repository z. B. `rabenbrau-website` erstellen.
2. Alle Dateien aus diesem Ordner in die oberste Ebene des Repositories hochladen.
3. GitHub: **Settings → Pages**.
4. Unter **Build and deployment**: `Deploy from a branch`.
5. Branch `main`, Ordner `/ (root)` auswählen und speichern.
6. Noch **keine Custom Domain** eintragen.

Bei einem GitHub-Konto/Organisation `luma-brauerei` lautet die Vorschau danach typischerweise:

`https://luma-brauerei.github.io/rabenbrau-website/`

## Späterer Go-Live

Erst nachdem die Vorschau vollständig geprüft ist:

1. `meta name="robots"` von `noindex,nofollow` auf `index,follow` ändern.
2. `robots.txt` auf normalen öffentlichen Betrieb umstellen.
3. In GitHub Pages `rabenbrau.ch` als Custom Domain eintragen.
4. Erst danach die DNS-Einträge beim aktuell zuständigen DNS-Anbieter anpassen.
5. Hostpoint-Mail-DNS-Einträge dabei beibehalten.
6. Website und `prost@rabenbrau.ch` testen.

## Struktur

- `index.html` – komplette One-Page-Website
- `assets/css/styles.css` – Layout und Responsive Design
- `assets/js/main.js` – Mobile Navigation
- `assets/images/` – RabenBrau-Bilder aus dem bestehenden Backup
- `assets/icons/favicon.svg` – temporäres Favicon
