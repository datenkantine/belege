# Belege & Materialien

Stabile Quellen- und Material-Kurzlinks für Veröffentlichungen der
Dr. Malcher Unternehmensberatung GmbH. Ausgeliefert über GitHub Pages unter
der Domain aus der Datei `CNAME` (Standard: `quellen.dr-malcher.de`).

Zweck: In Publikationen wird immer auf eine **eigene, stabile** Adresse zitiert
(z. B. `quellen.dr-malcher.de/gvv/westerheim`). Wohin diese intern zeigt, lässt
sich jederzeit ändern, ohne dass eine gedruckte Fußnote ungültig wird.

## Inhalt

- `CNAME` — die Custom Domain (eine Zeile). Bei Bedarf hier die gewünschte
  (Sub-)Domain eintragen.
- `.nojekyll` — sorgt für rein statische Auslieferung (kein Jekyll-Build).
- `robots.txt` + `noindex` — hält die Beleg-/Redirect-Seiten aus Suchindizes.
- `index.html` — interne, nicht verlinkte Übersicht aller Kurzlinks.
- `404.html` — Fallback.
- `gvv/westerheim/index.html` — Beispiel-Weiterleitung (Meta-Refresh) auf eine
  externe Quelle.

## Neuen Beleg anlegen

**Variante A — Weiterleitung auf eine fremde Quelle**
1. Neuen Ordner anlegen, z. B. `gvv/musterstadt/`.
2. Darin `index.html` aus `gvv/westerheim/index.html` kopieren.
3. Die beiden Ziel-URLs (`canonical` und `http-equiv="refresh"`) auf die neue
   Adresse setzen, Text anpassen.
4. Zitiert wird dann `quellen.dr-malcher.de/gvv/musterstadt`.

**Variante B — eigenes Dokument selbst hosten (robusteste Lösung)**
1. PDF direkt ins Repo legen, z. B. `gvv/westerheim-praesentation.pdf`.
2. Zitiert wird `quellen.dr-malcher.de/gvv/westerheim-praesentation.pdf`.
   (Stabil, versioniert, vollständig in eigener Hand.)

Hinweis: Das Repository ist öffentlich (Voraussetzung für kostenlose Pages).
Nur ablegen, was öffentlich sein darf — keine personenbezogenen Daten.
