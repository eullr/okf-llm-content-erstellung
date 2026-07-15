---
type: Referenz
title: Glossar
description: Verbindliche Definitionen der GEO-Kernbegriffe und Mapping der Tool-Terminologie.
tags: [referenz, glossar, terminologie]
timestamp: 2026-07-15T09:00:00Z
---

# Begriffe

| Begriff | Definition |
| --- | --- |
| Chunk | Autonomer Sinnblock eines Dokuments, den ein Retrieval-System einzeln extrahiert und bewertet. Regeln in [Semantisches Chunking](/methoden/chunking.md). |
| Vector Embedding | Mathematische Repräsentation eines Textblocks, über die das System die semantische Nähe zu einem Prompt berechnet. |
| Grounding | Absicherung einer LLM-Antwort durch Abgleich mit externen Dokumenten; Grundlage für Zitierung. Siehe [Zitierwürdigkeit](/methoden/zitierwuerdigkeit.md). |
| Query-Fan-out | Zerlegung eines komplexen Prompts in Teilanfragen (Sub-Queries), die separat beantwortet werden. Siehe [Query-Fan-out abdecken](/methoden/query-fan-out.md). |
| Direct Citation | Direkte Verlinkung der eigenen Website als Quelle in einer generativen Antwort. |
| Indirect Citation | Zitierung einer externen Quelle, die ihrerseits auf die Marke verweist. Siehe [Offpage](/offpage/mentions-grounding.md). |
| Share of Mentions (SoM) | Anteil der getrackten Prompts, in deren Antworten die Marke erwähnt wird. Leitmetrik, siehe [Erfolgsmessung](/messung/share-of-mentions.md). |
| Citation-Worthiness | Faktendichte eines Blocks, die ihn als Grounding-Beleg qualifiziert. |
| Entity-First | Prinzip, Pronomen durch explizite Kernentitäten zu ersetzen, damit der Block ausserhalb seines Kontexts eindeutig bleibt. |
| Self-Containment | Eigenschaft eines Chunks, ohne das Restdokument vollständig verständlich zu sein. |
| Recency Bias | Präferenz generativer Systeme für frische Inhalte. Siehe [Aktualität](/methoden/aktualitaet.md). |
| Timestamp-Gaming | Vortäuschung von Aktualität durch Datumsänderung ohne inhaltliches Update. Siehe [Anti-Patterns](/referenz/anti-patterns.md). |
| Zero-Click | Beantwortung des Prompts im KI-Interface ohne Klick auf die Quelle; entwertet Traffic als KPI. |
| Attribution Gap | Nicht messbarer Pfad, wenn Nutzer die Marke in einer KI-Antwort sehen und später direkt suchen. |
| E-E-A-T | Experience, Expertise, Authoritativeness, Trustworthiness; Vertrauensrahmen, siehe [Autorschaft](/methoden/eeat-autorschaft.md). |

# Tool-Terminologie-Mapping

Dieselbe Metrik trägt je nach Plattform unterschiedliche Namen. Für Reports gilt das interne Mapping:

| Interner Begriff | Peec AI | Otterly.AI |
| --- | --- | --- |
| Share of Mentions | Visibility | Brand Coverage |

Bei Aufnahme weiterer Tools (Rankscale, SISTRIX AI Prompt Tracking) wird die Tabelle erweitert; jede Erweiterung wird im [Log](/log.md) vermerkt.

# Citations

[1] [SoM-Messalgorithmus](/quellen/som-messalgorithmus.md)
