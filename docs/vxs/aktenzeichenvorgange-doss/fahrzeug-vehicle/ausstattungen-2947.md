---
title: "Ausstattungen VIN-Abfrageergebnis (VINEquipments)"
topic_id: "2947"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > VIN-Daten (VinResult) > Ausstattungen VIN-Abfrageergebnis (VINEquipments)"
---

# Ausstattungen VIN-Abfrageergebnis (VINEquipments)

<VINEquipments > ist ein Unter-Element von <VinResult> und enthält die Liste aller vom Hersteller gelieferten Sonderausstattungen. Sofern
eine Zuordnung vorhanden ist, wird der zugehörige Schlüssel der DAT Ausstattung ebenfalls
ausgegeben. Die Liste der Ausstattungen entspricht den Rohdaten vom Hersteller, es
wird hier durch die DAT keinerlei Überprüfung auf Plausibilität durchgeführt.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| AvNumberDat | Integer | DAT Ausstattungs-Nummer (AV-Code) |
| ManufacturerCode | String | Herstellerschlüssel |
| ShortName | String | Herstellertext |
