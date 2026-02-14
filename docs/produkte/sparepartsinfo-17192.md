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
| [possibleNames](#showid/17213 "SparePartsName") | complexType, [SparePartsName](#showid/17213 "SparePartsName") | Mögliche Namen |
| [previousPrices](#showid/17209 "PreviousPrices") | complexType, [PreviousPrices[]](#showid/17209 "PreviousPrices") | Vorherige Preise |
| previousPartNumbers | complexType, [previousPartNumber](#showid/22890 "PreviousPartNumber")[] | Enthält die vorherigen Ersatzteilnummern, die in Verwendung waren. |
| repairSet | complexType, RepairSet | Reparaturset |
| finisNumber | Boolean | Rückgabe, ob es sich um eine FINIS-Ersatzteilnummer oder um eine Ford-Katalognummer handelt. |
