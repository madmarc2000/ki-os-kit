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

## Quickstart (Stufe 1, ~10 Minuten)

1. Ordner `stufe-1-vault/` in Obsidian als Vault öffnen.
2. `00-START-HIER.md` öffnen — sie sagt dir in einem Satz, was zu tun ist.
3. **Einrichten:** Gib deiner KI die Datei `INIT.md` und sag „führe mich durch das Setup". Sie fragt die Grundlagen ab und richtet Struktur, Kontext-Dateien und `CLAUDE.md` selbst ein.
4. Loslegen: schau dir die `BEISPIEL-`Notizen in den Ordnern an, dann lösch sie und leg eigene an.

<details>
<summary>Einrichten ohne KI-Zugang (manuell)</summary>

`ANLEITUNG.md` öffnen und die Platzhalter (`{{NAME}}`, `{{VAULT_NAME}}` …) von Hand ersetzen.
</details>

Stufe 2 und 3 sind eigenständige Ordner mit eigener Anleitung — erst dazunehmen, wenn du sie willst.

## Philosophie

> „Vollkommenheit ist erreicht, wenn man nichts mehr weglassen kann." — Saint-Exupéry

Weglassen vor Hinzufügen. Die einfachste funktionierende Lösung gewinnt.

## Welche KI?

Der Wissens-Layer ist **KI-neutral** — Vault-Struktur, Regeln, Templates und `INIT.md` sind
reine Markdown-Dateien. Jede KI, die Text liest (Claude, ChatGPT, Gemini, lokale Modelle),
kann damit arbeiten: Inhalt in den Chat kopieren und „arbeite nach diesen Regeln" sagen.

`CLAUDE.md` ist nur ein **Beispiel-Dateiname** — die Konvention, die Claude Code automatisch
lädt. Bei anderen Agenten-Tools heißt die Router-Datei anders (`AGENTS.md` für Codex/OpenCode,
`GEMINI.md` für Gemini CLI). Inhaltlich bleibt sie gleich; nur den Namen pro Tool anpassen.

> Damit die KI **autonom** im Vault liest und schreibt (Daily Notes, Notizpflege), braucht sie
> Dateizugriff — also ein Agenten-Tool (Claude Code, Cowork oder das CLI des jeweiligen
> Anbieters), nicht nur einen reinen Web-Chat.

## Lizenz

MIT — frei nutzen, anpassen, weitergeben.
