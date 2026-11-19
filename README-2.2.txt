# CLIP-FINDER PRO 2.2

## Änderungen
- Anzahl der Clip-Vorschläge skaliert mit der Videolänge: 3 bis 20 Vorschläge.
- Lokale Wiederholungshistorie verhindert beim erneuten Import derselben Datei möglichst dieselben Zeitbereiche.
- Audio-Ranking kombiniert Spitzenpegel und durchschnittliche Lautstärke im Umfeld. Das ist eine Heuristik, keine semantische KI und keine echte Viralitätsprognose.
- Hochformat-Canvas auf 720 x 1280 erhöht.
- Hook-Auswahl nach Funny, WTF, Epic, Fail/Rage, Mystery und Streamer-Reaktion.
- Hook-Wechsel ohne direkte Wiederholung; doppeltes Hook-Eingabefeld entfernt.
- Service-Worker-Cache auf v4 gesetzt.

## Installation
Nur index.html und sw.js im bestehenden GitHub-Repository ersetzen und direkt auf main committen. Danach GitHub-Pages-App in Safari neu laden.

## Grenzen
- Die Analyse prüft weiterhin viersekündige Audiofenster im gewählten Zeitabstand. Ereignisse zwischen Stichproben können übersehen werden.
- Die Wiederholungshistorie verwendet Dateiname, Größe, lastModified und Laufzeit. Umbenannte oder neu exportierte Dateien können als neue Quelle gelten.
- 720x1280 verbessert die Canvas-Ausgabeauflösung. Die endgültige Encoderqualität hängt weiterhin von iOS/Safari und MediaRecorder ab; es ist kein verlustfreies Remux der Originaldatei.
- Alles bleibt lokal im Browser; keine kostenpflichtigen APIs.
