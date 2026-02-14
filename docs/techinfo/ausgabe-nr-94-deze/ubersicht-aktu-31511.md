---
title: "Übersicht aktueller & geplanter Änderungen"
topic_id: "31511"
breadcrumb: "Technische Informationen > Ausgabe Nr. 94 Dezember 2025 > Übersicht aktueller & geplanter Änderungen"
---

# Übersicht aktueller & geplanter Änderungen

2025-006 (geplant für Dezember 2025)

Schnittstellenfunktionen

| Service | betroffene Funktion | Änderung |
| --- | --- | --- |
| TradingServiceN | - | doppelte Elemente werden aus der schema1-Datei entfernt |
| VehicleSelectionService | Neu: getExistingEquipment  getPossibleEquipment  getEquipmentFromManufacturerCode | Funktionen wurden aus dem ConversionFunctionsService verschoben |

Neue VXS-Felder

| übergeordneter Node | Name des VXS-Elements |
| --- | --- |
| Dossier.Vehicle.RegistrationData | BaseNumberN (Länge 12, ersetzt BaseNumber mit Länge 9) |

2026-001 (geplant für Februar 2026)

Schnittstellenfunktionen

| Service | betroffene Funktion | Änderung |
| --- | --- | --- |
| VehicleUserPropertiesService | - | schema-Dateien werden zusammengeführt |
| ValuationVehiclePropertiesService | - | schema-Dateien werden zusammengeführt |
| BatchValuationService (myClaim) | startTask, getTask, cancelTask | entfallen |
| Authentication | authenticateUser | entfällt |
| Authentication | - | Entfernung von schema-Datei (Authentication\_schema1.xsd)  - datCredentials  - datrcbkb  - datrcpda  - baseBusinessObject  - datrcpkk  - datrcpan  - authenticationMethod  - httpMethodEnum  - interfaceType  - authorizationErrorCode  - localDateTime |
| https://www.dat.de/VehicleRepairOnline/services/VehicleRepairService?wsdl, https://www.dat.de/myClaim/soap/v2/VehicleRepairService?wsdl | calculate | entfällt |
| https://www.dat.de/VehicleRepairOnline/services/VehicleRepairService?wsdl | getCalculationResults | entfällt |
| https://www.dat.de/GlassRep/services?wsdl |  | entfällt |

2026-003 (geplant für Juni 2026)

Entfernung von VXS-Feldern

| übergeordneter Node | Name des VXS-Elements |
| --- | --- |
| Dossier.Vehicle.TechInfo | EmissionClass |
| Dossier.Vehicle.RegistrationData | BaseNumber |

Schnittstellenfunktionen

| Service | betroffene Funktion | Änderung |
| --- | --- | --- |
| Dossier1N | searchDossierList, searchDossierListN | Anpassung einer Fehlermeldung |
| DossierN | searchDossierList, searchDossierListN | Anpassung einer Fehlermeldung |
| ConversionFunctionsService | getExistingEquipmentN getPossibleEquipmentN getEquipmentFromManufacturerCodeN | Schnittstellenfunktionen sind seit dem Release 2025-006 abgekündigt und werden aus dem Service entfernt |
