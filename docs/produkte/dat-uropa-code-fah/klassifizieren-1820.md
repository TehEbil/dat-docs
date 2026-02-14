---
title: "Klassifizierende Ausstattungen"
topic_id: "1820"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Klassifizierende Ausstattungen"
---

# Klassifizierende Ausstattungen

Eine Untertypvariante hat bestimmte klassifizierende Ausstattungen. Sie wird damit
bestimmt. Die klassifizierenden Ausstattungen sind abhängig vom Fahrzeugaufbau bzw.
der Fahrzeugklasse. Sie unterscheiden sich NICHT nach der Fahrzeugart.  
Siehe dazu das folgende Schema:

| Klassifizierungsgruppe | GrpNr | PKW | Gel.Wg  / SUV | Kleintrapo/ Transporter | Kraftrad | Lastkraftwagen  /Omnibusse | Caravan | Motorcaravan |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Motor | 1 | X | X | X | X | X |  | X |
| Karosserie | 2 | X | X | X | X |  | X | X |
| Bauart | 7 |  |  |  |  | X |  | X |
| Getriebe | 11 | X | X | X |  |  |  |  |
| Radstand | 3 |  | X | X |  | X |  |  |
| Antriebsart | 4 |  | X | X |  |  |  |  |
| Anzahl Achsen | 9 |  |  |  |  | X | X |  |
| Fahrerhaus | 5 |  |  |  |  | X | X | X |
| Tonnage | 6 |  |  |  |  | X | X | X |
| Federungsart | 8 |  |  |  |  | X |  |  |
| Ausstattungslinie (optional) | 10 | (X) | (X) | (X) | (X) | (X) | (X) | (X) |

Beispiel

| DAT €uropa-Code® | 04-750-053-011-0001 | 01-570-011-008-0001 | 02-905-028-011-0001 | 03-830-013-001-0001 |
| --- | --- | --- | --- | --- |
| Fahrzeugart | LKW | PKW | Transporter | Kraftrad |
| Hersteller | Scania | Mercedes-Benz | Volkswagen | Suzuki |
| Haupttyp | R 143-500 IC 368 KW E2 '95-'96 | BM 124 E-Klasse Lim. (10.1992->) | T5 Bus | GSX 1300 R Hayabusa (WVA) |
| Untertyp | FSAFE/ 3800 / 18,0 / H 4X2 | 400 E / E 420 | Multivan Twenty | GSX 1300 R |
| AV-Kl. - Motor | Motor 14,2 Ltr.-368 kW Diesel | Motor 4,2 Ltr.- 205 kW V8 32V KAT | Motor 1,9 Ltr.- 77 kW TDI KAT (AXB) | Motor 1299 ccm - 129 kW |
| AV-Kl. - Karosserie |  | Karosserie 4-türig | Karosserie/Aufbau: Bus | Motorrad |
| AV-Kl. - Bauart | Karosserie/Aufbau: Sattelzugmaschine |  |  |  |
| AV-Kl. - Getriebe |  | Getriebe Automatik | Getriebe 5-Gang |  |
| AV-Kl. - Radstand | Radstand: 3800 mm |  | Radstand: 3000 mm |  |
| AV-Kl. - Antriebsart |  | Antriebsart: Heckantrieb | Antriebsart: Frontantrieb |  |
| AV-Kl. - Anzahl Achsen | Achskonfiguration: 4X2 |  |  |  |
| AV-Kl. - Fahrerhaus | Fahrerhaus: lang CR 19 A |  |  |  |
| AV-Kl. - Tonnage | Zul. Gesamtgewicht 18,00 t |  |  |  |
| AV-Kl. - Federungsart | Federung: Blatt/Blatt |  |  |  |
| AV-Kl. - Ausstattungslinie |  |  |  |  |

Zugriffsoperationen für die klassifizierenden Ausstattungen

Jede klassifizierende Ausstattungsgruppe hat ihre eigene Aufrufsoperation. Hier die
Darstellung der klassifizierenden Ausstattungsgruppen, der Aufrufsoperation und des
Bezugs zum Fahrzeugaufbau.

| Klassifizierungsgruppe | Operation | Pkw | Gelände-fzg. | Transporter | Kraftrad | Lkw |
| --- | --- | --- | --- | --- | --- | --- |
| 1 | getEngineOptions | X | X | X | X | X |
| 2 | getCarBodyOptions | X | X | X | X |  |
| 7 | getConstructionOptions |  |  |  |  | X |
| 11 | getGearingOptions | X | X | X |  |  |
| 3 | getWheelBaseOptions |  | X | X |  | X |
| 4 | getTypeOfDriveOptions |  | X | X |  |  |
| 9 | getNumberOfAxleOptions |  |  |  |  | X |
| 5 | getDriversCabOptions |  |  |  |  | X |
| 6 | getGrossVehicleWeightOptions |  |  |  |  | X |
| 8 | getSuspensionOptions |  |  |  |  | X |
| 10 | getEquipmentLineOptions | X | X | X | X | X |

Die Operationen sind gleichartig aufgebaut. Sie nutzen eine identische Parametersignatur
und Rückgabesignatur. Neben Fahrzeugart, Hersteller, Haupttyp und Untertyp können
je bereits gewählte Ausstattungen im Parameter „availableOptions" übergeben werden.
