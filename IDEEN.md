# Ideen & offene Konzepte

Lose Gedanken zur Weiterentwicklung des Kits. Noch nicht umgesetzt — erst diskutieren,
dann entscheiden, dann bauen.

---

## Selbst-fortschreibende Notizen — sauber gebaut

**Idee:** Notizen sollen sich mit neuer Info „von selbst" weiterentwickeln.

**Erkenntnis:** Eine Notiz ist passiv — sie entwickelt sich nicht selbst, die KI muss sie
lesen und schreiben. Eine Pflege-Regel *in* der Notiz greift nur, wenn die Notiz ohnehin
schon im Kontext ist. Der wichtige Fall („ich lerne etwas Neues über X") braucht aber, dass
die KI *weiß, dass die X-Notiz existiert* und sie gezielt zieht — dieses Routing kann nicht
in der noch-nicht-geladenen Notiz stehen.

**Saubere Trennung:**
- **Zentrales Routing** (in `CLAUDE.md`): „Info über eine Person/Projekt → deren Notiz
  aktualisieren." Generische Pflege gehört zentral, an *eine* Stelle.
- **Notiz-eigene Pflege-Zeile** nur dort, wo der Trigger *spezifisch* für diese Notiz ist
  (z. B. „Beträge jährlich im Jänner gegen quelle.at prüfen"). Das passt nicht in eine
  zentrale Regel, weil es nur hier gilt.

**Beispiel** (notiz-spezifischer Trigger):
```
---
type: referenz
tags: [foerderung]
date: 2026-06-24
---
# Förderungen
Zuschuss: 1.200 €/Monat (Stand 2026-06, quelle.at)
> Pflege: Beträge jährlich im Jänner gegen quelle.at prüfen.
```

**Voraussetzung:** Setzt atomisierte Entitäten voraus — die atomare Notiz ist der Ort für
ihre spezifische Pflege-Regel. Koppelt damit an die Atomisieren-Idee.

**Verworfen:** Eine generische „so pflege mich"-Zeile in *jeder* Notiz → Drift (hunderte
identische Mikro-Policies) und informationslos, analog zu einem `ai-first: true`, das
überall `true` ist. „Eine Quelle pro Fakt."

---

## Atomisieren wiederkehrender Entitäten

**Idee:** Flache Bullet-Listen (z. B. eine zentrale „Entscheidungen"-Sektion) sind nicht
verlinkbar und nur als Ganzes ladbar. Wiederkehrende Entitäten als eigene Notizen werden
Graph-Knoten und einzeln on-demand abrufbar.

**Scope (wichtig):** Nur was *oft referenziert* **und** *on-demand gebraucht* wird —
Personen, aktive Projekte, die dicksten Entscheidungen. Nicht jede flüchtige Idee.

**Trade-off:** Mehr Dateien = mehr Sprünge (relevant bei einhändiger Mobil-Nutzung) und was
atomisiert wird, liegt nicht mehr automatisch im Standard-Briefing. Was immer im Kontext
sein soll, bleibt im kompakten Briefing; Atomares ist für Referenz-auf-Abruf.

**Rollout:** forward-only (Konvention ab jetzt) + kleiner gezielter Backfill der meist-
referenzierten Entitäten. Kein Vault-weites Rewrite.

---

## Offen / zu prüfen

- `type`-Feld nur in gemischten Ordnern sinnvoll (in `Projekte/` ist es Duplikat zum Ordner).
- `ai-first: true` im Kit nochmal prüfen: trägt nur Information, wenn es Notizen gibt, bei
  denen es `false` wäre (z. B. importierte Alt-Vaults). Sonst raus.
- **KI-neutraler Build-/Adapter-Schritt:** Ein Script, das die neutrale Router-Quelle in
  `CLAUDE.md` (Claude Code), `AGENTS.md` (Codex/OpenCode) und `GEMINI.md` (Gemini CLI)
  spiegelt — eine Quelle, mehrere Tool-Outputs. Macht das Kit echt anbieter-unabhängig statt
  nur „kopier den Inhalt rüber". Die reifen Repos (eugeniughelbur) machen genau das.
