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
- **templates/**: Vorlagen für Notizen, Projekte, Daily Notes.
- **Wissensdatenbank/**: Referenzwissen, Kontext-Dateien, Dokumentation.

## System

- Lernschleife: Sektion „Wissen & Erkenntnisse" + sclose.

CLAUDE.md ist **Identität + Arbeitsregeln** der KI.

---

## Arbeitsregeln

### Allgemein
- Schreibstil: knapp, klar, lösungsorientiert. Funktion vor Theorie.
- Code: immer vollständige Dateien/Scripts, keine Snippets.
- API-Keys: niemals im Chat, niemals im Browser-Code — immer server-seitig (siehe Stufe 2).

### Obsidian
- **AI-first Notizen** (damit das Gedächtnis gut abrufbar bleibt):
  - Frontmatter immer: `type:` (projekt/tagebuch/aufgabe/wissen/idee/person/entscheidung), `date:`, `tags:` — bei Projekten und Aufgaben zusätzlich `status:`.
  - `[[Wikilinks]]` für **jede** genannte Person, jedes Projekt, jede Idee, jede Entscheidung — auch wenn die Zieldatei noch nicht existiert.
  - Externe Fakten mit Recency-Marker: `Behauptung (Stand YYYY-MM, quelle.de)`.
- Neue Notiz ohne Platz → `Aufgaben/` oder `Ideen/`.
- Dateien löschen/überschreiben → erst nachfragen.
- Aufgabe verwerfen → löschen (Obsidian sichert sie in `.trash`). Erledigte Aufgaben → `Archiv/`.

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
