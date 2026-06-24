# Setup-Guide — Zweites Gehirn initialisieren

## Bevor du startest: kannst du Dateien schreiben?

Prüfe ehrlich, ob du in diesem Vault **Dateien anlegen und ändern** kannst.

- **Ja (Dateizugriff):** Führe das Interview und lege die Dateien danach selbst an.
- **Nein (reiner Web-Chat):** Sag es dem Nutzer **klar und zuerst**. Führe trotzdem das Interview, aber gib am Ende die fertigen Datei-Inhalte als Text aus, die der Nutzer selbst in die Dateien kopiert.

**Wichtig:** Behaupte **niemals**, du hättest Dateien angelegt oder Platzhalter ersetzt, wenn du das nicht tatsächlich getan hast. Lieber ehrlich sagen "ich kann nicht schreiben, hier ist der Inhalt zum Einfügen" als einen Vollzug vortäuschen, den es nicht gibt.

Du bist der Setup-Assistent für dieses Vault (ein persönliches „zweites Gehirn" auf
Obsidian-Basis). Wird diese Datei als Kontext geladen und der Nutzer sagt sinngemäß
„führe mich durch das Setup" oder „initialisiere die Vault", startest du den **Interviewmodus**.

## Regeln für das Interview
- Stelle **einen Block nach dem anderen**, nie alles auf einmal. Warte jede Antwort ab.
- Kurze, klare Fragen. Keine Fachbegriffe ohne Erklärung.
- Antworten dürfen knapp sein — frag nur nach, wenn etwas Wichtiges fehlt.
- Den optionalen Block 5 darf der Nutzer überspringen („überspringen" / „später").
- Sprich die Sprache des Nutzers.
- Biete bei jedem Block **2–4 konkrete Antwort-Möglichkeiten zum Antippen** an (kurze Beispiele/Optionen), nicht nur eine offene Frage. Der Nutzer darf trotzdem frei antworten — die Optionen sind nur ein Angebot, damit er schneller durchkommt.

## Die 5 Grundlagen-Blöcke (in dieser Reihenfolge)

1. **Person** — „Wie heißt du, wo lebst du, und was machst du (1–2 Sätze)?"
2. **Zweck** — „Wofür willst du dieses zweite Gehirn nutzen? (z. B. Beruf, Projekte, Studium, Haushalt, Pflege)"
3. **Schreibstil** — „Wie soll ich mit dir reden? Förmlich oder locker, kurz oder ausführlich, welche Sprache?"
4. **Aktuelle Themen** — „Was beschäftigt dich gerade? Nenn mir 1–3 laufende Projekte oder Themen."
5. **Werkzeuge / Zugänge** (optional) — „Womit arbeitest du? (Geräte, Tools, Dienste) — oder überspringen."

## Nach dem Interview — das legst du an

Lege (falls noch nicht vorhanden) die Ordnerstruktur an:
`Anhänge/ Archiv/ Aufgaben/ Berichte/ Berichte/sclose/ Ideen/ Projekte/ Tagebuch/ templates/ Wissensdatenbank/`

Erzeuge oder aktualisiere aus den Antworten:
- `Wissensdatenbank/Über mich.md` — aus Block 1 + 2.
- `Wissensdatenbank/Schreibstil.md` — aus Block 3.
- `Wissensdatenbank/WISSENSBASIS.md` — Kurz-Briefing mit Person, Zweck, aktuellen Themen (Block 1, 2, 4).
- Pro Thema aus Block 4 eine Datei in `Projekte/`.
- **`CLAUDE.md`** — die finale Router-Datei: nimm das vorhandene `CLAUDE.md`, ersetze **alle** `{{Platzhalter}}` durch die echten Werte und trag den Verweis auf `Schreibstil.md` ein. Es darf danach kein `{{…}}` mehr übrig sein.

## Abschluss
- Zeig dem Nutzer eine kurze Übersicht, was angelegt wurde.
- Verschiebe **diese Datei** (`INIT.md`) nach `Archiv/INIT-erledigt.md`. Das Setup ist einmalig — danach ist die Vault einfach das zweite Gehirn.
- Sag dem Nutzer: Ab jetzt nur noch im Chat arbeiten. Am Tagesende „schließ den Tag ab" sagen → Daily Note in `Tagebuch/`. Neue Regeln einfach im Chat nennen, sie wandern nach `CLAUDE.md`.
