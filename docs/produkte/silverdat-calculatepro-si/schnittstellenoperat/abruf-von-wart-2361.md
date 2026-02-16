---
title: "Abruf von Wartungsintervallen: getMaintenanceIntervals"
topic_id: "2361"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abruf von Wartungsintervallen: getMaintenanceIntervals"
---

# Abruf von Wartungsintervallen: getMaintenanceIntervals

getMaintenanceIntervals ist eine Funktion zum Abrufen von Wartungsintervallen zu einem Fahrzeug.

Parameter

Als Eingabe dienen dabei der DAT €uropa-Code® (datECode), die Bauzeit (constructionTime) und die Locale (locale), wie im Kapitel [Element locale](../../../allgemein/dat-developers-guide/arbeiten-mit-den-web/element-locale-1352.md) beschrieben.

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| constructionTime | Integer, Pflicht |  | Bauzeit nach DAT-Notation, 4stellig |
| datECode | String, Pflicht |  | Gültiger DAT €uropa-Code |
| equipment | Long, optional |  | AV. Verfügbare Ausstattungen; mehrfach Auflistung möglich |
| locale | Locale, optional |  | [Element locale](../../../allgemein/dat-developers-guide/arbeiten-mit-den-web/element-locale-1352.md) |

Rückgabe

Als Rückgabe wird ein so genanntes „Fahrzeugdossier" zurückgeliefert. Dieses Dossier
ist im VXS-Format gehalten. Folgende Informationsblöcke werden zusätzlich zurückgegeben.
Die detaillierte Beschreibung des VXS-Formats und seiner Felder finden Sie im Kapitel "VXS":

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [Dossiers](../../../vxs/aktenzeichenvorgange-doss/index.md) | [Dossiers](../../../vxs/aktenzeichenvorgange-doss/index.md) | Enthält das Berechnungsergebnis inklusive aller sonstigen Informationen wie z.B. Ölfüllstandsmengen etc. |

```
Dossier
    DatCustomerAddress
    Vehicle
        RegistrationData
        Engine
        TechInfo
            FillingQuantities
        Equipment
    RepairWages
    RepairParameters
    CalcResultCommon
        RepairCalculationSummary
        CalculationSummary
    MaintenanceInterval
        MaintenancePositions
            MaterialPositions
```
