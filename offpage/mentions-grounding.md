---
type: Offpage
title: Mentions, Sentiment und Konsistenz
description: Externe Erwähnungen auf vertrauenswürdigen Plattformen als Grounding-Quelle für generative Antworten.
tags: [geo, offpage, mentions, sentiment, konsistenz, grounding]
timestamp: 2026-07-15T09:00:00Z
---

# Mechanik

LLM-Systeme stützen ihre Antworten auf Quellen, die sie bereits als verlässlich einstufen. Ohne starke externe Präsenz nimmt ein Modell eine Marke selbst dann nicht in die Antwort auf, wenn der eigene Onpage-Inhalt fehlerfrei ist. Externe Erwähnungen speisen dieselbe Grounding-Logik wie die [Zitierwürdigkeit](/methoden/zitierwuerdigkeit.md) onpage.

# Anforderungen

1. **Mentions auf Trust-Plattformen.** Erwähnungen auf Nachrichtenportalen, Branchenmedien und etablierten Foren (etwa Reddit) aufbauen. Sie erzeugen indirekte Zitationen: Das Modell zitiert die externe Quelle, die auf die Marke verweist.
2. **Sentiment steuern.** Der Kontext der Erwähnung zählt. Systematisches Review-Marketing auf relevanten Bewertungsplattformen aufbauen, da KI-Systeme Bewertungen für Empfehlungen aktiv auswerten.
3. **Datenkonsistenz.** Produktnamen, Preise, Funktionsumfang und Firmendaten müssen auf allen externen Flächen identisch sein (Verzeichnisse, Wikidata, App-Stores, Social-Profile). Widersprüchliche Angaben senken das Modellvertrauen in alle Quellen der Marke.
4. **Präsenz in Listicles.** Transaktionale Prompts ("bestes Tool für X") beantworten Modelle häufig auf Basis externer Rankings und Top-Listen. Die Marke muss in den relevanten externen Vergleichen vertreten sein.

# Citations

[1] [GEO-Infrastruktur und Reputation](/quellen/geo-infrastruktur-reputation.md)
