---
title: "Wertdefinitionen anlegen in der Wertermittlung"
topic_id: "11846"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Wertdefinitionen anlegen in der Wertermittlung"
---

# Wertdefinitionen anlegen in der Wertermittlung

Mit der Funktion setValueDefinition legen Sie Wertedefinitionsdaten zu einem bestehenden Vorgang an.

Parameter setValueDefinition

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Einstiegselement, enthält sämtliche Eingabedaten zum Vorgang | numerisch | x |
| ConfirmValue | Boolean | Bestätigung des Verkaufspreises gemäß Festlegung Sachverständiger in Brutto |  |  |
| ExpertDefinedSalesValueGross | Decimal | Verkaufspreis gemäß Festlegung Sachverständiger(Brutto) |  |  |
| RemarkRegardingOtherSource | String | Bemerkung sonstige Quelle |  |  |
| SumAccordingToOtherGross | Decimal | Verkaufspreis aus sonstiger Quelle in Brutto |  |  |
| SumAsOfWebScanGross | Decimal | Verkaufspreis aus webScan in Brutto |  |  |
