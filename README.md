# Nizza & Côte d'Azur 2026

Reiseführer-Website für einen Kurztrip Do 3.09.–So 7.09.2026 (Nizza/Cagnes-sur-Mer/Antibes/Cannes/Umgebung), im gleichen Aufbau wie [stephandel.github.io/fuerteventura-2026](https://stephandel.github.io/fuerteventura-2026) — als Test, ob sich diese Struktur auf ein anderes Reiseziel übertragen lässt.

Einzige Datei: `index.html` (Single-Page-App, kein Build-Schritt nötig).

## Lokal ansehen

```
python3 -m http.server 8000
```
dann `http://localhost:8000` öffnen.

## Noch offen (nicht von Claude erledigt — braucht deine Entscheidung)

Dieses Repo wurde bewusst **nicht** zu GitHub gepusht und es wurde **kein** Remote-Repo angelegt. Falls gewünscht:

1. `gh repo create nizza-2026 --public --source=. --remote=origin` (oder privat mit `--private`)
2. `git push -u origin main`
3. Auf GitHub: Settings → Pages → Deploy from branch → `main` / `/ (root)` aktivieren
4. Danach ist die Seite unter `https://<dein-username>.github.io/nizza-2026/` erreichbar

## Scope-Cuts gegenüber der Fuerteventura-Vorlage

- **Keine eigenen Fotos** — aus Zeitgründen (Reise beginnt in 2 Tagen) wurden Kartenbilder durch farbige CSS-Kacheln mit Emoji ersetzt statt echte Fotos zu recherchieren/laden.
- **Keine Favoriten/Ausblenden/Sortier-Interaktivität** — die FV-Seite hat pro Karte Favoriten-Herz, Ausblenden-Button und Sortier-Dropdowns mit JS-Logik. Hier bewusst weggelassen, um die Zeit in Recherche statt Interaktions-Feinschliff zu stecken. Die Kartenstruktur (Bewertung, Entfernung, Google-Maps-Link, Quelle+Stand) ist aber identisch übernommen.
- **Kein Unterkunfts-/Kostenvergleich** — die Großmutter wohnt vor Ort, es gibt keine Buchungsentscheidung zu treffen. Das war der größte strukturelle Unterschied zur 13-Nächte-FV-Logik.
- **Kalender ist viel terminkritischer** — bei FV ist der Reisezeitraum 13 Nächte lang und relativ tolerant gegenüber einzelnen ausfallenden Terminen. Hier ist die Reise auf 5 feste Tage gelegt, jeder Wochentag zählt (z. B. Puces de Nice hat sonntags zu — direkt am Abreisetag).
