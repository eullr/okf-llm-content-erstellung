---
type: Methode
title: Zitierwürdigkeit (Citation-Worthiness)
description: Faktendichte und Eigendaten, die eine LLM beim Grounding zur Quellenangabe zwingen.
tags: [geo, citations, grounding, faktendichte]
timestamp: 2026-07-15T09:00:00Z
---

# Mechanik: Grounding

Um Halluzinationen zu vermeiden, sucht eine LLM in externen Dokumenten nach Belegen (Grounding): konkrete Zahlen, Bedingungen, prüfbare Aussagen. Inhalte mit hoher Informationsdichte werden dabei bevorzugt extrahiert und mit direkter Quellenangabe (Citation) versehen. Inhalte ohne Belegwert werden paraphrasiert oder ignoriert.

# Regeln

1. **Konkrete Zahlen statt vager Aussagen.** Metriken, Prozentwerte, Spannen, Preise und technische Parameter benennen. "Deutlich schneller" ist wertlos, "42 Prozent kürzere Ladezeit" ist zitierfähig.
2. **Schwer reproduzierbare Eigendaten.** Eigene Markttests, interne Auswertungen und dokumentierte Fallstudien einsetzen. Daten, die es nirgendwo sonst gibt, machen die eigene Seite zur einzig möglichen Quelle.
3. **Textanker für Multimedia.** LLMs extrahieren Text. Kernaussagen von Grafiken, Rechnern und interaktiven Elementen müssen im Fliesstext dupliziert werden: "Der Rechner zeigt eine Ersparnis von X Prozent." Ohne Textanker verliert der zugehörige [Chunk](/methoden/chunking.md) bei der Extraktion seinen Sinn.

# Zusammenhang mit Offpage

Grounding stützt sich nicht nur auf die eigene Seite, sondern auch auf externe Quellen, die über die Marke schreiben. Die Offpage-Seite dieses Mechanismus in [Mentions, Sentiment und Konsistenz](/offpage/mentions-grounding.md).

# Citations

[1] [GEO-Content-Anforderungen](/quellen/geo-content-anforderungen.md)
