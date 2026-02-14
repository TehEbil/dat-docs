---
title: "MaintenanceIntervals (MaintenancePosition)"
topic_id: "1463"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > MaintenanceIntervals (MaintenancePosition)"
---

# MaintenanceIntervals (MaintenancePosition)

MaintenanceInterval

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DATProcessId | Integer | DVN |
| Description | String | Beschreibung |
| MaintenancePositions |  | Optional, s. MaintenancePosition |

MaintenancePosition

| Element | Typ | Beschreibung |
| --- | --- | --- |
| Order | Decimal | Reihenfolge |
| DATProcessId | Integer | DVN |
| RepairType | String | Repaircode |
| Description | String | Beschreibung |
| FootNote | String | Fußnote |
| PositionType | String | Mögliche Werte: X=mandatory, R/Z=additional/optional |
| MaterialPositions |  | Optional, [s. MaterialPosition](#showid/1465 "Material-Positionen (MaterialPosition(s))") |
