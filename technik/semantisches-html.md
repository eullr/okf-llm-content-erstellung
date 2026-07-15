---
type: Technik
title: Semantisches HTML und strukturierte Daten
description: Maschinenlesbare Code-Struktur, damit KI-Systeme Sinnblöcke, Tabellen und Entitäten korrekt interpretieren.
tags: [geo, technik, html, schema-org, json-ld, informationsarchitektur]
timestamp: 2026-07-15T09:00:00Z
---

# Grundproblem

Maschinen sehen kein visuelles Design, sie lesen Code-Struktur. Ein Inhalt, der visuell wie eine Tabelle aussieht, aber aus div-Containern besteht, ist für die Extraktion unbrauchbar.

# Anforderungen

1. **Semantische HTML-Tags.** article, main, header und footer statt bedeutungsloser div- und span-Container. Die Tags markieren, was Hauptinhalt ist und was Beiwerk.
2. **Echte Tabellen und Listen.** Vergleichstabellen mit table, thead, tbody, tr und td auszeichnen. Nur so können KI-Systeme die Daten zeilen- und spaltenweise extrahieren. Tabellen gehören zu den am häufigsten direkt übernommenen Elementen, siehe [Query-Fan-out](/methoden/query-fan-out.md).
3. **Schema.org via JSON-LD.** Strukturierte Daten sind Pflicht: Person für Autoren, Article für Beiträge, Product und Offer für Angebote, FAQPage für Fragenblöcke. JSON-LD ist vom visuellen HTML getrennt und maschinell am einfachsten zu verarbeiten. Die Markup-Daten speisen unter anderem den Google Knowledge Graph, aus dem AI Overviews schöpfen.
4. **Cluster-Architektur.** Inhalte als Pillar-Seite mit unterstützenden Detailartikeln organisieren. Interne Links tragen beschreibende Ankertexte ("Analyse der Klicktiefe" statt "mehr dazu"), damit der Zielkontext maschinenlesbar mitgegeben wird.

# Verbindung zur Redaktion

Die Code-Struktur ist das technische Gegenstück zu den [Chunking-Regeln](/methoden/chunking.md): Überschriftenhierarchie, echte Listen und Tabellen definieren die Grenzen, an denen Retrieval-Systeme Blöcke schneiden.

# Citations

[1] [GEO-Infrastruktur und Reputation](/quellen/geo-infrastruktur-reputation.md)
[2] [Schema.org Vokabular](https://schema.org)
