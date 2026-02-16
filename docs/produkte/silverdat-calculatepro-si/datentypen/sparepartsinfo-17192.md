---
title: "SparePartsInformation"
topic_id: "17192"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Datentypen > SparePartsResultPerSparePartNumber > SparePartsInformations > SparePartsInformation"
---

# SparePartsInformation

| Attribut | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Name Ersatzteilnummer |
| partNumber | String | Ersatzteilnummer |
| price | BigDecimal | Preis Ersatzteilnummer |
| priceDate | String | Preisdatum |
| amount | Integer | Betrag, nur für Reparaturset |
| workTimeMin | Decimal | Enthält die kleinste Arbeitszeit für das entsprechende Ersatzteil. |
| workTimeMax | Decimal | Enthält die größte Arbeitszeit für das entsprechende Ersatzteil |
| orderable | String | Bestellbar |
| [possibleNames](sparepartsname-17213.md) | complexType, [SparePartsName](sparepartsname-17213.md) | Mögliche Namen |
| [previousPrices](previousprices-17209.md) | complexType, [PreviousPrices[]](previousprices-17209.md) | Vorherige Preise |
| previousPartNumbers | complexType, [previousPartNumber](previouspartnu-22890.md)[] | Enthält die vorherigen Ersatzteilnummern, die in Verwendung waren. |
| repairSet | complexType, RepairSet | Reparaturset |
| finisNumber | Boolean | Rückgabe, ob es sich um eine FINIS-Ersatzteilnummer oder um eine Ford-Katalognummer handelt. |
