---
title: "DAT Europa-Codes aus dem VIN-Abfrage-Ergebnis (VINECode)"
topic_id: "2943"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > VIN-Daten (VinResult) > DAT Europa-Codes aus dem VIN-Abfrage-Ergebnis (VINECode)"
---

# DAT Europa-Codes aus dem VIN-Abfrage-Ergebnis (VINECode)

<VINECodes> ist ein Unter-Element von <VinResult> und enthält die gelieferten DAT €uropa-Codes zur VIN.

<VINECode> ist das Einzelelement.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| Country | string3 | Datenland als ISO-Code (DE, FR, IT usw.) |
| VehicleTypeKey | integer | Fahrzeugart |
| ManufacturerKey | integer | Hersteller |
| VehicleMainTypeKey | integer | Haupttyp |
| VehicleSubTypeKey | integer | Untertyp |
| VehicleSubTypeVariantKey | integer | Untertypvariante |
| ConstructionTimePriceList | integer | Preislisten-Bauzeit |
| Sign | integer | Warscheinlichkeitskennzeichen siehe VIN-Beschreibung |
| ConstructionTimeMin | integer | Beginnbauzeit des Fahrzeugtyps |
| ConstructionTime | integer | Produktionsbauzeit des Fahrzeugs |
| ConstructionTimeEdge | integer |  |
| ConstructionTimeProd | integer |  |
| VINContainers |  | [s. VINContainers](mogliche-conta-2945.md) |
