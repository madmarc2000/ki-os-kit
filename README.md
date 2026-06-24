# KI-OS Kit

Ein Bausatz, um ein persönliches **KI-Betriebssystem auf Basis von Obsidian** nachzubauen: strukturiertes "zweites Gehirn", eine `CLAUDE.md` als Router/Identität für die KI, klare Arbeitsregeln und ein optionaler autonomer Agent.

## Was ist Obsidian?

**Obsidian ist eine kostenlose Notiz-App.** Der Unterschied zu allen anderen: Deine Notizen bleiben als einfache Textdateien auf deinem eigenen Gerät — kein Konto, niemand liest mit, niemand kann den Zugang abschalten. Verschwindet die App, hast du trotzdem alles, denn es sind ja normale Dateien. Du kannst Notizen verknüpfen und in Sekunden durchsuchen — ein digitales Notizbuch, das ganz dir gehört.

Für ein KI-System ist genau das der entscheidende Punkt: Weil alles Klartext ist, kann deine **KI den Vault direkt lesen**. Er ist gleichzeitig dein Gedächtnis und der Wissensspeicher, aus dem die KI arbeitet — ohne dass deine Daten je das Haus verlassen.

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

## Auf iPhone oder iPad öffnen

Geht — ist nur einen Schritt fummeliger als am Computer, weil Obsidian auf iOS einen Vault nur an *einem* bestimmten Ort findet. Einmal verstanden, dauert es zwei Minuten. Du brauchst die **Obsidian-App** (gratis im App Store).

1. **Nur beim allerersten Mal:** Obsidian öffnen → "Neuen Vault erstellen" (engl. *Create new vault*) → irgendein Name → **"In iCloud sichern"** (engl. *Store in iCloud*) einschalten → erstellen. Das legt den iCloud-Ordner an, den Obsidian kennt. Diesen Probe-Vault kannst du danach ignorieren oder löschen.
2. **ZIP entpacken:** Dateien-App öffnen → dein heruntergeladenes ZIP lange gedrückt halten → **"Entpacken"**. Es entsteht ein Ordner mit deinem Vault-Namen.
3. **Ordner an den richtigen Ort schieben:** Den ganzen Ordner lange drücken → **"Bewegen"** → iCloud Drive → Ordner **Obsidian** → dort ablegen. Wichtig: den **kompletten Ordner** verschieben, nicht hineingehen und einzelne Dateien herausziehen — sonst bleiben die (unsichtbaren) Einstellungen zurück.
4. **Öffnen:** Obsidian → unten auf den Vault-Namen tippen (Vault-Umschalter) → dein Vault steht in der Liste → antippen. Fertig.

Taucht der Vault nicht auf, liegt er fast immer noch außerhalb des iCloud-Ordners "Obsidian" — das ist die häufigste Stolperfalle.

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
