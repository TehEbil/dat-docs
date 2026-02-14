---
title: "Responsebeschreibung getVehicleApproximateValue"
topic_id: "15424"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Annäherungsbewertung > Responsebeschreibung getVehicleApproximateValue"
---

# Responsebeschreibung getVehicleApproximateValue

Die Responseparameter können Sie unter dem Kapitel [Datenaustausch](datenstruktur-1791.md) einsehen. In der Tabelle werden nur spezielle Rückgabewerte der Funktion getVehicleApproximateValue aufgelistet.

| Parameter | Datentyp | Beschreibung |
| --- | --- | --- |
| IdentificationSource | String | Folgende Rückgabewerte sind möglich für diesen Parameter: DATECODE, KBA, NATIONALCODE |
| DATEquipmentId | Integer | Hier können 0-n DAT AV-Nummern der [klassifizierenden Ausstattung](../dat-uropa-code-fah/klassifizieren-1820.md) übergeben werden. Die Übergabe von Sonderausstattungen ist nicht möglich! |
| datECode | String | DAT €uropa-Code® Schlüssel ist abhängig von Kilometerstand, Bauzeit, Erstzulassung, Marktindex. |
| kba | String | HSN/TSN-Schlüssel; Wenn Sie meherere KBA Parameter angeben, werde mehrere Fahrzeuge angezeigt. |
| nationalCode | String | Österreichischer Nationalcode (NatCode); Nur für das Datenland Österreich zulässig. |
| container | Integer | Marktindex wird nur in Verbindung mit dem Parameter DAT €uropa-Code® gesetzt. |
| constructionTimeFrom | Integer | Bauzeit von; in DAT-Notation (als Filter für die Rückgabe) |
| constructionTimeTo | Integer | Bauzeit bis; in DAT-Notation (als Filter für die Rückgabe) |
| constructionTime | Integer | Bauzeit wird nur in Verbindung mit DAT €uropa-Code® und Marktindex gesetzt. Bauzeit in DAT-Notation. |
| mileage | Integer | Kilometerangabe; Wird das Feld nicht gefüllt, wird die Bezugsfahrstrecke verwendet. |
| registrationDate | Date | Erstzulassung (EZL). Ist der Parameter mileage nicht gefüllt, wird die EZL benutzt, um die Bezugsfahrstrecke zu ermitteln. Die Bezugsfahrstrecke wird anhand von registrationDate und Fahrzeugart berechnet. |
| devaluationType | String | Abwertungsart der Ausstattungen |
| vatType | String | Besteuerungsart. Wird kein Wert oder ein falscher Wert übergeben, wird mit der Differenzbesteuerung bewertet. |
