---
title: "SparePartsResultPerSparePartNumber"
topic_id: "17205"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Datentypen > SparePartsResultPerSparePartNumber"
---

# SparePartsResultPerSparePartNumber

| Attribut | Typ | Beschreibung |
| --- | --- | --- |
| pageSize | Integer | Anzahl der Ergebnisse pro Seite (Der maximale Wert ist 100) |
| pageNumber | Integer | Seitennummer der Ergebnisliste (Offset) |
| partNumberInput | String | Beinhaltet die angegebene Ersatzteilnummer aus der Anfrage. |
| partNumber | String | Ersatzteilnummer |
| datProcessNumber | Long | Enthält die entsprechende DAT-Verarbeitungsnummer (DVN) |
| vehiclesFound | Integer | Anzahl der gefundenen Fahrzeuge, an dem die Ersatzteilnummer verbaut werden kann |
| vehiclesReturned | Integer | Anzahl der zurückgegebenen Fahrzeuge, an dem die Ersatzteilnummer verbaut werden kann |
| [sparePartsInformations](#showid/17190 "SparePartsInformations") | complexType, [SparePartsInformations](#showid/17190 "SparePartsInformations") | Informationen über die Ersatzteilnummer |
| [sparePartsVehicles](#showid/17199 "SparePartsVehicles") | complexType, [SparePartsVehicles](#showid/17199 "SparePartsVehicles") | Informationen über die Fahrzeuge, an dem die Ersatzteilnummer verbaut werden kann |
| [equipments](#showid/17216 "EquipmentList") | complexType, [EquipmentList](#showid/17216 "EquipmentList") | Austattungen mit Beschreibungen, die für diese Ersatzteilnummer und die aufgelistete Fahrzeuge relevant sind. |

Bitte beachten Sie, dass der Unterschied zwischen den Elementen partNumber und partNumberInput darin liegt, dass partNumber die aktuell verwendete Ersatzteilnummer enthält und partNumberInput die Ersatzteilnummer, die in der Anfrage eingegeben wurde. Falls die Anfrage eine
veraltete Ersatzteilnummer enthält, erscheint diese in der Antwort unter partNumberInput und die aktuelle Ersatzteilnummer des entsprechenden Teils wird wie gewohnt unter
partNumber angezeigt, ansonsten enthalten beide Felder die gleiche Ersatzteilnummer.
