---
type: Messung
title: Erfolgsmessung über Share of Mentions
description: Messalgorithmus, der Content-Umbauten kausal mit der Markenpräsenz in generativen Antworten verknüpft.
tags: [geo, messung, share-of-mentions, kpi, benchmark]
timestamp: 2026-07-15T09:00:00Z
---

# Leitmetriken

* **Share of Mentions (SoM):** Anteil der getrackten Prompts, in deren Antworten die Marke erwähnt wird. Zentrale Erfolgsgrösse für Content-Umbauten.
* **Share of Direct Citations:** Anteil der Prompts, in denen das Modell die eigene Website direkt als Quelle verlinkt.
* **Indirect Citations:** Anzahl der Prompts, in denen das Modell externe Quellen zitiert, die auf die Marke verweisen, siehe [Offpage](/offpage/mentions-grounding.md).

Anteilswerte (Share) sind absoluten Zählwerten vorzuziehen: Der Prompt-Pool ändert sich über die Zeit, Prozentwerte bleiben vergleichbar und schützen den Trend vor Verzerrung.

# Messalgorithmus

1. **Input-Register führen.** Dokumentieren, welche URLs oder Unterthemen wann in Chunk-Form umgebaut und publiziert wurden. Ohne dieses Register lässt sich eine SoM-Veränderung keiner Massnahme zuordnen.
2. **Repräsentativen Prompt-Pool bilden.** Pro umgebautem Themencluster eine begrenzte, repräsentative Prompt-Auswahl mit informationalem oder transaktionalem Intent definieren.
3. **Auf URL-Ebene aggregieren.** SoM nicht pro Einzelprompt bewerten, sondern alle Prompts eines Clusters bündeln. Die Aggregation verbindet die operative Umsetzung mit dem messbaren Ergebnis und zeigt, ob der Umbau systematisch wirkt.
4. **Tooling aufsetzen.** Tracking-Plattformen (Peec AI, Rankscale, SISTRIX AI Prompt Tracking, Otterly.AI) auf tägliche Erhebung konfigurieren. Achtung Terminologie: Dieselbe Metrik heisst bei Peec AI "Visibility" und bei Otterly.AI "Brand Coverage"; für das Reporting ein internes Begriffs-Mapping pflegen.
5. **Wettbewerber benchmarken.** SoM für die relevanten Wettbewerber auf denselben Prompts mitlaufen lassen. Steigt der eigene Wert bei stagnierenden Wettbewerbern, ist die Wirkung der Massnahme belegt. Wird ein Wettbewerber dort erwähnt, wo die eigene Marke fehlt, dessen Chunk-Qualität analysieren.

# Risiken und blinde Flecken

* **Fragmentierung.** Derselbe Prompt liefert je nach Dialogkontext und Sitzungshistorie unterschiedliche Antworten, mit oder ohne Markennennung. Besonders relevant bei Chat-Systemen.
* **Sentiment-Automatik.** Tools klassifizieren Tonalität meist über Wortlisten und irren regelmässig. Stichprobenweise manuelle Validierung einplanen.
* **Positionsmetrik.** Die Position einer Erwähnung in der Antwort ist ohne Kontext wertlos: Platz eins kann in einer Warnliste stehen. Belastbar ist nur die Kombination aus Share of Mentions und validiertem Sentiment.
* **Attribution Gap.** Nutzer sehen die Marke in der KI-Antwort und suchen sie später direkt, ohne zu klicken. Web-Analytics kann diesen Pfad nicht zuordnen; der gemessene ROI unterschätzt die reale Wirkung.

# Citations

[1] [SoM-Messalgorithmus](/quellen/som-messalgorithmus.md)
[2] [OKR-Framework für die Chunking-Einführung](/quellen/okr-chunking-framework.md)
