---
type: Vorlage
title: Seitenstruktur für LLM-optimierte Inhalte
description: Grundgerüst einer Ratgeber- oder Pillar-Seite mit autonomen Chunk-Blöcken.
tags: [vorlage, seitenstruktur, chunking]
timestamp: 2026-07-15T09:00:00Z
---

# Gerüst

```markdown
# [Kernentität + Kernnutzen als H1]

[Direktantwort-Absatz: Kernaussage der Seite in zwei bis drei Sätzen,
mit Datumsmarker "Stand MM/JJJJ" und mindestens einer konkreten Zahl.]

## Was ist neu?
[Update-Box, siehe /vorlagen/update-box.md]

## [Teilfrage 1 als H2, in Nutzersprache]
[Autonomer Block: Antwort im ersten Satz, dann Belege.
Entität beim Namen nennen, keine Pronomen über Blockgrenzen.]

## [Teilfrage 2: Vergleich "X oder Y?"]
[Echte HTML-Tabelle mit benannten Kriterien.]

## [Teilfrage 3: "Wann lohnt sich was?"]
[Bedingungs-Chunk: wenn A, dann X; wenn B, dann Y. Kriterien explizit.]

## Häufige Fragen zu [Kernentität]
[FAQ-Block, siehe /vorlagen/faq-block.md]

[Autorenbox: Name, Qualifikation, Rolle, Profil-Link.]
```

# Verwendungsregeln

* Jeder H2-Block muss den Self-Containment-Test bestehen: aus dem Kontext gerissen bleibt er verständlich, siehe [Chunking](/methoden/chunking.md).
* Reihenfolge der Teilfragen nach Prompt-Nachfrage des Clusters, nicht nach interner Logik des Autors, siehe [Query-Fan-out](/methoden/query-fan-out.md).
* Technische Abnahme (semantische Tags, JSON-LD) vor Publikation, Kriterien in [Semantisches HTML](/technik/semantisches-html.md).
