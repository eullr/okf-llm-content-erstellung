---
type: Methode
title: Semantisches Chunking
description: Regeln zur Zerlegung von Inhalten in autonome, extrahierbare Blöcke für generative Systeme.
tags: [geo, chunking, content-architektur, retrieval]
timestamp: 2026-07-15T09:00:00Z
---

# Warum Chunking?

Generative Systeme analysieren Texte nicht linear von Anfang bis Ende. Sie zerlegen Seiten in einzelne Sinnblöcke (Chunks), wandeln diese in Vektor-Embeddings um und wählen für eine Antwort den Block mit der höchsten semantischen Relevanz zum Prompt. Die Relevanz eines einzelnen, präzise fokussierten Absatzes wiegt dabei oft schwerer als die Autorität der gesamten Domain. Ein sauber geschnittener Chunk erzeugt ein scharfes Embedding und wird dadurch zuverlässiger extrahiert.

# Kernregeln

1. **Ein Block, eine Aussage.** Jeder Absatz trägt genau einen Fokus oder beantwortet genau eine Frage. Semantisches Rauschen, leere Einleitungen und vage Formulierungen entfallen vollständig.
2. **Umgekehrte Pyramide.** Die Kernaussage steht im ersten Satz des Absatzes. Begründungen, Zahlen und Beispiele folgen danach.
3. **Volle Autonomie (Self-Containment).** Jeder Chunk muss ohne den Rest des Dokuments verständlich sein, damit die LLM ihn ohne Verzerrung in ihre Antwort übernehmen kann. Der Block beantwortet die Fragen Was, Wer und Wo aus sich selbst heraus.
4. **Entity-First.** Pronomen konsequent durch die Kernentität ersetzen: "Amazon Go" statt "das System", "die Peec-Visibility" statt "der Wert". Ohne explizite Entität verliert der Block ausserhalb seines Kontexts jede Bedeutung.
5. **Fragende Zwischenüberschriften.** H2 und H3 als Fragen formulieren. Das entspricht der Sprache der Nutzerprompts und den Teilfragen des [Query-Fan-out](/methoden/query-fan-out.md).
6. **Listen und Tabellen als atomare Einheiten.** Aufzählungen und Tabellen dürfen beim Schneiden nicht getrennt werden; sie werden von LLMs häufig direkt in Antworten übernommen.
7. **Bedingungs-Chunks.** Es-kommt-darauf-an-Szenarien explizit ausformulieren: wenn A, dann X; wenn B, dann Y. Klare Entscheidungskriterien erhöhen den Extraktionswert deutlich.
8. **Verbinden ohne Vermischen.** Sinnblöcke über Sprungmarken und interne Verlinkung koppeln, dabei die Grenzen jedes Chunks erhalten. Anforderungen an Ankertexte in [Semantisches HTML](/technik/semantisches-html.md).

# Negativbeispiel: mechanischer Schnitt

Ein rein nach Zeichenlänge geschnittener Block wie "...ermöglicht es Kunden, den Laden zu betreten, die Artikel mitzunehmen und ihn zu verlassen, ohne an einer Kasse anstehen zu müssen..." ist für Retrieval wertlos: Die Entität (Amazon Go) und das Konzept (Just Walk Out) fehlen, der Block kann keinem Prompt sicher zugeordnet werden und erhöht das Halluzinationsrisiko.

# Grenzen der Methode

* Es existiert kein Industriestandard für die optimale Chunk-Länge. ChatGPT, Perplexity und AI Overviews schneiden und bewerten unterschiedlich; die Optimierung bleibt iterativ und wird über die [Erfolgsmessung](/messung/share-of-mentions.md) gesteuert.
* Ein zu radikal auf Frage-Antwort-Blöcke reduzierter Text kann menschliche Leser abstossen. Guter Fliesstext mit klarer innerer Logik und visueller Struktur ist ebenfalls chunkbar; die Regeln gelten für die Struktur, nicht gegen die Lesbarkeit.
* Stützt sich ein Absatz auf eine Grafik ("wie die Abbildung zeigt"), verliert der Chunk bei der Extraktion seinen Sinn. Gegenmassnahme: Textanker, siehe [Zitierwürdigkeit](/methoden/zitierwuerdigkeit.md).

# Citations

[1] [OKR-Framework für die Chunking-Einführung](/quellen/okr-chunking-framework.md)
[2] [GEO-Content-Anforderungen](/quellen/geo-content-anforderungen.md)
[3] [Technical Guide Semantisches Chunking](/quellen/chunking-technical-guide.md) (nur Entity-First und Self-Containment)
