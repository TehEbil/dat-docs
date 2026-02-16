---
title: "Schnittstellenoperationen für die Fahrzeugauswahl"
topic_id: "1884"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Aufbau einer Fahrzeugauswahl > Schnittstellenoperationen für die Fahrzeugauswahl"
---

# Schnittstellenoperationen für die Fahrzeugauswahl

Nachfolgend nun eine Übersicht über die notwendigen Schnittstellen-Funktionen, um
die einzelnen Schlüssel zu erhalten:

| DAT €uropa-Code® und Marktindex | Element im Suchbaum | Operation | PKW | Gelände-  fahrzeug | Trans-  porter | Kraftrad | LKW |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 01 | Fahrzeugart | getVehicleTypes | x | x | x | x | x |
| 01 570 | Hersteller | getManufacturers | x | x | x | x | x |
| 01 570 032 | Haupttyp | getBaseModels | x | x | x | x | x |
| 01 570 032 012 | Untertyp | getSubModels | x | x | x | x | x |
|  | Motor | getEngineOptions | x | x | x | x | x |
|  | Karosserie | getBodyOptions | x | x | x | x |  |
|  | Bauart | getConstructionOptions |  |  |  |  | x |
|  | Getriebe | getGearingOptions | x | x | x |  | x |
|  | Radstand | getWheelbaseOptions |  | x | x |  | x |
|  | Antriebsart | getPropulsionOptions |  | x | x |  |  |
|  | Anzahl Achsen | getAxleOptions |  |  |  |  | x |
|  | Fahrerhaus | getDrivingCabOptions |  |  |  |  | x |
|  | Tonnage | getMaximumTotalWeightOptions |  |  |  |  | x |
|  | Federungsart | getSuspensionOptions |  | x | x | x | x |
|  | Ausstattungslinie | getEquipmentLineOptions | x |  |  |  |  |
| 01 570 032 012 0006 | Typvariante (Zusammenstellen des  DAT €uropa-Code®) | compileDatECode | x | x | x | x | x |
| 01 570 032 012 0006 DE005 | (DAT) Container | getPriceDiscoveryContainers | x | x | x | x | x |
| 01 570 032 012 0006 DE005 4330 | Bauzeitraum | getConstructionPeriods | x | x | x | x | x |
