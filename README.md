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
2. Einrichten — zwei Wege:
   - **Leicht (empfohlen):** `INIT.md` als Kontext an deine KI geben und „führe mich durch das Setup" sagen. Sie fragt die Grundlagen im Interview ab und füllt Struktur, Kontext-Dateien und `CLAUDE.md` selbst.
   - **Manuell:** `ANLEITUNG.md` öffnen und die Platzhalter (`{{NAME}}`, `{{VAULT_NAME}}` …) von Hand ersetzen — für Nutzung ohne KI-Zugang.
3. Loslegen: erste Notiz in `Tagebuch/`, erstes Projekt in `Projekte/`.

Stufe 2 und 3 sind eigenständige Ordner mit eigener Anleitung — erst dazunehmen, wenn du sie willst.

## Philosophie

> „Vollkommenheit ist erreicht, wenn man nichts mehr weglassen kann." — Saint-Exupéry

Weglassen vor Hinzufügen. Die einfachste funktionierende Lösung gewinnt.

## Lizenz

MIT — frei nutzen, anpassen, weitergeben.
