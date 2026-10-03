# Hüpffrosch

Ein Arcade-Spiel, gebaut als Web-App fürs iPhone. Du bringst fünf Frösche über eine Straße und einen Fluss in die Buchten am oberen Rand.

## Steuerung

- **Wischen** über das Spielfeld: Sprung in diese Richtung
- **Tippen** aufs Spielfeld: ein Sprung nach vorn
- **Steuerkreuz** unter dem Spielfeld
- Am Computer: Pfeiltasten oder WASD, `P` für Pause

## Regeln

- Autos und Lastwagen überfahren dich, im Wasser ertrinkst du. Auf Baumstämmen und Schildkröten kannst du mitfahren.
- Die blassen Schildkröten tauchen gleich ab.
- Pro Leben hast du 30 Sekunden. Übrige Zeit gibt Bonuspunkte.
- Sitzt eine Fliege in einer Bucht, gibt es +200 Punkte, wenn du dort landest.
- Sind alle fünf Buchten voll, kommt das nächste Level. Es wird schneller, ab Level 3 tauchen mehr Schildkröten.
- Bei 5.000 Punkten gibt es ein Extra-Leben, danach alle 10.000 Punkte.

## Aufs iPhone bringen

Die App braucht eine HTTPS-Adresse. Am einfachsten geht das mit GitHub Pages:

1. Im Repository auf GitHub: **Settings → Pages**.
2. Unter „Build and deployment“ als Quelle **Deploy from a branch** wählen, dann den Branch und den Ordner `/ (root)` auswählen und speichern.
3. Nach ein bis zwei Minuten erscheint dort die Adresse, z. B. `https://alfredjdh.github.io/huepffrosch/`.
4. Die Adresse auf dem iPhone in **Safari** öffnen, auf **Teilen** tippen und **Zum Home-Bildschirm** wählen.

Danach startet das Spiel wie eine App im Vollbild, mit eigenem Icon, und läuft nach dem ersten Start auch offline.

Ton gibt es nur, wenn der Stummschalter des iPhones aus ist.

## Dateien

| Datei | Inhalt |
| --- | --- |
| `index.html` | Das komplette Spiel (Grafik, Logik, Steuerung, Sound) |
| `manifest.webmanifest` | App-Name, Icon und Vollbildmodus für den Home-Bildschirm |
| `sw.js` | Offline-Cache. Bei Änderungen am Spiel die Versionsnummer `CACHE` erhöhen. |
| `icons/` | App-Icons |
