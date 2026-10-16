# ANT1 Zuladungs-Demo (synthetisch)

**Seite:** https://projektw2.github.io/ant1-web-demo/

Browser-Demo zur Zuladungsschätzung beim OLIVE ANT1: 3D-Modell drehen und zoomen,
Zuladung 0–1500 g wählen, eine Beschleunigungs- und Bremsfahrt abspielen,
synthetische IMU-, Raddrehzahl- und Motorstromwerte ansehen und eine exemplarische
Least-Squares-Schätzung ablesen. Läuft vollständig im Browser, ohne Backend.

> **Alle Werte sind synthetisch** (vereinfachtes 1D-Modell mit angenommenen
> Parametern). Keine Messung am realen ANT1 und keine validierte Genauigkeit.

**Inspiration:** https://maxsikorski.github.io/jumpstart-3d/

## Inhalt dieses Repositories

Dieses Repository enthält nur die **automatisch erzeugte Build-Ausgabe**. Der Quellcode
liegt in einem privaten Repository. Nach jedem Merge auf dessen `main` testet GitHub
Actions die Demo und ersetzt den Inhalt hier durch genau den getesteten Build:

- `index.html`, `assets/` (minifiziertes JavaScript und CSS, ohne Sourcemaps)
- `models/` (STL-Meshes des ANT1-Modells)
- `version.json` (Quell-Commit und Build-Zeitpunkt)
- `.nojekyll`, diese README

GitHub Pages liefert den Branch `main` aus. Änderungen direkt in diesem Repository
werden beim nächsten Deployment überschrieben.

## Stand (16.10.2026)

Noch **kein Deployment**. Repository und Pages sind eingerichtet, das Token für den
automatischen Push wartet auf die Freigabe durch die Organisation. Bis dahin zeigt die
Seite nur diese README; danach ersetzt sie der erste Build.
