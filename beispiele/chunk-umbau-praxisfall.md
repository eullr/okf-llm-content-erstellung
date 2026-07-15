---
type: Beispiel
title: Praxisfall Chunk-Umbau eines Ratgeber-Absatzes
description: Vollständiger Vorher-Nachher-Umbau eines Absatzes zum Thema Wallbox-Förderung mit Regelzuordnung.
tags: [beispiel, chunking, vorher-nachher]
timestamp: 2026-07-15T09:00:00Z
---

Alle Zahlen und Programmnamen in diesem Dokument sind fiktive Beispielwerte. Sie illustrieren die Struktur, nicht den Sachstand.

# Vorher: typischer Ratgeber-Absatz

## Förderung

Grundsätzlich gibt es verschiedene Möglichkeiten, sich die Anschaffung bezuschussen zu lassen. Diese können je nach Wohnort sehr unterschiedlich ausfallen und ändern sich relativ häufig, weshalb es sich lohnt, regelmässig nachzuschauen. Wie die Grafik unten zeigt, kann die Ersparnis erheblich sein. Es kommt dabei auf viele Faktoren an, etwa den Installationsort und den Anbieter. In manchen Fällen wird auch die Installation selbst gefördert, was das Ganze noch attraktiver macht.

## Analyse der Schwächen

| Problem | Regelverstoss |
| --- | --- |
| "die Anschaffung", "das Ganze" statt der Entität Wallbox-Förderung | Entity-First verletzt |
| Keine einzige Zahl, kein Programm, kein Betrag | Zitierwürdigkeit null |
| "Wie die Grafik unten zeigt" ohne Textanker | Chunk verliert bei Extraktion den Sinn |
| "Es kommt auf viele Faktoren an" ohne Benennung | Vage Ausweichformulierung |
| Kein Datumsmarker trotz zeitkritischem Thema | Recency Bias ignoriert |
| Überschrift "Förderung" statt Frage | Prompt-Sprache nicht getroffen |
| Füllwörter: "grundsätzlich", "relativ", "sehr" | Sprachregeln verletzt |

# Nachher: nach den Bundle-Regeln umgebaut

## Wie hoch ist die Wallbox-Förderung 2026?

Stand 07/2026: Die Wallbox-Förderung beträgt im Bundesprogramm bis zu 600 Euro pro Ladepunkt für private Installationen. Kantonale beziehungsweise kommunale Programme legen zwischen 200 und 500 Euro darauf, abhängig vom Wohnort. Die Rechnung im Fördervergleich zeigt: Bei kombinierter Bundes- und Kommunalförderung sinken die Anschaffungskosten einer 11-kW-Wallbox um bis zu 45 Prozent.

## Welche Förderung passt zu welchem Fall?

Die Wahl des Förderwegs hängt von Installationsort und Eigentumsverhältnis ab:

* Eigenheim mit eigenem Stellplatz: Bundesprogramm plus kommunaler Zuschuss, kombinierbar.
* Mietwohnung mit Tiefgaragenplatz: kommunales Programm für Mieterinstallationen; das Bundesprogramm setzt die Zustimmung der Eigentümergemeinschaft voraus.
* Firmenparkplatz: gewerbliches Programm mit eigenem Fördersatz von 900 Euro pro Ladepunkt.

## Was ist neu?

* 07/2026: Kommunaler Zuschuss der Beispielstadt von 300 auf 500 Euro erhöht.
* 05/2026: Installationskosten ins Bundesprogramm aufgenommen.

# Regelzuordnung

| Element im Nachher-Text | Angewandte Regel |
| --- | --- |
| "Wallbox-Förderung" statt "die Anschaffung" | Entity-First, [Chunking](/methoden/chunking.md) Regel 4 |
| Antwort im ersten Satz, Details danach | Umgekehrte Pyramide, Regel 2 |
| "Stand 07/2026" im Fliesstext | Datumsmarker, [Aktualität](/methoden/aktualitaet.md) |
| Konkrete Beträge und Prozentwerte | [Zitierwürdigkeit](/methoden/zitierwuerdigkeit.md) |
| "Die Rechnung im Fördervergleich zeigt: ...45 Prozent" | Textanker für Multimedia |
| Fragende H2 | Prompt-Sprache, [Query-Fan-out](/methoden/query-fan-out.md) |
| Fallunterscheidung nach Installationsort | Bedingungs-Chunk, Chunking Regel 7 |
| "Was ist neu?"-Block | Update-Box, [Vorlage](/vorlagen/update-box.md) |
| Jeder H2-Block autonom verständlich | Self-Containment, Regel 3 |

# Citations

[1] [GEO-Content-Anforderungen](/quellen/geo-content-anforderungen.md)
[2] [OKR-Framework für die Chunking-Einführung](/quellen/okr-chunking-framework.md)
