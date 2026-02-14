---
title: "constructionTime2Date"
topic_id: "2033"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Konvertierungsoperationen > constructionTime2Date"
---

# constructionTime2Date

Beschreibung

Ermittelt aus einer DAT-kodierten Bauzeitangabe das Datum. Zur Erleichterung des Umgangs
mit Bauzeitangaben kann die Operation constructionTime2Date genutzt werden, die eine Bauzeitangabe in ein Datums-Format konvertiert.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| constructionTime | Integer | DAT-Notation Bauzeit | Bauzeit | X |

Rückgabe

Die Rückgabe erfolgt als Datums-Format. Bei leerem Übergabe-Parameter wird der Wert
1969-12-01T00:00:00.000+01:00 zurückgeliefert.

WSDL

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>?wsdl

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | services | ConversionFunctionsService |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | services | ConversionFunctionsService |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | services | ConversionFunctionsService |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | soap | ConversionFunctionsService |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | soap | ConversionFunctionsService |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | soap/v2 | ConversionFunctionsService |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | soap/v2 | ConversionFunctionsService |
