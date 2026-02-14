---
title: "Abwertungsart DecreaseType"
topic_id: "1390"
breadcrumb: "Datenaustauschformat VXS > Wertelisten > Abwertungsart DecreaseType"
---

# Abwertungsart DecreaseType

Die DAT ordnet den Sonderausstattungen eine jeweilig entsprechende Standardabwertungsart
zu. Diese Zuordnungen und die Abwertungstabellen selbst werden regelmäßig aktualisiert.

Sie überschreiben die Standardeinstellung der DAT, indem Sie eine der nachfolgend
aufgelisteten Abwertungsarten in ihrem Request übergeben.

| Abwertungsart | Kurzschreibweise | Beschreibung |
| --- | --- | --- |
| Residual value | RV | Die Abwertung erfolgt entsprechend dem Restwert des Fahrzeugs (Basiswert) im Vergleich zum Listenneupreis. |
| Table1 | T1 | Die Abwertung erfolgt entsprechend einer Tabelle, die eine Abwertung in Abhängigkeit des Ausstattungsalters beinhaltet. |
| Table2 | T2 | Die Abwertung erfolgt entsprechend einer Tabelle, die eine Abwertung in Abhängigkeit des Ausstattungsalters beinhaltet. Die Tabelle2 wertet stärker ab als die Tabelle1. |
| Table3 | T3 | Die Abwertung erfolgt entsprechend einer Tabelle, die eine Abwertung in Abhängigkeit des Ausstattungsalters beinhaltet. Die Tabelle3 wertet stärker ab als die Tabelle2. |
| Table4 | T4 | Die Abwertung erfolgt entsprechend einer Tabelle, die eine Abwertung in Abhängigkeit des Ausstattungsalters beinhaltet. Die Tabelle4 wertet stärker ab als die Tabelle3. |
| DEFAULT TABLE | DT | Die Abwertung erfolgt entsprechend der Standardabwertungsart. |
| VV | \_ | Spezielle Abwertungstabelle für Österreich. Diese ist nur in Verbindung mit datCountryIndicator='AT' verwendbar. |
| Percentage | Percentage | Die Abwertung erfolgt prozentuell vom Basiswert. |
| Equipment Percentage | EquipPercentage | Die Abwertung erfolgt prozentual vom Neupreis der Sonder- bzw. Zusatzausstattung. |
