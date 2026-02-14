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
| [sparePartsInformations](sparepartsinfo-17190.md) | complexType, [SparePartsInformations](sparepartsinfo-17190.md) | Informationen über die Ersatzteilnummer |
| [sparePartsVehicles](sparepartsvehi-17199.md) | complexType, [SparePartsVehicles](sparepartsvehi-17199.md) | Informationen über die Fahrzeuge, an dem die Ersatzteilnummer verbaut werden kann |
| [equipments](equipmentlist-17216.md) | complexType, [EquipmentList](equipmentlist-17216.md) | Austattungen mit Beschreibungen, die für diese Ersatzteilnummer und die aufgelistete Fahrzeuge relevant sind. |
