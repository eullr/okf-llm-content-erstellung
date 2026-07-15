---
type: Referenz
title: Anti-Patterns
description: Muster, die die GEO-Wirkung zerstören oder Texte als maschinell erzeugt entlarven.
tags: [referenz, anti-patterns, ki-floskeln, qualitaet]
timestamp: 2026-07-15T09:00:00Z
---

# Strukturelle Anti-Patterns

1. **Mechanischer Schnitt.** Blöcke rein nach Zeichenlänge trennen, ohne Entitäts- und Sinnbezug. Folge: Chunks ohne zuordenbare Bedeutung, Negativbeispiel in [Semantisches Chunking](/methoden/chunking.md).
2. **Q&A-Übersteuerung.** Den gesamten Text in Frage-Antwort-Paare zerhacken. Maschinen können damit arbeiten, menschliche Leser springen ab; Fliesstext mit klarer innerer Logik bleibt chunkbar.
3. **Bildgebundene Aussagen.** Kernaussagen nur in Grafiken oder Rechnern transportieren ("wie die Abbildung zeigt"). Ohne Textanker verliert der Block bei der Extraktion seinen Sinn.
4. **Timestamp-Gaming.** Veröffentlichungsdatum ändern ohne substanzielles Update. Erkennbar und voraussichtlich zunehmend abgestraft, siehe [Aktualität](/methoden/aktualitaet.md).
5. **Tabellen aus div-Containern.** Visuell eine Tabelle, im Code keine; für die Extraktion unbrauchbar, siehe [Semantisches HTML](/technik/semantisches-html.md).

# Sprachliche Anti-Patterns (maschinelle Fussabdrücke)

Diese Muster markieren Texte als LLM-generiert und senken sowohl das Leservertrauen als auch die Differenzierung gegenüber massenhaft generierter Konkurrenz.

1. **KI-Floskelvokabular.** Gesperrte Wörter und Wendungen: "nahtlos", "eintauchen", "entscheidend", "Pionier", "bahnbrechend", "begeistern", Komposita auf "-landschaft" (Themenlandschaft, Toollandschaft), "Oase", "besticht durch", "steht als Symbol für", "atemberaubend", "perfekt abgerundet", "Zusätzlich" am Satzanfang.
2. **Leere Abschlussformeln.** "Zusammenfassend lässt sich sagen", "insgesamt zeigt sich": Sätze ohne neue Information, reiner Rauschanteil.
3. **Elegante Variation.** Künstliche Synonyme für Kernbegriffe erfinden, um Wiederholung zu vermeiden. Zerstört das Entity-First-Prinzip: Die Entität muss beim Namen genannt werden, konsequent gleich.
4. **Falsche Spannweiten.** Konstruktionen "von X bis Y" ohne echte Skala dahinter ("von der Planung bis zur Umsetzung").
5. **Gedankenstrich- und Fettdruck-Inflation.** Hohe Dichte an Gedankenstrichen und fett markierten Halbsätzen ist ein typografischer Marker maschineller Texte.
6. **Vage Ausweichformulierungen.** "Es kommt auf viele Faktoren an" ohne Benennung der Faktoren. Gegenmittel ist konstruktive Unsicherheit, siehe [Sprache und Formulierung](/methoden/sprache-formulierung.md).

# Prozessuale Anti-Patterns

1. **Umbau ohne Baseline.** Seiten umschreiben, bevor der Ausgangs-SoM gemessen wurde. Der Effekt ist danach nicht mehr belegbar, siehe [Playbook Seiten-Umbau](/playbooks/seiten-umbau.md).
2. **Positionsgläubigkeit.** Die Position der Markennennung in der Antwort als Erfolg werten; ohne Kontext wertlos, siehe [Erfolgsmessung](/messung/share-of-mentions.md).

# Citations

[1] [GEO-Content-Anforderungen](/quellen/geo-content-anforderungen.md)
[2] [SoM-Messalgorithmus](/quellen/som-messalgorithmus.md)
