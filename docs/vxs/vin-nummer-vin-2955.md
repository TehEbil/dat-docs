---
title: "VIN-Nummer (VINumber)"
topic_id: "2955"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > VIN-Daten (VinResult) > VIN-Nummer (VINumber)"
---

# VIN-Nummer (VINumber)

< VINumber > ist ein Unter-Element von < VINVehicle >. Hier wird die Vehicle identification number (VIN) dargestellt. Ist dieses Feld
leer, ist keine VIN-Abfrage durchgeführt worden. Für die weitere Verarbeitung sollte
die VIN aus dem Container [Vehicle](#showid/6692 "Fahrzeug (Vehicle)") genommen werden.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| VinCode | string | Die VIN-Nummer, DAT-internes Feld |
| OrderCode | string |  |
| Manufacturer | string |  |
