---
type: Vorlage
title: FAQ-Block
description: Struktur für die Abdeckung von Sub-Queries am Seitenende, mit Schema-Hinweis.
tags: [vorlage, faq, query-fan-out]
timestamp: 2026-07-15T09:00:00Z
---

# Gerüst

```markdown
## Häufige Fragen zu [Kernentität]

### [Frage exakt in erwartbarer Prompt-Formulierung]?
[Antwort in maximal drei Sätzen. Erster Satz beantwortet die Frage
vollständig. Entität beim Namen nennen.]

### [Frage zu Preis oder Kosten]?
[Konkrete Zahl oder Spanne mit Datumsmarker.]

### [Frage zu Risiken oder typischen Fehlern]?
[Konkretes Risiko plus Gegenmassnahme.]
```

# Verwendungsregeln

* Mindestens drei, höchstens acht Paare; jedes Paar deckt eine reale Sub-Query des Clusters ab, keine Alibi-Fragen.
* Fragen aus dem getrackten Prompt-Pool ableiten, nicht erfinden, siehe [Erfolgsmessung](/messung/share-of-mentions.md).
* Den Block als FAQPage in JSON-LD auszeichnen, siehe [Semantisches HTML](/technik/semantisches-html.md).
