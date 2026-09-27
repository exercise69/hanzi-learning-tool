# Hanzi-Leiter

Lern-App für 500 chinesische Schriftzeichen (vereinfacht), aufgeteilt in drei Stufen:

- **Stufe 1:** die 100 häufigsten Zeichen
- **Stufe 2:** Zeichen 101–300
- **Stufe 3:** Zeichen 301–500, mit Alltagsvokabular für Reisen in Laos

Funktionen: Karteikarten, Quiz (drei Modi), Lesetexte, die nur Zeichen der jeweiligen Stufe verwenden, und typische chinesische Schilder aus Laos.

## Nutzung

App öffnen: https://exercise69.github.io/hanzi-learning-tool/

1. Einmal mit Internet öffnen.
2. Auf den Startbildschirm legen:
   - iPhone (Safari): Teilen → „Zum Home-Bildschirm“
   - Android (Chrome): Menü ⋮ → „App installieren“ bzw. „Zum Startbildschirm hinzufügen“
3. Danach läuft die App auch ohne Internet.

Der Lernfortschritt wird nur lokal im Browser gespeichert.

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | Die komplette App inkl. Daten und Schriften |
| `sw.js` | Service Worker für den Offline-Modus |
| `manifest.json` | App-Beschreibung für den Startbildschirm |
| `icon-*.png`, `apple-touch-icon.png` | App-Icons |

**Update:** Nach Änderungen an `index.html` in `sw.js` die Konstante `CACHE_VERSION` hochzählen, sonst behalten Handys die alte Fassung im Cache.

## Hinweise

- Die Reihenfolge folgt grob der Zeichenhäufigkeit und ist um Alltagszeichen ergänzt. Es ist keine offizielle HSK-Liste.
- Schriften: Noto Serif SC und Source Sans 3 (SIL Open Font License), als Teilmenge eingebettet.
