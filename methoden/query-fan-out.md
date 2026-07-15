---
type: Methode
title: Query-Fan-out abdecken
description: Alle Teilfragen eines komplexen Prompts auf einer Seite beantworten, damit die Seite als universeller Quellendonor dient.
tags: [geo, query-fan-out, faq, vollstaendigkeit]
timestamp: 2026-07-15T09:00:00Z
---

# Mechanik

Systeme wie AI Overviews zerlegen einen komplexen Nutzerprompt in mehrere Teilanfragen (Sub-Queries) und beantworten jede separat. Eine Seite, die viele dieser Teilfragen in eigenständigen Blöcken abdeckt, wird für die zusammengesetzte Antwort mehrfach herangezogen.

# Regeln

1. **Erwartbare Fragen antizipieren.** Angrenzende Themen wie Preise, Risiken, Alternativen, Schritt-für-Schritt-Vorgehen und typische Fehler als eigene Sinnblöcke oder FAQ-Abschnitte ausformulieren.
2. **Es-kommt-darauf-an-Szenarien.** Bedingungen und Entscheidungsbäume integrieren: wann welcher Ansatz besser passt, mit klaren Kriterien. Solche Blöcke haben überdurchschnittlichen Extraktionswert.
3. **Direkte Vergleiche.** Gegenüberstellungen im Format "X gegen Y" mit benannten Kriterien anlegen, bevorzugt als echte Tabelle (technische Anforderungen in [Semantisches HTML](/technik/semantisches-html.md)).
4. **Fragende Zwischenüberschriften.** Jede Teilfrage erhält eine eigene H2- oder H3-Frage und darunter einen autonomen Block nach den [Chunking-Regeln](/methoden/chunking.md).

# Citations

[1] [GEO-Content-Anforderungen](/quellen/geo-content-anforderungen.md)
