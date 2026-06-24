# KI-OS Kit

Ein Bausatz, um ein persönliches **KI-Betriebssystem auf Basis von Obsidian** nachzubauen:
strukturiertes „zweites Gehirn", eine `CLAUDE.md` als Router/Identität für die KI, klare
Arbeitsregeln und ein optionaler autonomer Agent.

Das Kit ist in drei Stufen aufgebaut. **Du nimmst nur, was du brauchst.**

| Stufe | Inhalt | Voraussetzung | Server? |
|-------|--------|---------------|---------|
| **1 — Vault + Methodik** | Ordnerstruktur, `CLAUDE.md`, Regeln, Templates | Obsidian (gratis) + Sync | **nein** |
| **2 — Agent** | Autonomer Task-Runner, Secrets-Konzept | + Always-On-Rechner + KI-Account | nein |
| **3 — Dienste** | Eigene Web-Dienste, Reverse Proxy | + eigener VPS + Domain | ja |

> Server brauchst du **erst ab Stufe 3** — und dann ist es *dein* Server, nicht der des Autors.

## Herunterladen

**Mit git** (Terminal):

```
git clone https://github.com/madmarc2000/ki-os-kit.git
```

**Ohne git** (kein Terminal nötig): oben auf den grünen **Code**-Knopf → **Download ZIP** → entpacken.

Danach `stufe-1-vault/` in Obsidian als Vault öffnen — weiter geht's unten.

## Welche KI brauchst du?

Entscheidend ist, ob deine KI **Dateien schreiben** kann:

- **KI-Tool mit Dateizugriff** (Claude Code, Cowork, Gemini CLI, Codex CLI): führt das Interview *und* legt die Dateien selbst an. Vollautomatisch.
- **Reiner Web-Chat** (Gemini, ChatGPT, Claude im Browser): kann **keine** Dateien schreiben. Er führt dich durchs Interview und gibt dir die fertigen Inhalte aus — **kopieren musst du selbst**. Behauptet ein Web-Chat, er habe Dateien angelegt, stimmt das nicht: prüf im Dateiexplorer nach.
- **Kein KI-Zugang**: der manuelle Weg (`_setup/ANLEITUNG.md`).

Der Wissens-Layer selbst ist **KI-neutral** — Struktur, Regeln und Templates sind reines Markdown, das jede KI lesen kann. `CLAUDE.md` ist nur ein Beispiel-Dateiname (Claude Code lädt ihn automatisch); bei anderen Agenten heißt die Router-Datei `AGENTS.md` (Codex/OpenCode) oder `GEMINI.md` (Gemini CLI). Inhaltlich gleich, nur der Name ändert sich.

## Loslegen

Sobald `stufe-1-vault/` in Obsidian offen ist, führt dich die Datei **`00-START-HIER.md`** Schritt für Schritt durch die Einrichtung: Interview, Obsidian-Einstellungen, erste Notizen. Mehr musst du nicht wissen, um anzufangen.

Stufe 2 und 3 sind eigenständige Ordner mit eigener Anleitung — erst dazunehmen, wenn du sie willst.

## Philosophie

> „Vollkommenheit ist erreicht, wenn man nichts mehr weglassen kann." — Saint-Exupéry

Weglassen vor Hinzufügen. Die einfachste funktionierende Lösung gewinnt.

## Lizenz

MIT — frei nutzen, anpassen, weitergeben.
