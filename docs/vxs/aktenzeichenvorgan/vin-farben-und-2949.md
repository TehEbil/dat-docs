---
title: "VIN Farben und Innenausstattungen (VINColor)"
topic_id: "2949"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > VIN-Daten (VinResult) > VIN Farben und Innenausstattungen (VINColor)"
---

# VIN Farben und Innenausstattungen (VINColor)

< VINColors> ist ein Unter-Element von <VinResult> und enthält die gelieferten DAT €uropa-Code® zur Vehicle identification number (VIN).

<VINColor> ist das Einzelelement.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| ColorID | String | DAT-interne Gruppierung |
| Code | String | alphanumerische Herstellerangaben |
| Description | String | Herstellerbeschreibung |
| PaintType | String | interner Schlüssel der Lackart (siehe: [LacquerType aus RepairParameters](../wertelisten/lackart-lacque-1342.md)) |
| CountCoat | String | Anzahl Schichten |
