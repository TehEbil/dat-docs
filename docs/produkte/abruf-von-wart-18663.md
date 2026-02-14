---
title: "Abruf von Wartungsintervallen: getMaintenanceIntervals"
topic_id: "18663"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abruf von Wartungsintervallen: getMaintenanceIntervals"
---

# Abruf von Wartungsintervallen: getMaintenanceIntervals

getMaintenanceIntervals() ist eine Funktion zum Abrufen von Wartungsintervallen zu einem Fahrzeug.

Parameter

Als Eingabe dienen dabei der DAT €uropa-Code® (datECode), die Bauzeit (constructionTime) und die Locale (locale), wie im Kapitel [Element locale](#showid/1352 "Element locale ") beschrieben.

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| constructionTime | Integer, Pflicht |  | Bauzeit nach DAT-Notation, 4stellig |
| datECode | String, Pflicht |  | Gültiger DAT €uropa-Code |
| equipment | Long, optional |  | AV. Verfügbare Ausstattungen; mehrfach Auflistung möglich |
| locale | Locale, optional |  | [Element locale](#showid/1352 "Element locale ") |

Rückgabe

Als Rückgabe wird ein so genanntes „Fahrzeugdossier" zurückgeliefert. Dieses Dossier
ist im VXS-Format gehalten. Folgende Informationsblöcke werden zusätzlich zurückgegeben.
Die detaillierte Beschreibung des VXS-Formats und seiner Felder finden Sie im Kapitel "VXS":

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [Dossiers](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)") | [Dossiers](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)") | Enthält das Berechnungsergebnis inklusive aller sonstigen Informationen wie z.B. Ölfüllstandsmengen etc. |

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
