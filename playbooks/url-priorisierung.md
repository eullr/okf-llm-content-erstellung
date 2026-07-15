---
type: Playbook
title: URL-Priorisierung für den Umbau
description: Kriterien und Reihenfolge für die Auswahl der zuerst umzubauenden Seiten.
tags: [playbook, priorisierung, roadmap]
timestamp: 2026-07-15T09:00:00Z
---

# Vorfilter: technische Blocker

URLs mit blockiertem Crawler-Zugang (robots.txt, Firewall, reines Client-Rendering) werden nicht redaktionell umgebaut, bevor der Zugang steht. Redaktionsaufwand auf unsichtbaren Seiten ist verlorener Aufwand, siehe [Crawler-Zugang](/technik/crawler-zugang.md).

# Priorisierungskriterien

Je URL beziehungsweise Cluster vier Kriterien bewerten:

1. **Prompt-Nachfrage.** Wie viele getrackte Prompts des Kunden zielen auf das Thema des Clusters? Hohe Nachfrage zuerst.
2. **Wettbewerbs-Gap.** Wird ein Wettbewerber in den Antworten erwähnt, die eigene Marke nicht? Solche Cluster haben den grössten kurzfristigen Hebel, siehe [Erfolgsmessung](/messung/share-of-mentions.md).
3. **Geschäftswert.** Nähe des Clusters zu Transaktion oder Lead; informativ-ferne Themen nachrangig.
4. **Umbau-Aufwand.** Grobe Schätzung: Anzahl Absätze, Verfügbarkeit von Eigendaten für die [Zitierwürdigkeit](/methoden/zitierwuerdigkeit.md), Abhängigkeit von IT-Änderungen.

# Reihenfolgebildung

Hoch bewertete Nachfrage plus Wettbewerbs-Gap bei niedrigem Aufwand bilden die erste Welle. Cluster mit hohem Geschäftswert, aber IT-Abhängigkeit laufen parallel als Technik-Tickets an. Die Reihenfolge wird nach jedem Messfenster gegen die tatsächliche SoM-Entwicklung neu geprüft, nicht einmalig festgeschrieben.

# Citations

[1] [SoM-Messalgorithmus](/quellen/som-messalgorithmus.md)
