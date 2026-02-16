---
title: "Protokolle MaterialProtocol LabourProtocol LacquerProtocol"
topic_id: "2904"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Protokolle MaterialProtocol LabourProtocol LacquerProtocol"
---

# Protokolle MaterialProtocol LabourProtocol LacquerProtocol

| Element | Typ | Beschreibung |
| --- | --- | --- |
| InvalidProcesses | repairProcessList | keine Daten für aktuelles Fahrzeug |
| UnspecificProcesses | repairProcessList | Daten für andere Baueziten o. Ausstattungen |
| PartOfCombinationProcesses | repairProcessList | Eingaben, Teil einer Kombination |
| PartOfOtherProcesses | repairProcessList | Eingaben, Teile anderer Prozesse |
| RemovedByCompositeProcesses | repairProcessList | Prozesse, die durch interne Logik entfernt wurden |
| MissingLacquerInformationProcesses | repairProcessList | Fehlende Lack-Informationen |

repairProcessList

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DATProcessId | integer | Datenverarbeitungsnummer (DVN) |
| RepairType | string | Reparaturart, numerisch |
