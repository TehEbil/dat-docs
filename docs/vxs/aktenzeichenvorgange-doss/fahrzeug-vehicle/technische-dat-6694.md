---
title: "Technische Daten (TechInfo)"
topic_id: "6694"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Technische Daten (TechInfo)"
---

# Technische Daten (TechInfo)

<TechInfo> ist ein Unter-Element von <Vehicle> und <UpperBody> und enthält Informationen zu den technischen Daten des Fahrzeugs.

Felder:

| Element | Typ | Beschreibung | Abrufbar durch Anwendung |
| --- | --- | --- | --- |
| (Dat)Acceleration | Decimal | Beschleunigung von 0 auf 100 km/h (s) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)BatteryCapacity | Decimal | Batteriekapazität (kWh) | Fahrzeugauswahl |
| (Dat)BatteryConstructionType | String | Batteriebauart | Fahrzeugauswahl |
| (Dat)BatteryVoltage | Decimal | Batteriespannung (V) | Fahrzeugauswahl |
| (Dat)BatteryWeight | Decimal | Batteriegewicht (kg) | Fahrzeugauswahl |
| (Dat)Capacity | Integer | Hubraum (ccm) | Fahrzeugauswahl |
| (Dat)ChargingCurrentPlugType | String | Ladestromsteckertyp | Fahrzeugauswahl |
| (Dat)Co2Emission | Decimal | CO2-Ausstoß (g/km) | Fahrzeugauswahl |
| (Dat)Consumption | Decimal | Kraftstoffverbrauch (l/100km) kombiniert (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionElectricalCurrent | Decimal | Stromverbrauch (kWh/100 km) | Fahrzeugauswahl |
| (Dat)ConsumptionInnerCng | Decimal | Kraftstoffverbrauch CNG innerorts (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionInnerH | Decimal | Kraftstoffverbrauch H innerorts (kg/100 km) (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionInnerLpg | Decimal | Kraftstoffverbrauch LPG innerorts (kg/100 km) (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionInTown | Decimal | Kraftstoffverbrauch innerorts (l/100km) (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionMixCng | Decimal | Kraftstoffverbrauch CNG kombiniert (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionMixH | Decimal | Kraftstoffverbrauch H kombiniert (kg/100 km) (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionMixLpg | Decimal | Kraftstoffverbrauch LPG kombiniert (kg/100 km) (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionOuterCng | Decimal | Kraftstoffverbrauch CNG außerorts (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionOuterH | Decimal | Kraftstoffverbrauch H außerorts (kg/100 km) (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionOuterLpg | Decimal | Kraftstoffverbrauch LPG außerorts (kg/100 km) (NEFZ) | Fahrzeugauswahl |
| (Dat)ConsumptionOutOfTown | Decimal | Kraftstoffverbrauch außerorts (l/100km) (NEFZ) | Fahrzeugauswahl |
| (Dat)CountOfAirbags | Integer | Anzahl Airbags | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)CountOfAxles | Integer | Anzahl Achsen | Fahrzeugauswahl |
| (Dat)CountOfDrivedAxles | Integer | Anzahl angetriebener Achsen | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)Cylinder | Integer | Anzahl Zylinder | Fahrzeugauswahl |
| (Dat)CylinderArrangement | String | Zylinderanordnung | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)DriveN | String | Antriebsart Benennung | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| DriveCode | String | Antriebsart Schlüssel | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)EmissionClass | String | Schadstoffklasse (veraltet, bitte nicht mehr verwenden!) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)EmissionClassN | Element | Schadstoffklasse (Struktur aus den Werten für Typ, Beschreibung und OBD Ja/Nein) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)EnergyEfficiencyClass | String | EnVKV Energieeffizienzklasse (NEFZ) | Fahrzeugauswahl |
| (Dat)EngineCycle | Integer | Motorsteuerung (Takt) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)FuelMethod | String | Kraftstoffart Benennung | Fahrzeugauswahl |
| FuelMethodCode | String | Kraftstoffart Schlüssel | Fahrzeugauswahl |
| (Dat)FuelMethodType | String | Kraftstofftyp Schlüssel | Fahrzeugauswahl |
| (Dat)Height | Integer | Fahrzeug-Höhe (mm) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)Length | Integer | Fahrzeug-Länge (mm) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)LoadingHeight | Long | Laderaum-Höhe (mm) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)LoadingLength | Long | Laderaum-Länge (mm) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)LoadingSpace | Long | Laderaum-Volumen (dm³) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)LoadingSpaceMax | Long | Laderaum-Volumen max. (dm³) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)LoadingWidth | Long | Laderaum-Breite (mm) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)NormalChargeDuration | Decimal | Ladedauer bei Standardladung (STD) (WallBox/Ladestation) | Fahrzeugauswahl |
| (Dat)NormalChargeVoltage | Long | Standardladung (V) | Fahrzeugauswahl |
| (Dat)Payload | Long | Nutzlast (kg) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)PermissableTotalWeight | Decimal | Zulässiges Gesamtgewicht (kg) | Fahrzeugauswahl |
| (Dat)PluginSystem | Boolean | Plug-in-System (J/N) | Fahrzeugauswahl |
| (Dat)PowerHp | Integer | Leistung (PS) | Fahrzeugauswahl |
| (Dat)PowerHpMax | Decimal | Motorleistung (PS) (max) | Fahrzeugauswahl |
| (Dat)PowerHpMaxSecondary | Decimal | Motorleistung (PS) (max) Sekundär-Antrieb | Fahrzeugauswahl |
| (Dat)PowerHpPermanent | Decimal | Motorleistung (PS) (Permanent/Dauer) | Fahrzeugauswahl |
| (Dat)PowerHpPermanentSecondary | Decimal | Motorleistung (PS) (Permanent/Dauer) Sekundär-Antrieb | Fahrzeugauswahl |
| (Dat)PowerHpSystem | Decimal | Systemleistung (PS) | Fahrzeugauswahl |
| (Dat)PowerKw | Decimal | Leistung (kW) | Fahrzeugauswahl |
| (Dat)PowerKwMax | Decimal | Motorleistung (kW) (max) | Fahrzeugauswahl |
| (Dat)PowerKwMaxSecondary | Decimal | Motorleistung (kW) (max) Sekundär-Antrieb | Fahrzeugauswahl |
| (Dat)PowerKwPermanent | Decimal | Motorleistung (kW) (Permanent/Dauer) | Fahrzeugauswahl |
| (Dat)PowerKwPermanentSecondary | Decimal | Motorleistung (kW) (Permanent/Dauer) Sekundär-Antrieb | Fahrzeugauswahl |
| (Dat)PowerKwSystem | Decimal | Systemleistung (kW) | Fahrzeugauswahl |
| (Dat)QuickChargeDuration | Decimal | Ladedauer bei Schnellladung (STD) (WallBox/Ladestation) | Fahrzeugauswahl |
| (Dat)QuickChargeVoltage | Long | Schnellladung (V) | Fahrzeugauswahl |
| (Dat)QuickdropSystem | Boolean | Quickdrop-System (J/N) | Fahrzeugauswahl |
| (Dat)RangeOfElectricMotor | Long | Elektromotor-Reichweite (km) | Fahrzeugauswahl |
| (Dat)RangeTotal | Long | Gesamtreichweite (km) | Fahrzeugauswahl |
| (Dat)RoofLoad | Integer | Dachlast (kg) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)RotationsOnMaxPower | Integer | Anzahl Umdrehungen pro Minute bei maximaler Leistung | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)RotationsOnMaxTorque | Integer | Anzahl Umdrehungen pro Minute bei maximalem Drehmoment | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)SpeedMax | Integer | Höchstgeschwindigkeit (km/h) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)SuitableForE10 | Boolean | E10 geeignet | Fahrzeugauswahl |
| (Dat)TankVolume | Integer | Tankinhalt (l) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)TankVolumeAlternative | Long | Tankinhalt alternativ (l) | Fahrzeugauswahl |
| (Dat)Torque | Integer | Drehmoment (Nm) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)TrailerLoadBraked | Integer | Anhängelast gebremst (kg) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)TrailerLoadUnbraked | Integer | Anhängelast ungebremst (kg) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)UnloadedWeight | Decimal | Leergewicht (kg) | Fahrzeugauswahl |
| (Dat)VehicleDoors | Integer | Anzahl Türen | Fahrzeugauswahl |
| (Dat)VehicleSeats | Integer | Anzahl Sitze | Fahrzeugauswahl |
| (Dat)WeightTotalCombination | Long | Zul. Gesamtgewicht Fahrzeugkombination (kg) | Fahrzeugauswahl |
| (Dat)WheelBase | Integer | Radstand (mm) | Fahrzeugauswahl |
| (Dat)Width | Integer | Fahrzeug-Breite (mm) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)WidthForGarage | Long | Fahrzeugbreite-Garagenmaß (mm) | Fahrzeugauswahl |
| AxleLoadFront | Integer | Achslast vorn (kg) |  |
| AxleLoadBack | Integer | Achslast hinten (kg) |  |
| AxleLoadMiddle | Integer | Achslast mitte (kg) |  |
| CabineStructureDescription | String | Aufbau Fahrerhaus (Beschreibung) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| CabineStructureType | String | Aufbau Fahrerhaus (Schlüssel) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| DustBadge | String | Feinstaubplakette | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| FillingQuantities | Element | Füllstandsmengen; nur für Fahrzeugarten 1 und 2 | calculatePro |
| GearboxType | String | Getriebeart; manual; automatic; other | Fahrzeugauswahl |
| InsuranceTypeClassCascoComplete | String | Typklasse Vollkasko | Fahrzeugauswahl |
| InsuranceTypeClassCascoPartial | String | Typklasse Teilkasko | Fahrzeugauswahl |
| InsuranceTypeClassLiability | String | Typklasse Haftpflicht | Fahrzeugauswahl |
| NrOfGears | String | Anzahl der Gänge bzw. "V" für stufenloses Getriebe (CVT) | Fahrzeugauswahl |
| OriginalTireSizeAxle1 | String | Serienbereifung Vorderachse |  |
| OriginalTireSizeAxle2 | String | Serienbereifung Hinterachse |  |
| ProductGroupCode | Integer | Produktgruppe (Schlüssel), identisch mit GrpFor aus der Datenlieferung [Zusatzelement 3](../../../lieferungen/satzbeschreibung-dat-urop/beschreibung-zusatze/felderliste-te-2837.md) |  |
| ProductGroupName | String | Produktgruppe (Name) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| (Dat)StructureDescription | String | Fahrzeugaufbau Kurzbezeichnung | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| StructureType | String | Fahrzeugaufbau (Limousine, Kombi, …) | Fahrzeugauswahl, nur mit Berechtigung „erweiterte Fahrzeugdaten" |
| TonnageClass | String | Tonnage-Klasse | Fahrzeugauswahl |
| UpperBodyMaterial | String | Material Aufbau |  |
| UpperBodyStructureAndVersion | String | Lkw-Aufbau Version |  |
| UpperBodyStructureDescription | String | Lkw-Aufbau Beschreibung |  |
| UpperBodyStructureDescriptionUser | String | Lkw-Aufbau Beschreibung (Benutzer) |  |
| UpperBodyStructureType | String | Lkw-Aufbau Typ |  |
| WheelBase2 | Integer | Radstand alternative, Hinterachse (mm) | Fahrzeugauswahl |
| (Dat)Co2EmissionBivalent | Decimal | CO2-Ausstoß (g/km) bei CNG-, LPG- oder Wasserstoffbetrieb nach NEFZ | Fahrzeugauswahl |
| (Dat)EnergyEfficiencyClassMax | String | Energieffizienzklasse nach NEFZ max. | Fahrzeugauswahl |
| (Dat)EnergyEfficiencyClassBivalentMin | String | Energieffizienzklasse bei CNG-, LPG- oder Wasserstoffbetrieb nach NEFZ min. | Fahrzeugauswahl |
| (Dat)EnergyEfficiencyClassBivalentMax | String | Energieffizienzklasse bei CNG-, LPG- oder Wasserstoffbetrieb nach NEFZ max. | Fahrzeugauswahl |
| (Dat)ConsumptionCngUnit | String | CNG Verbrauchseinheit (Benutzer-Feld aktuell nicht unterstützt) | Fahrzeugauswahl |
| (Dat)CostsEnergyAt15TkmPerYear | Decimal | Energiekosten bei 15000 km Jahreslaufleistung | Fahrzeugauswahl |
| (Dat)TaxPerYear | Decimal | Kraftfahrzeugsteuer pro Jahr | Fahrzeugauswahl |
| (Dat)Co2CostsNextTenYearsLow | Decimal | Mögliche CO2-Kosten die nächsten 10 Jahre (15 Tkm/Jahr) bei niedrigen CO2-Preis | Fahrzeugauswahl |
| (Dat)Co2CostsNextTenYearsMedium | Decimal | Mögliche CO2-Kosten die nächsten 10 Jahre (15 Tkm/Jahr) bei mittleren CO2-Preis | Fahrzeugauswahl |
| (Dat)Co2CostsNextTenYearsHigh | Decimal | Mögliche CO2-Kosten die nächsten 10 Jahre (15 Tkm/Jahr) bei hohen CO2-Preis | Fahrzeugauswahl |
| (Dat)YearOfValidityAverageFuelElectricityPrice | Integer | Kraftstoff/Strompreisdurchschnitt Gültigkeitsjahr | Fahrzeugauswahl |
| (Dat)PriceOfFuelAverageInYear | Decimal | Kraftstoffpreis Jahresdurchschnitt (EUR/l) | Fahrzeugauswahl |
| (Dat)PriceOfElectricityAverageInYear | Decimal | Strompreis Jahresdurchschnitt (EUR/kWh) | Fahrzeugauswahl |
| (Dat)PriceCo2PerTonLow | Decimal | Niedriger CO2-Preis (EUR/t) | Fahrzeugauswahl |
| (Dat)PriceCo2PerTonMedium | Decimal | Mittlerer CO2-Preis (EUR/t) | Fahrzeugauswahl |
| (Dat)PriceCo2PerTonHigh | Decimal | Hoher CO2-Preis (EUR/t) | Fahrzeugauswahl |
| (Dat)RangeOfCo2PriceYearStart | Integer | CO2-Preiszeitraum von (Jahr) | Fahrzeugauswahl |
| (Dat)RangeOfCo2PriceYearEnd | Integer | CO2-Preiszeitraum bis (Jahr) | Fahrzeugauswahl |
| FuelMethodDetail | String | Kraftstoffart Detail, zur Energiekostenberechnung für die EnVKV (Deutschland) | Fahrzeugauswahl |
| FuelMethodDetailName | String | Kraftstoffart Detail Name für EnVKV | Fahrzeugauswahl |
| (Dat)PriceOfFuelPerKgAverageInYear | Decimal | Kraftstoffpreis Jahresdurchschnitt (EUR/kg) | Fahrzeugauswahl |
