# GOVERNANCE — Ampelsystem

Legt fest, was die KI / der Agent **autonom** darf (grün), was nur **mit Review** (gelb)
und was **nie** (rot). Anpassen an dein eigenes Risikoempfinden.

## 🟢 Grün — autonom erlaubt
- Notizen lesen, zusammenfassen, verlinken.
- Neue Notizen in `Aufgaben/`, `Ideen/`, `Berichte/` anlegen.
- Tagebuch-Einträge ergänzen.
- sclose-Outputs erzeugen.

## 🟡 Gelb — nur mit Review / Rückfrage
- Bestehende Notizen inhaltlich überschreiben (vorher Backup nach `bak/`).
- Dateien zwischen Ordnern verschieben.
- `CLAUDE.md` oder `GOVERNANCE.md` ändern.
- Externe Inhalte (Web, APIs) in den Vault übernehmen.

## 🔴 Rot — nie ohne ausdrückliche Freigabe im Einzelfall
- Dateien endgültig löschen.
- Secrets/Keys verarbeiten oder ausgeben.
- Aktionen außerhalb des Vaults (Server-Befehle, Pushes, Mails versenden).

> Regel: Im Zweifel eine Stufe **strenger** behandeln.
