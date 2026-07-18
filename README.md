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

## Sprachen

Zweisprachig DE/EN über einen Toggle im Header (client-seitig, `data-i18n`).
Persistenz in `localStorage`, Auto-Erkennung der Browsersprache.

## Inhalte (echt, aus den Projekt-Verzeichnissen)

- **Code Tycoon** — 2D-Software-Dev-/Wirtschaftssimulation, live auf Steam
  ([app/4347780](https://store.steampowered.com/app/4347780/), Demo: app/4417500).
- **Code Rescue** — interaktives Programmier-Lernspiel (3D), in Entwicklung, gebaut mit PHPolygon.
- **PHPolygon** ist eine **eigene** GitHub-Org: https://github.com/phpolygon/phpolygon (MIT).
- Studio-Org: https://github.com/mennen-games · Kontakt: hmennen90@gmail.com

## Struktur

```
index.html                 # Hauptseite (Hero, Spiele, Engine, Über uns) + i18n
404.html                   # Fehlerseite
assets/favicon.svg         # App-Mark (M mit Caret)
.github/workflows/deploy.yml
```

## Optional / später

- Eigene Domain (CNAME) statt `mennen-games.github.io`.
- Screenshots / OG-Image für Social-Previews.
