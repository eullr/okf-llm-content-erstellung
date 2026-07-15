---
type: Quelle
title: GEO-Infrastruktur und Reputation
description: Technische, semantische und Offpage-Anforderungen, ohne die LLM-optimierter Text unsichtbar bleibt.
tags: [quelle, geo, technik, offpage]
timestamp: 2026-07-15T09:00:00Z
verlaesslichkeit: hoch
---

# Inhalt in Kürze

Drei Anforderungsblöcke jenseits des Texts: (1) Crawler-Zugang, (2) maschinenlesbare Code-Semantik, (3) externe Reputation als Grounding-Basis.

# Kernaussagen

* KI-Crawler (GPTBot, ClaudeBot) lesen nur den initialen Server-HTML-Response und führen kein JavaScript aus.
* robots.txt ist verbindlich, llms.txt experimentell; Firewalls und CDN-Regeln blockieren KI-Bots teils versehentlich.
* KI-Bots folgen internen 301-Weiterleitungen in der Regel nicht; 5xx-Fehler können das Crawling stoppen.
* Semantische Tags (article, main), echte table-Auszeichnung und Schema.org via JSON-LD sind Pflicht; JSON-LD speist unter anderem den Google Knowledge Graph.
* Cluster-Architektur (Pillar plus Detailseiten) mit beschreibenden Ankertexten.
* Offpage: Mentions auf Trust-Plattformen, systematisches Review-Marketing, Datenkonsistenz über alle externen Flächen, Präsenz in Listicles.
* Risiken: Blackbox-Retrieval ohne Garantien; SSR-Umbau und fehlerfreie Architektur kosten IT-Budget.
