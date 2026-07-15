---
type: Quelle
title: SoM-Messalgorithmus
description: Fünfstufiger Algorithmus zur Messung der Chunking-Wirkung über Share of Mentions.
tags: [quelle, messung, share-of-mentions]
timestamp: 2026-07-15T09:00:00Z
verlaesslichkeit: hoch
---

# Inhalt in Kürze

Begründet, warum klassischer Traffic als KPI für Chunking untauglich ist (Zero-Click), und definiert Share of Mentions als Leitmetrik mit fünfstufigem Messalgorithmus.

# Kernaussagen

* Input-Register: dokumentieren, welche URLs wann in Chunk-Form publiziert wurden; ohne Register keine Kausalzuordnung.
* Begrenzter, repräsentativer Prompt-Pool pro Themencluster.
* Aggregation auf URL- bzw. Cluster-Ebene statt Einzelprompt-Betrachtung.
* Tool-Terminologie divergiert: Share of Mentions heisst bei Peec AI "Visibility", bei Otterly.AI "Brand Coverage"; internes Mapping nötig.
* Wettbewerbs-Benchmark auf denselben Prompts validiert die Wirkung.
* Anteilswerte statt Absolutzahlen, da sich der Prompt-Pool über die Zeit ändert.
* Risiken: Antwort-Fragmentierung je nach Dialogkontext, fehleranfällige Sentiment-Automatik, wertlose Positionsmetrik ohne Kontext.
