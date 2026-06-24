# Obsidian einrichten

Diese Einstellungen schalten das Vault-Layout „scharf" — ohne sie funktioniert der Vault
zwar, aber Anhänge, Vorlagen und Tagesnotizen landen am falschen Ort. Einmal klicken, fertig.
(Eine KI kann das in Stufe 1 nicht für dich tun — die Einstellungen liegen in `.obsidian/`,
nicht in den Notizen.)

## Einstellungen

1. **Anhänge-Speicherort** — Einstellungen → Dateien & Links → „Standardspeicherort für neue
   Anhänge" → `Anhänge`. Sonst landen eingefügte Bilder im Wurzelverzeichnis.
2. **Anhänge aus Graph & Suche raushalten** — Dateien & Links → „Ignorierte Dateien" →
   `Anhänge/` eintragen.
3. **Vorlagen** — Einstellungen → Core-Plugins → „Vorlagen" aktivieren → Vorlagen-Ordner =
   `templates`. Macht die mitgelieferten Templates per Hotkey nutzbar.
4. **Tägliche Notizen** — Core-Plugins → „Tägliche Notizen" aktivieren → Ort = `Tagebuch`,
   Datumsformat = `YYYY-MM-DD`, Vorlage = `templates/tagebuch`.
5. *(optional)* **Gelöschte Dateien** — Dateien & Links → auf „In Papierkorb (Obsidian, .trash)
   verschieben" lassen. Kein eigener Trash-Ordner nötig.
6. *(optional, Community-Plugin)* **Dataview** — installieren für Abfragen wie „alle offenen
   `#aufgabe`".

## Die Ordner — wofür sie da sind

- **Aufgaben/** — offene To-dos. Format siehe `BEISPIEL-aufgabe.md`.
- **Projekte/** — laufende Vorhaben mit Ziel und Status. Siehe `BEISPIEL-projekt.md`.
- **Tagebuch/** — Tagesnotizen, eine pro Tag (`YYYY-MM-DD.md`). Siehe `BEISPIEL.md`.
- **Ideen/** — schnelle Einfälle, roh festgehalten, später ausgearbeitet.
- **Wissensdatenbank/** — Referenzwissen, das du nachschlägst. Siehe `BEISPIEL-wissen.md`.
- **Skills/** — abrufbare Prozesse für die KI, eine `.md` pro Skill.
- **Berichte/** — generierte Zusammenfassungen und Auswertungen.
- **Anhänge/** — Bilder, PDFs, eingebettete Dateien. Füllt sich automatisch, sobald
  Einstellung 1 gesetzt ist — hier nichts von Hand ablegen.
- **Archiv/** — abgeschlossene Projekte und Notizen, die du behalten, aber nicht mehr aktiv
  sehen willst. Startet leer.
