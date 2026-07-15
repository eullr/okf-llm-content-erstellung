---
type: Methode
title: Sprache und Formulierung
description: Satzbau- und Wortwahlregeln, die präzise Vektor-Embeddings und fehlerfreie Extraktion ermöglichen.
tags: [geo, sprache, redaktion, embeddings]
timestamp: 2026-07-15T09:00:00Z
---

# Grundprinzip

Die Sprache muss maximal dicht, einfach und eindeutig sein. Jedes überflüssige Wort verwässert das Vektor-Embedding des Absatzes und senkt die Wahrscheinlichkeit, dass der Block einem passenden Prompt zugeordnet wird.

# Regeln

1. **Aktiv statt Passiv.** Aktive Konstruktionen verkürzen den Satz und machen die Handlungsträger explizit. Das unterstützt zugleich den Entity-First-Ansatz aus dem [Chunking](/methoden/chunking.md).
2. **Füllwörter streichen.** Einleitungen wie "grundsätzlich", "natürlich", "sehr" oder "diesbezüglich" tragen keine Information und entfallen.
3. **Kurze Sätze.** Lange Schachtelsätze in mehrere kurze Aussagen zerlegen. Jede Aussage wird so einzeln extrahierbar.
4. **Konstruktive Unsicherheit.** Gibt es keine pauschale Antwort, wird die Abhängigkeit direkt formuliert: "Die Wahl hängt von X und Y ab; wer A braucht, wählt Variante 1." Vage Ausweichformulierungen ("es kommt auf viele Faktoren an") sind wertlos.

# Wirkung

Ein Absatz ohne Füllmaterial bildet einen scharfen Vektorprofil-Punkt im Embedding-Raum. Die Maschine kann ihn dem Nutzerintent ohne Mehrdeutigkeit zuordnen. Diffuse Absätze benötigen dagegen mehr umgebenden Kontext und verlieren im Retrieval gegen fokussierte Konkurrenzblöcke.

# Citations

[1] [GEO-Content-Anforderungen](/quellen/geo-content-anforderungen.md)
