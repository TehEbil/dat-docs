---
title: "Übersicht aktueller & geplanter Änderungen"
topic_id: "32039"
breadcrumb: "Technische Informationen > Ausgabe Nr. 95 Februar 2026 > Übersicht aktueller & geplanter Änderungen"
---

# Übersicht aktueller & geplanter Änderungen

2026-001 (geplant für Februar 2026)

Schnittstellenfunktionen

| Service | betroffene Funktion | Änderung |
| --- | --- | --- |
| VehicleUserPropertiesService | - | schema-Dateien werden zusammengeführt |
| ValuationVehiclePropertiesService | - | schema-Dateien werden zusammengeführt |
| BatchValuationService (myClaim) | startTask, getTask, cancelTask | entfallen |
| Authentication | authenticateUser | entfällt |
| Authentication | - | Entfernung von schema-Datei (Authentication\_schema1.xsd)  - datCredentials  - datrcbkb  - datrcpda  - baseBusinessObject  - datrcpkk  - datrcpan  - authenticationMethod  - httpMethodEnum  - interfaceType  - authorizationErrorCode  - localDateTime |

2026-002 (geplant für April 2026)

Erweiterung von VXS-Feldern

| übergeordneter Node | Name des VXS-Elements |
| --- | --- |
| Dossier.RepairCalculation.ProcedureRelatedParameters.EuroLacquerFactor | materialIndexPreparation |
| Dossier.RepairCalculation.ProcedureRelatedParameters.EuroLacquerFactor | materialIndexComponents |
| Dossier.RepairCalculation.ProcedureRelatedParameters.EuroLacquerFactor | isSurchargeForMatt |
| Dossier.RepairCalculation.ProcedureRelatedParameters.EuroLacquerFactor | isSurchargeForMattSmallParts |
| Dossier.RepairCalculation.ProcedureRelatedParameters.EuroLacquerFactor | lacquerTechnique |
| Dossier.RepairCalculation.RepairPositions.RepairPosition | LacquerStoneChipProtection |
| Dossier.RepairCalculation.RepairPositions.RepairPosition | LacquerCorrosionProtection |
| Dossier.RepairCalculation.RepairPositions.RepairPosition | LacquerHardshipAllowance |
| Dossier.RepairCalculation.RepairPositions.RepairPosition | LacquerPrePaintingComponents |
| Dossier.RepairCalculation.CalcResultCommon | LacquerPriceVersion |
| Dossier.RepairCalculation.CalcResultCommon | LacquerPriceDate |
| Vehicle.TechInfo | BatteryCapacityNet |
| Vehicle.TechInfo | BatteryCapacityGross |

Entfernung von VXS-Feldern

| übergeordneter Node | Name des VXS-Elements |
| --- | --- |
| Dossier.RepairCalculation.ProcedureRelatedParameters.EuroLacquerFactor | materialPerPointCost |
| Dossier.RepairCalculation.ProcedureRelatedParameters.EuroLacquerFactor | isLacquerPlasticWhenFitted |
| Dossier.RepairCalculation.RepairPositions.RepairPosition | LacquerScratchProofFinishTime |
| Dossier.RepairCalculation.CalcResultCommon.LacquerPositions.LacquerPosition | MaterialPoints |

Schnittstellenfunktionen

| Service | betroffene Funktion | Änderung |
| --- | --- | --- |
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
