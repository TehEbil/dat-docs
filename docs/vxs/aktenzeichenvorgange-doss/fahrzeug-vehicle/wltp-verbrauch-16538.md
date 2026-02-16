---
title: "WLTP Verbrauchs- und Emissionswerte (TechInfoWltp)"
topic_id: "16538"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Technische Daten (TechInfo) > WLTP Verbrauchs- und Emissionswerte (TechInfoWltp)"
---

# WLTP Verbrauchs- und Emissionswerte (TechInfoWltp)

<TechInfoWltp> ist ein Unter-Element von <TechInfo> und enthält WLTP Min./Max. Werte zu Kraftstoffverbrauch, CO2-Emissionen, Stromverbrauch
und elektrischer Reichweite des Fahrzeugs.

Das WLTP-Testverfahren berücksichtigt nicht nur verschiedene Situationen und Geschwindigkeiten
im Straßenverkehr, sondern auch die verschiedenen Ausstattungsvarianten und Gewichtsklassen
eines Autos. Die Hersteller gruppieren fast immer die Verbräuche nach Motor-Getriebe-Variante,
individuelle Ausstattungen bzw. Ausstattungslinien werden hier, nicht eindeutig berücksichtigt
und daher werden meist die Angaben als von-bis Werte gemacht, Basisfahrzeug mit Serienausstattung
(als Min.) und höchste Ausstattungslinie + Sonderausstattung (als Max.). Die von DAT
angezeigten Verbrauchswerte entsprechen die von Hersteller angegebenen Verbrauchswerte
(laut Preisliste oder Verkaufshandbuch) und nicht ein individuell konfiguriertes Fahrzeug
(Werte wie in COC-Bescheinigung oder Fahrzeugschein).

Felder:

| Element | Typ | Beschreibung | Abrufbar durch Anwendung |
| --- | --- | --- | --- |
| (Dat)WltpConsumptionLowMin | Decimal | Minimaler Kraftstoffverbrauch (l/100 km) bei niedrigen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionLowMax | Decimal | Maximaler Kraftstoffverbrauch (l/100 km) bei niedrigen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionMediumMin | Decimal | Minimaler Kraftstoffverbrauch (l/100 km) bei mittleren Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionMediumMax | Decimal | Maximaler Kraftstoffverbrauch (l/100 km) bei mittleren Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionHighMin | Decimal | Minimaler Kraftstoffverbrauch (l/100 km) bei hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionHighMax | Decimal | Maximaler Kraftstoffverbrauch (l/100 km) bei hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionExtraHighMin | Decimal | Minimaler Kraftstoffverbrauch (l/100 km) bei sehr hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionExtraHighMax | Decimal | Maximaler Kraftstoffverbrauch (l/100 km) bei sehr hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionMixedMin | Decimal | Minimaler Kraftstoffverbrauch (l/100 km) bei gemischten Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionMixedMax | Decimal | Maximaler Kraftstoffverbrauch (l/100 km) bei gemischten Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentLowCngMin | Decimal | Minimaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) bei niedrigen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentLowCngMax | Decimal | Maximaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) bei niedrigen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMediumCngMin | Decimal | Minimaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) bei mittleren Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMediumCngMax | Decimal | Maximaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) bei mittleren Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentHighCngMin | Decimal | Minimaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) bei hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentHighCngMax | Decimal | Maximaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) bei hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentExtraHighCngMin | Decimal | Minimaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) bei sehr hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentExtraHighCngMax | Decimal | Maximaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) bei sehr hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMixedCngMin | Decimal | Minimaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) bei gemischten Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMixedCngMax | Decimal | Maximaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km) bei gemischten Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentLowLpgMin | Decimal | Minimaler Kraftstoffverbrauch LPG (l/100 km) bei niedrigen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentLowLpgMax | Decimal | Maximaler Kraftstoffverbrauch LPG (l/100 km) bei niedrigen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMediumLpgMin | Decimal | Minimaler Kraftstoffverbrauch LPG (l/100 km) bei mittleren Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMediumLpgMax | Decimal | Maximaler Kraftstoffverbrauch LPG (l/100 km) bei mittleren Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentHighLpgMin | Decimal | Minimaler Kraftstoffverbrauch LPG (l/100 km) bei hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentHighLpgMax | Decimal | Maximaler Kraftstoffverbrauch LPG (l/100 km) bei hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentExtraHighLpgMin | Decimal | Minimaler Kraftstoffverbrauch LPG (l/100 km) bei sehr hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentExtraHighLpgMax | Decimal | Maximaler Kraftstoffverbrauch LPG (l/100 km) bei sehr hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMixedLpgMin | Decimal | Minimaler Kraftstoffverbrauch LPG (l/100 km) bei gemischten Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMixedLpgMax | Decimal | Maximaler Kraftstoffverbrauch LPG (l/100 km) bei gemischten Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentLowHMin | Decimal | Minimaler Kraftstoffverbrauch H (kg/100 km) bei niedrigen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentLowHMax | Decimal | Maximaler Kraftstoffverbrauch H (kg/100 km) bei niedrigen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMediumHMin | Decimal | Minimaler Kraftstoffverbrauch H (kg/100 km) bei mittleren Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMediumHMax | Decimal | Maximaler Kraftstoffverbrauch H (kg/100 km) bei mittleren Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentHighHMin | Decimal | Minimaler Kraftstoffverbrauch H (kg/100 km) bei hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentHighHMax | Decimal | Maximaler Kraftstoffverbrauch H (kg/100 km) bei hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentExtraHighHMin | Decimal | Minimaler Kraftstoffverbrauch H (kg/100 km) bei sehr hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentExtraHighHMax | Decimal | Maximaler Kraftstoffverbrauch H (kg/100 km) bei sehr hohen Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMixedHMin | Decimal | Minimaler Kraftstoffverbrauch H (kg/100 km) bei gemischten Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionBivalentMixedHMax | Decimal | Maximaler Kraftstoffverbrauch H (kg/100 km) bei gemischten Geschwindigkeiten nach WLTP | Fahrzeugauswahl |
| (Dat)WltpCo2ClassMin | String | Minimale CO2 Emissionsklasse nach WLTP | Fahrzeugauswahl |
| (Dat)WltpCo2ClassMax | String | Maximale CO2 Emissionsklasse nach WLTP | Fahrzeugauswahl |
| (Dat)WltpCo2ClassWithDischargedBatteryMin | String | Minimale CO2 Emissionsklasse mit entladener Batterie nach WLTP | Fahrzeugauswahl |
| (Dat)WltpCo2ClassWithDischargedBatteryMax | String | Maximale CO2 Emissionsklasse mit entladener Batterie nach WLTP | Fahrzeugauswahl |
| (Dat)WltpCo2EmissionMin | Decimal | Minimaler CO2-Ausstoß (g/km) nach WLTP | Fahrzeugauswahl |
| (Dat)WltpCo2EmissionMax | Decimal | Maximaler CO2-Ausstoß (g/km) nach WLTP | Fahrzeugauswahl |
| (Dat)WltpCo2EmissionWithDischargedBatteryMin | Decimal | Minimaler CO2-Ausstoß (g/km) mit entladener Batterie nach WLTP | Fahrzeugauswahl |
| (Dat)WltpCo2EmissionWithDischargedBatteryMax | Decimal | Maximaler CO2-Ausstoß (g/km) mit entladener Batterie nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalMin | Decimal | Minimaler Stromverbrauch (kWh/100 km) nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalMax | Decimal | Maximaler Stromverbrauch (kWh/100 km) nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionWithDischargedBatteryMin | Decimal | Minimaler Kraftstoffverbrauch (l/100 km) mit entladener Batterie nach WLTP | Fahrzeugauswahl |
| (Dat)WltpConsumptionWithDischargedBatteryMax | Decimal | Maximaler Kraftstoffverbrauch (l/100 km) mit entladener Batterie nach WLTP | Fahrzeugauswahl |
| (Dat)WltpRangeElectricalMin | Integer | Elektromotor-Reichweite (km) bei min. nach WLTP | Fahrzeugauswahl |
| (Dat)WltpRangeElectricalMax | Integer | Elektromotor-Reichweite (km) bei max. nach WLTP | Fahrzeugauswahl |
| (Dat)WltpRangeTotalMin | Integer | Gesamtreichweite (km) bei min. nach WLTP | Fahrzeugauswahl |
| (Dat)WltpRangeTotalMax | Integer | Gesamtreichweite (km) bei max. nach WLTP | Fahrzeugauswahl |
| neue Felder: |  |  |  |
| (Dat)WltpCo2EmissionElectricalMin | Decimal | CO2-Ausstoß (g/km) bei elektrischem Betrieb nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpCo2EmissionElectricalMax | Decimal | CO2-Ausstoß (g/km) bei elektrischem Betrieb nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpCo2ClassElectricalMin | String | CO2-Klasse bei elektrischem Betrieb nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpCo2ClassElectricalMax | String | CO2-Klasse bei elektrischem Betrieb nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionWithDischargedBatteryLowMin | Decimal | Kraftstoffverbrauch (l/100km) bei entladener Batterie bei niedrigen Geschwindigkeiten nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionWithDischargedBatteryLowMax | Decimal | Kraftstoffverbrauch (l/100km) bei entladener Batterie bei niedrigen Geschwindigkeiten nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionWithDischargedBatteryMediumMin | Decimal | Kraftstoffverbrauch (l/100km) bei entladener Batterie bei mittleren Geschwindigkeiten nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionWithDischargedBatteryMediumMax | Decimal | Kraftstoffverbrauch (l/100km) bei entladener Batterie bei mittleren Geschwindigkeiten nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionWithDischargedBatteryHighMin | Decimal | Kraftstoffverbrauch (l/100km) bei entladener Batterie bei hohen Geschwindigkeiten nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionWithDischargedBatteryHighMax | Decimal | Kraftstoffverbrauch (l/100km) bei entladener Batterie bei hohen Geschwindigkeiten nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionWithDischargedBatteryExtraHighMin | Decimal | Kraftstoffverbrauch (l/100km) bei entladener Batterie bei sehr hohen Geschwindigkeiten nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionWithDischargedBatteryExtraHighMax | Decimal | Kraftstoffverbrauch (l/100km) bei entladener Batterie bei sehr hohen Geschwindigkeiten nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionEnergyLtrMin | Decimal | Energieverbrauch (l/100km) nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionEnergyLtrMax | Decimal | Energieverbrauch (l/100km) nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionEnergyElectricalMin | Decimal | Energieverbrauch bei elektrischem Betrieb (kWh/100 km) kombiniert nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionEnergyElectricalMax | Decimal | Energieverbrauch bei elektrischem Betrieb (kWh/100 km) kombiniert nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalLowMin | Decimal | Stromverbrauch (kWh/100 km) bei niedrigen Geschwindigkeiten nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalLowMax | Decimal | Stromverbrauch (kWh/100 km) bei niedrigen Geschwindigkeiten nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalMediumMin | Decimal | Stromverbrauch (kWh/100 km) bei mittleren Geschwindigkeiten nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalMediumMax | Decimal | Stromverbrauch (kWh/100 km) bei mittleren Geschwindigkeiten nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalHighMin | Decimal | Stromverbrauch (kWh/100 km) bei hohen Geschwindigkeiten nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalHighMax | Decimal | Stromverbrauch (kWh/100 km) bei hohen Geschwindigkeiten nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalExtraHighMin | Decimal | Stromverbrauch (kWh/100 km) bei sehr hohen Geschwindigkeiten nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalExtraHighMax | Decimal | Stromverbrauch (kWh/100 km) bei sehr hohen Geschwindigkeiten nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalCityMin | Decimal | Stromverbrauch (kWh/100 km) im City-Betrieb nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionElectricalCityMax | Decimal | Stromverbrauch (kWh/100 km) im City-Betrieb nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpRangeElectricalCityMin | Integer | Reichweite (km) bei elektrischem City-Betrieb nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpRangeElectricalCityMax | Integer | Reichweite (km) bei elektrischem City-Betrieb nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionCngUnit | String | CNG Verbrauchseinheit für WLTP-Werte (Benutzer-Feld aktuell nicht unterstützt) | Fahrzeugauswahl |
| (Dat)WltpCo2EmissionBivalentMin | Decimal | CO2-Ausstoß (g/km) bei CNG-, LPG- oder Wasserstoffbetrieb nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpCo2EmissionBivalentMax | Decimal | CO2-Ausstoß (g/km) bei CNG-, LPG- oder Wasserstoffbetrieb nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpCo2ClassBivalentMin | String | CO2-Klasse bei CNG-, LPG- oder Wasserstoffbetrieb nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpCo2ClassBivalentMax | String | CO2-Klasse bei CNG-, LPG- oder Wasserstoffbetrieb nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionEnergyBivalentMin | Decimal | Energieverbrauch (kg/100 km) bei CNG-, LPG- oder Wasserstoffbetrieb (cbm/100 km im Falle von CNG und WltpConsumptionCngUnit == 'CBM') nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionEnergyBivalentMax | Decimal | Energieverbrauch (kg/100 km) bei CNG-, LPG- oder Wasserstoffbetrieb (cbm/100 km im Falle von CNG und WltpConsumptionCngUnit == 'CBM') nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionEnergyWeightedLtrMin | Decimal | Energieverbrauch gewichtet (l/100km) nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionEnergyWeightedLtrMax | Decimal | Energieverbrauch gewichtet (l/100km) nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpConsumptionEnergyWeightedKwhMin | Decimal | Energieverbrauch gewichtet (kWh/100 km) nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpConsumptionEnergyWeightedKwhMax | Decimal | Energieverbrauch gewichtet (kWh/100 km) nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpCo2EmissionWeightedMin | Decimal | CO2-Ausstoß (g/km) gewichtet kombiniert nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpCo2EmissionWeightedMax | Decimal | CO2-Ausstoß (g/km) gewichtet kombiniert nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpCo2ClassWeightedMin | String | CO2-Klasse gewichtet kombiniert nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpCo2ClassWeightedMax | String | CO2-Klasse gewichtet kombiniert nach WLTP max. | Fahrzeugauswahl |
| (Dat)WltpUtilFactorPercentMin | Decimal | Nutzungsfaktor (%) nach WLTP min. | Fahrzeugauswahl |
| (Dat)WltpUtilFactorPercentMax | Decimal | Nutzungsfaktor (%) nach WLTP max. | Fahrzeugauswahl |
| (Dat)YearOfValidityAverageFuelElectricityPrice | Integer | Kraftstoff/Strompreisdurchschnitt Gültigkeitsjahr (DAT-Feld aktuell nicht unterstützt) | Fahrzeugauswahl |
| (Dat)PriceOfFuelAverageInYear | Decimal | Kraftstoffpreis Jahresdurchschnitt (EUR/l) (DAT-Feld aktuell nicht unterstützt) | Fahrzeugauswahl |
| (Dat)PriceOfElectricityAverageInYear | Decimal | Strompreis Jahresdurchschnitt (EUR/kWh) (DAT-Feld aktuell nicht unterstützt) | Fahrzeugauswahl |
| (Dat)PriceCo2PerTonLow | Decimal | Niedriger CO2-Preis (EUR/t) (DAT-Feld aktuell nicht unterstützt) | Fahrzeugauswahl |
| (Dat)PriceCo2PerTonMedium | Decimal | Mittlerer CO2-Preis (EUR/t) (DAT-Feld aktuell nicht unterstützt) | Fahrzeugauswahl |
| (Dat)PriceCo2PerTonHigh | Decimal | Hoher CO2-Preis (EUR/t) (DAT-Feld aktuell nicht unterstützt) | Fahrzeugauswahl |
| (Dat)RangeOfCo2PriceYearStart | Integer | CO2-Preiszeitraum von (Jahr) (DAT-Feld aktuell nicht unterstützt) | Fahrzeugauswahl |
| (Dat)RangeOfCo2PriceYearEnd | Integer | CO2-Preiszeitraum bis (Jahr) (DAT-Feld aktuell nicht unterstützt) | Fahrzeugauswahl |
