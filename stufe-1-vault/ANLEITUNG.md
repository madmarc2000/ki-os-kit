# Anleitung — Stufe 1 einrichten

## 1. Obsidian installieren
[obsidian.md](https://obsidian.md) — kostenlos, lokal. Diesen Ordner (`stufe-1-vault/`)
als Vault öffnen: *Vault öffnen → Ordner wählen*.

## 2. Sync wählen (eine Option)
- **iCloud / OneDrive / Dropbox** — Vault-Ordner ins Cloud-Verzeichnis legen. Gratis, einfach.
- **Obsidian Sync** — [obsidian.md/sync](https://obsidian.md/sync), ~4–8 €/Monat, verschlüsselt.
- **Git** — für Technik-affine. Versionierung inklusive.

## 3. Platzhalter ersetzen
Such-und-Ersetze in `CLAUDE.md` (und überall sonst) folgende Werte:

| Platzhalter | Bedeutung | Beispiel |
|-------------|-----------|----------|
| `{{NAME}}` | Dein Name | Max Mustermann |
| `{{ORT}}` | Wohnort/Region | Wien, AT |
| `{{VAULT_NAME}}` | Name des Vaults | Mein Hirn |
| `{{KONTEXT}}` | 1–2 Sätze über dich | „Arbeite lösungsorientiert, baue technische Systeme." |

> `{{DOMAIN}}`, `{{VPS_IP}}` & Co. tauchen erst in Stufe 2/3 auf — hier ignorieren.

## 4. Loslegen
- Tagesnotiz: `Tagebuch/YYYY-MM-DD.md` (Vorlage in `templates/`)
- Neues Projekt: Datei in `Projekte/` (Vorlage in `templates/`)
- Frage an die KI im Tagebuch markieren: `#frage`

## 5. Die KI anlernen
`CLAUDE.md` ist der Einstiegspunkt. Wenn du mit einer KI (z.B. Claude) arbeitest, gib ihr
diese Datei als Kontext — sie beschreibt Struktur, Regeln und wie du arbeitest.
