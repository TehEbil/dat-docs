---
title: "SparePartsResultPerDPN"
topic_id: "17219"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Datentypen > SparePartsResultPerDPN"
---

# SparePartsResultPerDPN

| Attribut | Typ | Beschreibung |
| --- | --- | --- |
| pageSize | Integer | Anzahl der Ergebnisse pro Seite (Der maximale Wert ist 100) |
| pageNumber | Integer | Seitennummer der Ergebnisliste (Offset) |
| datProcessNumber | Long | DVN-Nummer |
| vehiclesFound | Integer | Anzahl der gefundenen Fahrzeuge, an dem die Ersatzteilnummer verbaut werden kann |
| vehiclesReturned | Integer | Anzahl der zurückgegebenen Fahrzeuge, an dem die Ersatzteilnummer verbaut werden kann |
| [sparePartsInformations](#showid/17190 "SparePartsInformations") | complexType, [SparePartsInformations](#showid/17190 "SparePartsInformations") | Informationen über die Ersatzteilnummer |
| [sparePartsVehicles](#showid/17199 "SparePartsVehicles") | complexType, [SparePartsVehicles](#showid/17199 "SparePartsVehicles") | Informationen über die Fahrzeuge, an dem die Ersatzteilnummer verbaut werden kann |
| [equipments](#showid/17216 "EquipmentList") | complexType, [EquipmentList](#showid/17216 "EquipmentList") | Austattungen mit Beschreibungen, die für diese Ersatzteilnummer und die aufgelistete Fahrzeuge relevant sind. |
