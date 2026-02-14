---
title: "valueCode2Description"
topic_id: "2056"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Konvertierungsoperationen > valueCode2Description"
---

# valueCode2Description

Beschreibung

Die Funktion ermittelt anhand des DAT €uropa-Code® + Marktindex die Beschreibung für jeden Bestandteil des DAT €uropa-Code® und die Liste der klassifizierenden Ausstattungsvarianten (clfAvList).

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| datECode | String | DAT €uropa-Code® | Gültiger DAT €uropa-Code® | X |
| container | String | Marktindex | Gültiger Marktindex | X |

Rückgabe

Zurückgegeben werden folgende Werte:

| Name | Beschreibung |
| --- | --- |
| baseModelLabeling | Haupttypbezeichung |
| containerLabeling | Marktindex-Bezeichnung |
| manufacturerLabeling | Hersteller-Bezeichnung |
| subModelLabling | Untertyp-Bezeichnung |
| vehicleTypeLabling | Fahrzeugtyp-Bezeichnung |
| equipmentLabeling | Ausstattungs-Bezeichnung |
| equipmentClassification | Bezeichnung der klassifizierenden Ausstattung |
| equipmentNumber | DAT-AV-Code |

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
