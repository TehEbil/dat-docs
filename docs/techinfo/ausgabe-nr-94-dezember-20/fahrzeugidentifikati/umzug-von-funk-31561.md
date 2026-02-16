---
title: "Umzug von Funktionen"
topic_id: "31561"
breadcrumb: "Technische Informationen > Ausgabe Nr. 94 Dezember 2025 > Fahrzeugidentifikation > Erweiterungen > Umzug von Funktionen"
---

# Umzug von Funktionen

Im Zusammenhang mit der Verwendung der zentralen Schemadatei vxs.xsd mussten wir drei Funktionen aus dem ConversionFunctionsService inkompatibel ändern. Wir verschieben gleichzeitig diese Funktionen in den VehicleSelectionService, damit wir den ConversionFunctionsService ohne Bezug zur vxs.xsd erhalten.

Betroffene Funktionen:

ConversionFunctionsService (alt)

- getExistingEquipmentN
- getPossibleEquipmentN
- getEquipmentFromManufacturerCodeN

VehicleSelectionService (neu)

- getExistingEquipment
- getPossibleEquipment
- getEquipmentFromManufacturerCode

Bitte stellen Sie Ihre Systeme baldmöglichst um und nutzen die neuen Funktionen aus
dem VehicleSelectionService.
