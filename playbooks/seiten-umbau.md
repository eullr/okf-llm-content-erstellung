---
type: Playbook
title: Seiten-Umbau in Chunk-Form
description: Siebenstufiger Ablauf für den Umbau einer bestehenden Seite, von der SoM-Baseline bis zur Iteration.
tags: [playbook, umbau, prozess]
timestamp: 2026-07-15T09:00:00Z
---

# Ablauf

1. **Baseline messen.** Prompt-Pool des Ziel-Clusters definieren und den aktuellen Share of Mentions vor jedem Eingriff erheben. Ohne Baseline ist die Wirkung später nicht belegbar, siehe [Anti-Patterns](/referenz/anti-patterns.md).
2. **Technik-Gate prüfen.** Server-HTML, robots.txt-Freigabe, Firewall und Statuscodes der Ziel-URL verifizieren, Kriterien in [Crawler-Zugang](/technik/crawler-zugang.md). Ist der Zugang blockiert, hat der redaktionelle Umbau keine Wirkung; Blocker zuerst beheben.
3. **Ist-Analyse des Texts.** Jeden Absatz gegen die [Chunking-Regeln](/methoden/chunking.md) und die [Anti-Patterns](/referenz/anti-patterns.md) prüfen: Entitäten, Autonomie, Faktendichte, Datumsmarker, bildgebundene Aussagen.
4. **Umbau.** Nach der [Seitenstruktur-Vorlage](/vorlagen/seiten-struktur.md) neu gliedern; Teilfragen aus dem Prompt-Pool ableiten ([Query-Fan-out](/methoden/query-fan-out.md)); Zahlen und Eigendaten ergänzen ([Zitierwürdigkeit](/methoden/zitierwuerdigkeit.md)); Referenzumbau im [Praxisfall](/beispiele/chunk-umbau-praxisfall.md).
5. **Technische Abnahme.** Semantische Tags, echte Tabellen und JSON-LD gegen [Semantisches HTML](/technik/semantisches-html.md) prüfen; Rendering im Server-HTML-Response verifizieren.
6. **Publizieren und registrieren.** Publikationsdatum und URL ins Input-Register eintragen, Format in [Erfolgsmessung](/messung/share-of-mentions.md). Der Registereintrag ist Teil der Publikation, nicht optionaler Nachtrag.
7. **Messfenster und Iteration.** SoM des Clusters über ein festes Fenster gegen die Baseline und die Wettbewerber vergleichen. Da keine Standard-Chunk-Länge existiert, ist der Umbau iterativ: Blöcke mit ausbleibender Extraktion nachschärfen.

# Abgrenzung

Dieses Playbook beschreibt den Ablauf. Verbindliche Freigabe-Gates vor kundensichtbarer Publikation werden ausserhalb des Bundles durchgesetzt; das Bundle liefert die Kriterien, nicht den Zwang.

# Citations

[1] [SoM-Messalgorithmus](/quellen/som-messalgorithmus.md)
[2] [GEO-Infrastruktur und Reputation](/quellen/geo-infrastruktur-reputation.md)
