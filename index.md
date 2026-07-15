---
okf_version: "0.1"
bundle_version: "1.2.0"
author: Eugen Ullrich
contact: hi@eullrich.com
visibility: public
license: CC-BY-4.0
license_url: https://creativecommons.org/licenses/by/4.0/deed.de
attribution: "Eugen Ullrich, eullrich.com"
source: https://eullrich.com/okf-bundle-markenwissen
---

# LLM-Content-Erstellung

Wissensbundle für die Erstellung und Umstrukturierung von Web-Inhalten, die von generativen Systemen (ChatGPT, Gemini, Perplexity, AI Overviews) extrahiert, zitiert und erwähnt werden sollen. Sieben Bereiche: redaktionelle Methoden, technische Voraussetzungen, Offpage-Signale, Erfolgsmessung, Playbooks, Beispiele mit Vorlagen und Referenz.

# Methoden

* [Semantisches Chunking](/methoden/chunking.md) - Regeln zur Zerlegung von Inhalten in autonome, extrahierbare Blöcke.
* [Sprache und Formulierung](/methoden/sprache-formulierung.md) - Aktiv, kurz, ohne Füllwörter, mit klaren Bedingungen.
* [Zitierwürdigkeit](/methoden/zitierwuerdigkeit.md) - Zahlen, Eigendaten und Textanker als Grundlage für Grounding.
* [Query-Fan-out abdecken](/methoden/query-fan-out.md) - Teilfragen, Vergleiche und Es-kommt-darauf-an-Szenarien.
* [Aktualität und Recency Bias](/methoden/aktualitaet.md) - Sichtbare Datumsmarker und echte Updates statt Timestamp-Gaming.
* [Autorschaft und E-E-A-T](/methoden/eeat-autorschaft.md) - Autorenboxen und Profilseiten als Vertrauenssignale.

# Technik

* [Crawler-Zugang](/technik/crawler-zugang.md) - Server-HTML statt Client-JavaScript, robots.txt, Firewall, Statuscodes.
* [Semantisches HTML und strukturierte Daten](/technik/semantisches-html.md) - Echte Tabellen, JSON-LD, Cluster-Architektur, Ankertexte.

# Offpage

* [Mentions, Sentiment und Konsistenz](/offpage/mentions-grounding.md) - Externe Erwähnungen als Grounding-Quelle für LLM-Antworten.

# Messung

* [Erfolgsmessung über Share of Mentions](/messung/share-of-mentions.md) - Input-Register, Prompt-Pool, URL-Aggregation, Wettbewerbs-Benchmark.

# Playbooks

* [Seiten-Umbau](/playbooks/seiten-umbau.md) - Sieben Schritte von der SoM-Baseline bis zur Iteration.
* [URL-Priorisierung](/playbooks/url-priorisierung.md) - Auswahlkriterien für die Umbau-Reihenfolge.

# Beispiele und Vorlagen

* [Praxisfall Chunk-Umbau](/beispiele/chunk-umbau-praxisfall.md) - Vollständiger Vorher-Nachher-Fall mit Regelzuordnung.
* [Seitenstruktur](/vorlagen/seiten-struktur.md) - Grundgerüst einer LLM-optimierten Seite.
* [FAQ-Block](/vorlagen/faq-block.md) - Struktur für Query-Fan-out-Abdeckung.
* [Update-Box](/vorlagen/update-box.md) - "Was ist neu?"-Block gegen Recency-Verlust.

# Referenz

* [Glossar](/referenz/glossar.md) - Verbindliche Begriffsdefinitionen und Tool-Terminologie-Mapping.
* [Anti-Patterns](/referenz/anti-patterns.md) - Strukturelle, sprachliche und prozessuale Muster, die Wirkung zerstören.

# Quellen

* [Quellenverzeichnis](/quellen/index.md) - Fünf verdichtete Quellkonzepte mit Verlässlichkeitseinschätzung; Basis aller Citations im Bundle.

# Lizenz

Dieses Bundle steht unter [Creative Commons Namensnennung 4.0 International](https://creativecommons.org/licenses/by/4.0/deed.de) (CC BY 4.0). Sie dürfen es kopieren, weitergeben, verändern und kommerziell einsetzen, solange Sie "Eugen Ullrich, eullrich.com" als Quelle nennen. Bedingungen in [LICENSE.md](/LICENSE.md), Lizenz-Volltext bei Creative Commons.

# Pflege

Ein Konzept gilt als überprüfungsbedürftig, wenn sein timestamp älter als sechs Monate ist oder eine zitierte Quelle sich substanziell geändert hat. Änderungen an Konzepten werden im [Log](/log.md) mit Datum vermerkt; das Glossar und die Tool-Terminologie-Tabelle werden bei jeder Tool-Aufnahme mitgezogen. Kurator ist der Bundle-Autor; Modelle pflegen Inhalte nur auf dessen Freigabe.
