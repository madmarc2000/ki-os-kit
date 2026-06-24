# KI-OS Kit

Ein Bausatz, um ein persönliches **KI-Betriebssystem auf Basis von Obsidian** nachzubauen: strukturiertes "zweites Gehirn", eine `CLAUDE.md` als Router/Identität für die KI, klare Arbeitsregeln und ein optionaler autonomer Agent.

Das Kit ist in drei Stufen aufgebaut. **Du nimmst nur, was du brauchst.**

| Stufe | Inhalt | Voraussetzung | Server? |
|-------|--------|---------------|---------|
| **1 — Vault + Methodik** | Ordnerstruktur, `CLAUDE.md`, Regeln, Templates | Obsidian (gratis) + Sync | **nein** |
| **2 — Agent** | Autonomer Task-Runner, Secrets-Konzept | + Always-On-Rechner + KI-Account | nein |
| **3 — Dienste** | Eigene Web-Dienste, Reverse Proxy | + eigener VPS + Domain | ja |

> Server brauchst du **erst ab Stufe 3** — und dann ist es *dein* Server, nicht der des Autors.

## Sofort starten — ohne Download, ohne KI

**→ [Vault jetzt im Browser bauen](https://madmarc2000.github.io/ki-os-kit/)**

Klick den Link, beantworte fünf kurze Fragen, lade deinen fertigen Vault als ZIP, entpack ihn (egal wohin) und öffne ihn in Obsidian. **Fertig.** Ordner, Regeln, Profil *und* die Obsidian-Einstellungen sind schon eingerichtet — kein Terminal, keine KI, kein Vorwissen.

Die Seite lädt einmal und läuft danach komplett in deinem Browser. Deine Eingaben werden **nicht hochgeladen** — wichtig, wenn du sensible Dinge notierst. Am Computer öffnen (Mac oder PC), nicht am Handy.

## Das ganze Kit holen

Brauchst du nur, wenn du **Stufe 2 oder 3** willst oder den Bausatz **offline** nutzen möchtest (die `setup.html` liegt auch lokal im Kit und läuft dann ganz ohne Internet).

**Mit git** (Terminal):

```
git clone https://github.com/madmarc2000/ki-os-kit.git
```

**Ohne git** (kein Terminal nötig): oben auf den grünen **Code**-Knopf → **Download ZIP** → entpacken.

## Mit einer KI (Alternative zum Bausatz)

Wenn du ohnehin ein KI-Tool nutzt: Öffne `stufe-1-vault/` in Obsidian, gib der KI die Datei `_setup/INIT.md` und sag "führe mich durch das Setup". `00-START-HIER.md` erklärt jeden Schritt. Was deine KI dafür können muss, steht im nächsten Abschnitt.

## Welche KI brauchst du?

*(Nur wichtig, wenn du den KI-Weg gehst — der Bausatz oben braucht keine KI.)*

Entscheidend ist, ob deine KI **Dateien schreiben** kann:

- **KI-Tool mit Dateizugriff** (Claude Code, Cowork, Gemini CLI, Codex CLI): führt das Interview *und* legt die Dateien selbst an. Vollautomatisch.
- **Reiner Web-Chat** (Gemini, ChatGPT, Claude im Browser): kann **keine** Dateien schreiben. Er führt dich durchs Interview und gibt dir die fertigen Inhalte aus — **kopieren musst du selbst**. Behauptet ein Web-Chat, er habe Dateien angelegt, stimmt das nicht: prüf im Dateiexplorer nach.
- **Kein KI-Zugang**: der manuelle Weg (`_setup/ANLEITUNG.md`).

Der Wissens-Layer selbst ist **KI-neutral** — Struktur, Regeln und Templates sind reines Markdown, das jede KI lesen kann. `CLAUDE.md` ist nur ein Beispiel-Dateiname (Claude Code lädt ihn automatisch); bei anderen Agenten heißt die Router-Datei `AGENTS.md` (Codex/OpenCode) oder `GEMINI.md` (Gemini CLI). Inhaltlich gleich, nur der Name ändert sich.

## Stufe 2 und 3

Eigenständige Ordner mit eigener Anleitung — erst dazunehmen, wenn du sie willst.

## Philosophie

> "Vollkommenheit ist erreicht, wenn man nichts mehr weglassen kann." — Saint-Exupéry

Weglassen vor Hinzufügen. Die einfachste funktionierende Lösung gewinnt.

## Lizenz

MIT — frei nutzen, anpassen, weitergeben.
