---
title: "RepairParameters"
topic_id: "1415"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > RepairParameters"
---

# RepairParameters

Wichtige Information:

Bitte beachten Sie, dass unsere Schnittstelle weiterhin die RepairParameters unterstützen wird. Diese Parameter ermöglichen die Berücksichtigung zusätzlicher Faktoren
außerhalb der Maske Vorgangsbezogene Daten, die nicht über die ProcedureRelatedParameters übermittelt werden können – beispielsweise bei der Phantomkalkulation. Für Kalkulationsfaktoren,
die innerhalb der Maske Vorgangsbezogene Daten liegen, sind jedoch zwingend die ProcedureRelatedParameters zu verwenden.

| Element | Datatype | Beschreibung |
| --- | --- | --- |
| SeriesSpecific | Boolean | Abfrage Serienkalkulation; mögliche Werte: True/False |
| PhantomCalculation | Boolean | Abfrage Phantomkalkulation; mögliche Werte: True/False |
| PartsCorrection | Decimal | Teilekorrektur (Auf-/Abschlag in Prozent) |
| PartsDiscountPercentage | Decimal | Ersatzteilrabatt prozentual |
| PartsDiscountAmount | Decimal | Erstatzteilrabatt absoult |
| PartsDiscountPercentageForOpt | Decimal | Ersatzteilrabatt Optimierung auf RBK prozentual |
| PartsDiscountAmountForOpt | Decimal | Ersatzteilrabatt Optimierung auf RBK absolut |
| ConsumablesType | Werteliste | ConsumablesType kann die Werte 0, 1 oder 2 annehmen und legt fest, wie das Klein- und Verbrauchsmaterial mit ConsumablesPercentage zu ermitteln ist.  0 = Pauschale Angabe  1 = Prozentual aus der Summe der Ersatzteilpreise  2 = Prozentual aus der Summe der Lohnkosten |
| ConsumablesFlatAmount | Decimal | Pauschalbetrag in einer Währung |
| ConsumablesPercentage | Decimal | ist eine Angabe in Prozent für die Ermittlung von Klein- und Verbrauchsmaterial.  Optionaler Prozentwert, Wertebereich [0,00 bis 9,99]. |
| ConsumablesPercentageForOpt | Decimal | Optionaler Prozentwert bei Optimierung nach Rohbaukarosse, Wertebereich [0,00 bis 9,99].  (<CalcResultToUse>optimized</CalcResultToUse>) |
| ProcurementCosts | Decimal | Beschaffungskosten > Ersatzteile (EUR) |
| ProcurementCostsMaterial | Decimal | Beschaffungskosten für Material |
| ProcurementCostsBodyInWhite | Decimal | Beschaffungskosten > Rohbaukarosserie (EUR) |
| ProcurementCostsAlignmentBrackets | Decimal | Beschaffungskosten > Richtwinkelsatz (EUR) |
| ProcurementCostsPercentage | Decimal | Optionaler Prozentwert für die Ermittlung der Beschaffungskosten aus der Summe der Ersatzteilpreise. Wertebereich [0,00 – 99,99]. |
| ProcurementCostsPercentageBodyInWhite | Decimal | Dieser Parameter wirkt nur bei einer Optimierung auf Rohbaukarosse  // nur bei <CalcResultToUse>optimized</CalcResultToUse> |
| ProcurementCostsMax | Decimal | Ist die Angabe eines Maximalwertes für die aus dem Prozentwert ermittelten Beschaffungkosten. Es ist ein Betrag in einer Währung.  Maximaler Wert für die Beschaffungskosten. Wertebereich [0,00 bis 99999,99]. |
| ProcurementCostsMaxBodyInWhite | Decimal | Dieser Parameter wirkt nur bei einer Optimierung auf Rohbaukarosse  // nur bei <CalcResultToUse>optimized</CalcResultToUse> |
| PriceDate | Date | Ersatzteilfraktoren > Preisdatum |
| LacquerFremdleistungGlobal | String |  |
| LacquerMethod | String | Lackiermethode [EURO\_LACQUER | MANUFACTURER\_SPECIFIC | AZT] |
| LacquerTypeId | String |  |
| LacquerType | String | Lackart |
| LacquerTypeLayers | Integer | Anzahl Lackierschichten |
| LacquerDismountedPrelacquer | Boolean | Ausgebaut vorlackieren |
| LacquerPlasticMounted | Boolean | Kunststoffteile eingebaut lackieren |
| LacquerWithoutDisassembly | Boolean |  |
| LacquerWithForcedDisassembly | Boolean | Montageteile ausgebaut lackieren |
| LacquerReducedLeadTime | Boolean | Vorbereitung Einzelauftrag/Kleinteile |
| LacquerWithRack | Boolean | Einsatz Gerüst |
| LacquerAdditionTwoColor | Boolean | Zuschlag für 2. Farbe |
| LacquerAdditionMattpaint | Boolean |  |
| LacquerAdjustmentMixingUnit | Boolean | Lackzusatz: Farbtonangleich - Mischanlage |
| LacquerAdjustmentMixingColours | Integer |  |
| LacquerAdjustmentExemplarySheets | Integer | Anzahl Musterbleche |
| LacquerCompleteFlatrate | Decimal |  |
| LacquerWorkFlatrate | Decimal | Lacklohn / Lackmaterial > Pauschaler Lohn (EUR) |
| LacquerMaterialFlatrate | Decimal |  |
| SpecialLacquerAward | Decimal | Zuschlag Spezial-Lack (EUR) |
| LacquerMaterialPercentage | Decimal |  |
| LacquerMaterialIndex | Integer | Lackmaterial Materialindex (%) |
| LacquerMaterialChargePerPoint | Decimal |  |
| LacquerMaterialPriceCategory | Integer | Materialpreisgruppen nur für die Dateländer Polen und Tschechien |
| LacquerMaterialPrintDescr | Boolean |  |
| LacquerLeadTimeMetal | Decimal | Vorbereitungszeit Blech (%) |
| LacquerLeadTimePlastic | Decimal | Vorbereitungszeit Kunststoff (%) |
| LacquerLeadTimePercentage | Decimal |  |
| LacquerDisposalCosts | Decimal | Entsorgungskosten (%) |
| LacquerCoveringPanes | Integer | Abdeckarbeit geklebte Scheiben |
| LacquerCoveringDismountedPlastic | Integer | Abdeckarbeit ausgebaute Kunststoffteile |
| LacquerMattBlackWindowFrames | Integer | Anzahl mattschwarze Fensterrahmen |
| LacquerWageDiscountAmount | Decimal | Lacklohn / Lackmaterial > Lackmaterial > Rabatt in EUR |
| LacquerWageDiscountPercentage | Decimal | Lacklohn / Lackmaterial > Lackmaterial > Rabatt in Prozent |
| LacquerWageDiscountAmountForOpt | Decimal | Lacklohn / Lackmaterial > Lackmaterial > Rabatt Optimierung auf RBK in EUR |
| LacquerWageDiscountPercentageForOpt | Decimal | Lacklohn / Lackmaterial > Lackmaterial > Rabatt Optimierung auf RBK in Prozent |
| LacquerMaterialDiscountAmount | Decimal |  |
| LacquerMaterialDiscountPercentage | Decimal |  |
| LacquerMaterialDiscountAmountForOpt | Decimal |  |
| LacquerMaterialDiscountPercentageForOpt | Decimal |  |
| LacquerCompleteDiscountAmount | Decimal |  |
| LacquerCompleteDiscountPercentage | Decimal |  |
| LacquerCompleteDiscountAmountForOpt | Decimal |  |
| LacquerCompleteDiscountPercentageForOpt | Decimal |  |
| LacquerPaintWorkDiscountPercentage | Decimal |  |
| LacquerTimeUnitSystem | String | Das Zeitmaß für die Arbeitswerte bei den Lackiermethoden AZT und Eurolack.  Rückgabewerte:  "STD" = Stunden  "AE" = Arbeitseinheit (nur Niederlande)  "ZE" = Zeiteinheit  "AW" = Arbeitswert |
| LacquerTimeUnitsPerHour | Integer |  |
| TimeUnitSystem | String |  |
| TimeUnitsPerHour | String |  |
| TimeUnitsOfManufacturer | Boolean |  |
| RepairWageDiscountPercentage | Decimal | Arbeitslohnfaktoren Rabatt in Prozent |
| RepairWageDiscountAmount | Decimal | Arbeitslohnfaktoren Rabatt in Euro |
| RepairWageDiscountPercentageForOpt | Decimal | Arbeitslohnfaktoren Rabatt Optimierung auf RBK in Prozent |
| RepairWageDiscountAmountForOpt | Decimal | Arbeitslohnfaktoren Rabatt Optimierung auf RBK in Euro |
| LongWorkDescriptions | Boolean | Anzeige langer Arbeitstexte |
| AllIncludedWork | Boolean | Sämtliche umfasste Arbeiten ausgeben |
| FeeAE | Decimal |  |
| WithDomusCalculation | Boolean |  |
| PriceLevel | Integer |  |
| LacquerDiscountFactor | Decimal |  |
| WearBodyAge | Decimal |  |
| WearBodyCorrosion | Decimal |  |
| WearTyreMinSize | Decimal |  |
| WearTyreActualSize | Decimal |  |
| WearTyreSize | Decimal |  |
| WearTyreAge | String |  |
| WearBatAge | Decimal |  |
| WearBatTime | Decimal |  |
| WearPlasticAge | Decimal |  |
| WearCompAge | Decimal |  |
| WearCompMileage | Decimal |  |
| WearCompTypeId | Integer |  |
| WearCompTypeDesc | String |  |
| CalculationType |  |  |
| ConsumablesOfWagePerc | Decimal |  |
| ConsumablesPercentageSmallPartsForOpt | Decimal |  |
| IndicatorDataUsedAsPattern | Boolean |  |
| IndicatorIsGlassCalculation | Boolean | Mit getrennter Glaskalkulation |
| IndicatorGlassCalculationWithoutWork | Boolean | Glaskalkulation ohne Arbeit |
| IndicatorOptBodyShell | Boolean |  |
| IndicatorTimeUnitsInHours | Boolean |  |
| IndicatorWarrantyCalculation | Boolean |  |
| IndicatorWithoutBodyCavityAndUnderseal | Boolean |  |
| LevelOneE | Decimal |  |
| LevelOneJ | Decimal |  |
| LevelOneM | Decimal |  |
| LevelThree | Decimal |  |
| LevelTwo | Decimal |  |
| MaterialConstantPartsIntegrated | Decimal |  |
| MaterialConstantPartsRemoved | Decimal |  |
| MaterialConstantByAmount | Decimal |  |
| MaterialCostsPerUnit1CoatPainting | Decimal |  |
| ProcurementCostsPercBodyShellForOpt | Decimal |  |
| RentingCostsAlignmentBrackets | Decimal | Miete Richtwinkelsatz (EUR) |
| SparePartsDisposalCostsPerc | Decimal |  |
| CalculationWithoutConstants | Boolean |  |
| LacquerScratchResistant | Boolean |  |
| PearlEffectSurcharge | Decimal |  |
| ColorCount | Integer |  |
| DMSCalculation | Boolean |  |
| DMSPaintWPN | String |  |
| ExternalProvider | String |  |
| ExternalProviderStatus | Integer |  |
| TotalPredamageAmount | Decimal | Gibt die Vorschadenpauschale in Euro an. |
| TotalNFOAmount | Decimal | Gibt den Neu Für Alt (NFA) Abzug pauschaler Wert in Euro an. |
| TotalNFOPercent | Decimal | Eingabe Neu Für Alt (NFA) Abzug in Prozent. |
| TotalValueImprovementAmount | Decimal | Gibt die Wertverbesserungpauschale in Euro an. |
| AdditionalCostsFlatAmount | Decimal | Gibt die Nebenkostenpauschale in Euro an.  Optionaler Betrag in Euro, Bereich [0-100,00] |
| AdditionalCostsPercent | Decimal | Gibt an, zu wie viel Prozent die Nebenkostenpauschale berücksichtigt wird.  Optionaler Prozentwert für Nebenkostenpauschale, Bereich [0-100,0].  Lesart: 34,50 Euro zu 80 Prozent. |
| DisposalCostsSparePartsPercentage | Decimal | Gibt die Entsorgungskosten in Prozent von der Summe der Ersatzteilpreise an.  Optionaler Prozentwert, Wertebereich [0-99,99]. |
| LacquerAdjustments |  |  |
| PartsSurchargeInProtocol | Boolean | ET-Zuschlag nur im Protokoll anzeigen |
| PartsSurchargeSeparated | Boolean | Ersatzteilzuschlag separat |
| AztFourLayerLacquerMode | String | 4-Schicht Lackierung  [DRY\_AND\_SAND | WET\_IN\_WET |DRY\_AND\_SAND\_2\_TIMES] |
| AztThreeLayerLacquerMode | String | 3-Schicht Lackierung  [DRY\_AND\_SAND | WET\_IN\_WET] |
| StandardEVPrinting | Boolean | Angabe, ob in der Druck-Ansicht die Serienausstattung vorhanden sein soll oder nicht.  true | false]    true: Die Serienausstattung ist in der Druck-Ansicht vorhanden.  false: Die Serienausstattung ist nicht in der Druck-Ansicht vorhanden. |
