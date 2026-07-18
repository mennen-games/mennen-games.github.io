# mennen-games.github.io

Die offizielle Website von **Mennen Games** — ein unabhängiges Spielestudio.
Kommerzielle Spiele, angetrieben von [PHPolygon](https://github.com/mennen-games), unserer Open-Source-Engine in PHP.

🔗 **Live:** https://mennen-games.github.io

## Stack

- Statische Single-Page-Site (plain HTML/CSS/JS, kein Build-Tool)
- Deploy über **GitHub Actions** → GitHub Pages (`.github/workflows/deploy.yml`)
- Design nach dem Mennen-Games-Brand-Guide (Corporate Identity):
  - Farben: Deep Petrol `#0A1217`, Warm Off-White `#F2F2EB`, adaptiver Akzent Mint `#4DD9BF` / Gold `#F5D475`
  - Schriften: Inter (Display/Text) + Inconsolata (Mono/Terminal)
  - Signatur: selbst-tippende Wortmarke mit Terminal-Caret, Code-Stream, Scanlines

## Lokal ansehen

Einfach `index.html` im Browser öffnen — oder ein kleiner Server:

```bash
python -m http.server 8000
# → http://localhost:8000
```

## Deployen

Jeder Push auf `main` löst den Workflow aus und veröffentlicht die Seite automatisch.

## Struktur

```
index.html                 # Hauptseite (Hero, Spiele, Engine, Über uns)
404.html                   # Fehlerseite
assets/favicon.svg         # App-Mark (M mit Caret)
.github/workflows/deploy.yml
```

## Noch offen / Platzhalter

- Spiel-Beschreibungen, Genres und Preise für **Code Tycoon** und **Code Rescue** sind Platzhalter.
- Kontakt-Mailadresse `hallo@mennengames.dev` ggf. anpassen.
- Optional: eigene Domain (CNAME) statt `mennen-games.github.io`.
