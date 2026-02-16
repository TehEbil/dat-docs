---
title: "Übersicht geplanter Änderungen"
topic_id: "31044"
breadcrumb: "Technische Informationen > Ausgabe Nr. 93 September 2025 > Übersicht geplanter Änderungen"
---

# Übersicht geplanter Änderungen

2025-005 (geplant für Oktober 2025)

Entfernung von VXS-Feldern

| übergeordneter Node | Name des VXS-Elements |
| --- | --- |
| Dossier.Vehicle | VehicleTypeName |
| ContainerName |
| Dossier.Vehicle.TechInfo | Drive |
| Dossier.Vehicle.Equipment | SpecialEditionPackageName |

Information: Die Entfernung der Emissionsklasse (EmissionClass) musste verschoben werden, da das alternative Feld (EmissionClassN) noch nicht umfassend im VXS-Export verfügbar ist.

Schnittstellenfunktionen

| Service | betroffene Funktion | Änderung |
| --- | --- | --- |
| Oberflächenintegration der valuateExpert | - | Änderung im Aufruf |
| VehicleSelection | getBaseModels | entfällt |
| https://www.dat.de | getSystemStatus.json | neue Schnittstellenfunktion zum Abruf des DAT Systemstatus |

2025-006 (geplant für Dezember 2025)

Schnittstellenfunktionen

| Service | betroffene Funktion | Änderung |
| --- | --- | --- |
| TradingServiceN | - | doppelte Elemente werden aus der schema1-Datei entfernt |
| https://www.dat.de/VehicleRepairOnline/services/VehicleRepairService?wsdl, https://www.dat.de/myClaim/soap/v2/VehicleRepairService?wsdl | calculate | entfällt |
| https://www.dat.de/VehicleRepairOnline/services/VehicleRepairService?wsdl | getCalculationResults | entfällt |
| https://www.dat.de/GlassRep/services?wsdl |  | entfällt |

2026-001 (geplant für Februar 2026)

Schnittstellenfunktionen

| Service | betroffene Funktion | Änderung |
| --- | --- | --- |
| VehicleUserPropertiesService | - | schema-Dateien werden zusammengeführt |
| ValuationVehiclePropertiesService | - | schema-Dateien werden zusammengeführt |
| BatchValuationService (myClaim) | startTask, getTask, cancelTask | entfallen |
| Authentication | authenticateUser | entfällt |
| Authentication | - | Entfernung von schema-Datei (Authentication\_schema1.xsd)  - datCredentials  - datrcbkb  - datrcpda  - baseBusinessObject  - datrcpkk  - datrcpan  - authenticationMethod  - httpMethodEnum  - interfaceType  - authorizationErrorCode  - localDateTime |

2026-003 (geplant für Juni 2026)

Entfernung von VXS-Feldern

| übergeordneter Node | Name des VXS-Elements |
| --- | --- |
| Dossier.Vehicle.TechInfo | EmissionClass |

Schnittstellenfunktionen

| Service | betroffene Funktion | Änderung |
| --- | --- | --- |
| Dossier1N | searchDossierList, searchDossierListN | Anpassung einer Fehlermeldung |
| DossierN | searchDossierList, searchDossierListN | Anpassung einer Fehlermeldung |
