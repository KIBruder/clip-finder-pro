# CLIP-FINDER PRO 2.3 — HD QUALITY

## Update
- Standard-Canvas auf 1080 x 1920 (Full HD 9:16) erhöht.
- Export-Auswahl: Full HD 1080p oder Standard HD 720p.
- Angeforderte Video-Bitrate: 10 Mbit/s bei 1080p, 5,5 Mbit/s bei 720p.
- Angeforderte Audio-Bitrate: 192 kbit/s.
- Aufnahme weiterhin mit 30 FPS und synchronisierter Audiospur.
- Service-Worker-Cache auf v5 gesetzt.

## Installation
Im bestehenden GitHub-Repository `clip-finder-pro` die Dateien `index.html` und `sw.js` ersetzen und direkt auf `main` committen. Danach die GitHub-Pages-Seite in Safari neu laden. Falls die alte Version angezeigt wird, Safari-Tab schließen und die Seite erneut öffnen.

## Hinweise
- Die Bitraten sind angeforderte Werte. iOS/Safari und das gewählte Aufnahmeformat können die tatsächliche Encoder-Ausgabe begrenzen.
- 1080p erzeugt eine größere Datei und beansprucht mehr Leistung. Bei Überhitzung, Ruckeln oder Exportabbrüchen 720p verwenden.
- Eine höhere Exportauflösung kann keine Details wiederherstellen, die im Quellvideo fehlen oder bereits komprimiert wurden.
- Die App verarbeitet lokal im Browser; keine kostenpflichtigen APIs.
