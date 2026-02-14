---
title: "Achsen (Axle)"
topic_id: "2892"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Reifen (Tires) > Achsen (Axle)"
---

# Achsen (Axle)

| Element | Typ | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| AxleNo | Integer | Nummer der Achse | numerisch |
| TireId | Integer | DAT-Reifennummer; | numerisch |
| TireState | String | Reifenstatus | mounted = montiert  unmounted = nicht montiert  spare wheel = Ersatzrad |
| NrOfTires | Integer | Reifenanzahl;  Werte:  Transporter und LKW: erste Achse: 2, weitere Achsen: 2 oder 4;  Kraftrad: erste Achse: 1 oder 2, weitere Achsen: 1;  unmontierte Reifen oder  Reserverad: 1; | 1,  2,  4 |
| TireType | String | Reifenart |  |
| TireOriginalPrice | Decimal | Neupreis |  |
| TireSpeedIndex | String | Geschwindigkeitsindex |  |
| TireSize | String | Reifengröße |  |
| TireSafetySystem | String | Reifen-Sicherheitssystem |  |
| TireManufacturer | Integer | Code für Reifenhersteller |  |
| TireManufacturerName | String | Name des Reifenherstellers |  |
| TireBrandEanCode | String | EAN (European Article Number) der Reifenmarke |  |
| PrintLoadCapacityIdx | Boolean |  | TRUE  FALSE |
| TireOriginalTreadDepth | Integer | Original Profiltiefe in mm | numerisch |
| TireLoadCapacityIndex | Integer | Tragfähigkeitsindex in kg |  |
| TireLoadCapacityIndex2 | Integer | Tragfähigkeitsindex 2 in kg |  |
| TreadDepthLeftOuterPerc | Decimal | Profiltiefe links außen in Prozent | numerisch |
| TreadDepthLeftInnerPerc | Decimal | Profiltiefe links innen in Prozent | numerisch |
| TreadDepthRightInnerPerc | Decimal | Profiltiefe rechts innen in Prozent | numerisch |
| TreadDepthRightOuterPerc | Decimal | Profiltiefe rechts außen in Prozent | numerisch |
| TreadDepthLeftOuterMm | Decimal | Profiltiefe links außen in mm | numerisch |
| TreadDepthLeftInnerMm | Decimal | Profiltiefe links innen in mm | numerisch |
| TreadDepthRightInnerMm | Decimal | Profiltiefe rechts innen in mm | numerisch |
| TreadDepthRightOuterMm | Decimal | Profiltiefe rechts außen in mm | numerisch |
| ManualEntry | Boolean | Kennzeichen, ob Achse manuell angelegt wurde | TRUE = manueller Eintrag FALSE = kein manueller Eintrag |
| RetreadedLeftOuter | Boolean | Kennzeichen; Reifen links außen runderneuert | TRUE = runderneuert FALSE = nicht runderneuert |
| RetreadedLeftInner | Boolean | Kennzeichen; Reifen links innen runderneuert | TRUE = runderneuert FALSE = nicht runderneuert |
| RetreadedRightInner | Boolean | Kennzeichen; Reifen rechts innen runderneuert | TRUE = runderneuert FALSE = nicht runderneuert |
| RetreadedRightOuter | Boolean | Kennzeichen; Reifen rechts außen runderneuert | TRUE = runderneuert FALSE = nicht runderneuert |
