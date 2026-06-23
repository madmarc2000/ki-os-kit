# Vault Context — {{VAULT_NAME}}

Dieses Vault ist das zweite Gehirn von {{NAME}}.

> **Kompakte Wissensbasis:** [[Wissensdatenbank/WISSENSBASIS]] — bei jeder neuen Session
> **zuerst** lesen, danach gezielt nachladen.

## Über mich

{{NAME}}, {{ORT}}. {{KONTEXT}}

Ausführliches Profil: [[Wissensdatenbank/Über mich]]

---

## Vault-Struktur

- **Anhänge/**: Bilder, PDFs, Medien. Obsidian speichert hier automatisch.
- **Archiv/**: Abgeschlossene Projekte, inaktive Notizen.
- **Aufgaben/**: To-Dos, offene Punkte, Checklisten.
- **Berichte/**: Zusammenfassungen, Session-Protokolle, sclose-Outputs.
- **Ideen/**: Lose Gedanken, Konzepte ohne konkretes Projekt. Tag: `#idee`
- **Projekte/**: Aktive Projekte mit Ziel und Enddatum. Eine .md pro Projekt.
- **Tagebuch/**: Tägliche Einträge. Format: `YYYY-MM-DD.md`. Tags: `#frage` / `#erledigt` / `#idee`
- **Trash/**: Verworfene Notizen. Soft-Delete-Puffer — NICHT für Erledigtes (das → `Archiv/`). Älter als 30 Tage darf endgültig gelöscht werden.
- **templates/**: Vorlagen für Notizen, Projekte, Daily Notes.
- **Wissensdatenbank/**: Referenzwissen, Kontext-Dateien, Dokumentation.

## System-Bausteine (modular)

- **Skills/** — abrufbare Prozesse, eine .md pro Skill. Bei neuer Aufgabe passenden Skill laden; fehlt einer, neu anlegen nach gleichem Schema.
- **GOVERNANCE.md** — Ampelsystem (grün/gelb/rot): was die KI autonom darf, was nur mit Review, was nie.
- Lernschleife: Sektion „Wissen & Erkenntnisse" + sclose.

CLAUDE.md ist **Identität + Router**: Prozessdetails leben in `Skills/`, Regeln in `GOVERNANCE.md`.

---

## Arbeitsregeln

### Allgemein
- Schreibstil: knapp, klar, lösungsorientiert. Funktion vor Theorie.
- Code: immer vollständige Dateien/Scripts, keine Snippets.
- API-Keys: niemals im Chat, niemals im Browser-Code — immer server-seitig (siehe Stufe 2).

### Obsidian
- `[[Wikilinks]]` für interne Verknüpfungen.
- YAML-Frontmatter: `tags`, `status` (aktiv/abgeschlossen/pausiert), `date`.
- Neue Notiz ohne Platz → `Aufgaben/` oder `Ideen/`.
- Dateien löschen/überschreiben → erst nachfragen.
- Backup vor Änderung: Kopie nach `bak/` im Vault-Root, Schema `<Ordner>__<datei>.BAK-YYYY-MM-DD-HHMM.md`. Bei jedem Lauf: `bak/`-Dateien älter als 7 Tage löschen.
- Aufgabe verwerfen → nach `Trash/`. Erledigte Aufgaben → `Archiv/`, nicht Trash.

### Wenn ich sage „merk dir das"
→ relevante Datei in `Wissensdatenbank/` aktualisieren und die Änderung benennen.

### Wenn ich „zusammenfassung" schreibe (oder `#sclose`)
→ sclose-Output erstellen:

```
## sclose — [Projektname]
**Datum:** YYYY-MM-DD

**Entscheidungen:**
- [Entscheidung] → [Ein-Satz-Begründung]

**Offene Punkte / Nächste Schritte:**
- [ ] [Schritt]

**Stand:** [Ein Satz]
```

Speichern in `Berichte/sclose/YYYY-MM-DD.md` (oder `…-[projektname].md`).
Kein Diskussionsverlauf, keine KI-Argumente — nur Fakten und Entscheidungen.

---

## Session-Routinen

- **Session-Start:** Prüfe neue `#frage`-Tags in `Tagebuch/`. Zeige offene Punkte aktiver Projekte, wenn relevant.
- **„Wo war ich?":** Letzte 2–3 Tagebuch-Einträge + aktive Projekt-Dateien → kurzes Briefing, kein Fließtext.
- **Session-Ende:** sclose wie oben.

---

## Technische Prinzipien

- **One-tap-Prinzip:** Jeder Workflow minimiert manuelle Schritte.
- **Eine Quelle pro Fakt**, keine Duplikate.
- **Einfachste funktionierende Lösung gewinnt.**

---

## Wissen & Erkenntnisse

Persistentes Gedächtnis zwischen Sessions. Die KI lernt nicht dauerhaft — relevante
Erkenntnisse, Entscheidungen und neues Wissen werden hier abgelegt.

**Format pro Eintrag:** `- [YYYY-MM-DD] [Thema]: [Erkenntnis in 1-2 Sätzen]`

**Regeln:**
- Kein Gesprächsverlauf — nur Fakten, Entscheidungen, Erkenntnisse.
- Max 2 Sätze pro Eintrag. Neue Einträge unten anhängen.
- Am Session-Ende fragt die KI: „Was soll ich aus diesem Gespräch festhalten?"

**Einträge:**
- [YYYY-MM-DD] Beispiel: Hier kommt deine erste Erkenntnis rein.

---

## Handlungsprinzip: Weglassen vor Hinzufügen

> „Vollkommenheit ist nicht erreicht, wenn man nichts mehr hinzufügen, sondern wenn man
> nichts mehr weglassen kann." — Saint-Exupéry

- Vor jeder Ergänzung prüfen: lässt sich das Problem durch **Weglassen** lösen?
- Kein Teil, keine Datei, kein Schritt ohne klaren Zweck.
- Bei Vorschlägen: erst reduzieren, dann optimieren.

## Arbeits-Workflow für neue Projekte/Features

Verbindliche Reihenfolge — kein Schritt überspringen:

1. **Diskutieren** — Optionen, Vor-/Nachteile. Noch nichts bauen.
2. **Entscheiden** — Entscheidungen festhalten (sclose-Format wenn sinnvoll).
3. **Mockup** — Low-Effort-Prototyp zum Validieren (statisches HTML, Skizze, Dummy-Daten).
4. **Bauen** — erst nach Freigabe des Mockups.

---

## Erweiterungen

- **Agent (autonomes Ausführen):** siehe `../stufe-2-agent/`.
- **Eigene Web-Dienste (VPS):** siehe `../stufe-3-dienste/`.
