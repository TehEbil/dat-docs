---
title: "Detailpositionen"
topic_id: "29032"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Bewertungsdaten (Valuation) > Zustand (Condition) > Detailpositionen"
---

# Detailpositionen

<DetailPositionList> enthalt ein Element <DetailPosition>. <DetailPosition> enthält weitere Elemente:

DetailPositionList

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DetailPosition | DetailPosition |  |

DetailPosition

|  |  |  |
| --- | --- | --- |
| Element | Typ | Beschreibung |
| Id | String | Id der Detailposition |
| Description | String | Beschreibung der Detailposition |
| ValueNet | Decimal | Betrag (Netto) |
| ValueGross | Decimal | Betrag (Brutto) |
| BaseValuePercentage | Decimal | Prozent vom Grundwert |
