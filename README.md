# Wochenliste

Persönliche Wochenplanung als einzelne HTML-Datei: Aufgabenliste mit Serien, Kalender (08:00–22:00) mit Slots und Spielen, Essensplan pro Woche.

## Funktionen

- Aufgaben mit Deadline, Uhrzeit und Dauer, einmalig oder als Serie (mehrere Wochentage)
- Kalender mit Wochenansicht, Drag and Drop zwischen Liste und Tagen, Wochenverlauf
- Slots (z. B. Arbeit, Uni, Training) als Hintergrundblöcke, Termine als reine Kalendereinträge
- Essensplan für Mittag und Abend, pro Woche
- Dunkles Farbschema "Nachtblau", mobil bedienbar

## Nutzen

`index.html` im Browser öffnen. Ohne Datenbank läuft die Seite als lokale Vorschau, Eingaben werden dann nicht gespeichert.

Die Synchronisation nutzt die `db`-Fähigkeit der Claude-Artefakte (`window.claude.use`). Dort liegen die Sammlungen `tasks`, `templates`, `events`, `mealplans` und `meta`. Für den Betrieb außerhalb von Claude muss `init()` auf einen eigenen Speicher (z. B. Firestore oder localStorage) umgestellt werden.

## Aufbau

Alles steckt in `index.html` (CSS und JavaScript inline, keine Build-Schritte). Schriften kommen von Google Fonts: Fraunces, Work Sans, IBM Plex Mono.

## Lizenz

MIT, siehe `LICENSE`.
