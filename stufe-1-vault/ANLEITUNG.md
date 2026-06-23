# Anleitung — Stufe 1 einrichten

> **Schneller Weg:** Statt der Schritte 3 unten kannst du `INIT.md` als Kontext an deine KI
> geben und „führe mich durch das Setup" sagen — sie fragt die Grundlagen ab und legt
> Struktur, Kontext-Dateien und die fertige `CLAUDE.md` selbst an. Diese Anleitung beschreibt
> den **manuellen** Weg (ohne KI-Zugang).

## 1. Obsidian installieren
[obsidian.md](https://obsidian.md) — kostenlos, lokal. Diesen Ordner (`stufe-1-vault/`)
als Vault öffnen: *Vault öffnen → Ordner wählen*.

## 2. Sync wählen
Hält den Vault auf mehreren Geräten gleich. Eine Option genügt:

- **iCloud / Dropbox / OneDrive / Google Drive** — Vault-Ordner ins Cloud-Verzeichnis legen. Gratis, null Konfiguration; iCloud ist auf Apple-Geräten der einfachste Weg. Nachteil: keine echte Versionshistorie, gelegentlich Sync-Konflikte (v. a. am `.obsidian`-Ordner).
- **[Obsidian Sync](https://obsidian.md/sync)** — der hauseigene Dienst, ab ~$4/Monat (jährlich, [Preise](https://obsidian.md/pricing)). Ende-zu-Ende-verschlüsselt, Versionshistorie, plattformübergreifend, am reibungsärmsten.
- **Git** (Obsidian-Git-Plugin) — gratis, volle Versionshistorie, von überall klonbar. Auf Handy/Tablet aber fummelig.

Faustregel: nur Apple-Geräte → iCloud · plattformübergreifend & bequem → Obsidian Sync · technik-affin & Versionshistorie wichtig → Git.

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
