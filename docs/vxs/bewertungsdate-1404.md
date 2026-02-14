---
title: "Bewertungsdaten (Valuation)"
topic_id: "1404"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Bewertungsdaten (Valuation)"
---

# Bewertungsdaten (Valuation)

| Element | Typ | Beschreibung | Status |
| --- | --- | --- | --- |
| (Dat)OriginalPrice | Decimal | Listenneupreis nach DAT €uropa-Code® + Marktindex (netto) ohne Sonderausstattungen |  |
| (Dat)OriginalPriceGross | Decimal | Listenneupreis nach DAT €uropa-Code® + Marktindex (brutto) ohne Sonderausstattungen |  |
| PrognosisDate | Date | Stichtag der Bewertung im Rahmen der Zukunftsprognose (max. 6 Monate in der Zukunft). |  |
| PricelistDate | Date | Preislistendatum |  |
| (Dat)BasePrice | Decimal | Richtwert nach DAT €uropa-Code® + Marktindex (netto auf Basis der Regelbesteuerung) ohne Sonderausstattungen |  |
| Mileage | Decimal | Kilometerstand (km) | noch nicht aktiv |
| ReferenceMileage | Decimal | Bezugsfahrstrecke lt. DAT (km) |  |
| (Dat)MileageCorr | Decimal | Laufleistungskorrektur(netto) |  |
| AdditionalManualMileageCorr | Decimal | Manuelle Laufleistungskorrektur  Benutzerwert für die noch nicht berücksichtigte Laufleistungsdifferenz |  |
| MinValue4MileageCorr | Integer | Manuelle Laufleistungskorrektur  Minimalwert der Laufleistung für die DAT-Korrektur |  |
| MaxValue4MileageCorr | Integer | Manuelle Laufleistungskorrektur  Maximalwert der Laufleistung für die DAT-Korrektur |  |
| (Dat)InitialRegistrationCorr | Decimal | Erstzulassungskorrektur (netto) |  |
| (Dat)DevaluationFactorPerc | Decimal | Hilfsvariable |  |
| (Dat)BasePrice2 | Decimal | Richtwert nach DAT korrigiert um Laufleistungs- und Erstzulassungskorrektur; Basiswert durch DAT-Ermittlung, netto auf Basis der Regelbesteuerung |  |
| EquipmentSign | String | Kennzeichen, Ausstattungswert Herkunft:  calculated value – Einzelausstattungbewertung  flat-rate value – Pauschaler Ausstattungswert |  |
| ManualEquipmentOriginalPrice | Decimal | Manuelle Vorgabe eines pauschalen Ausstattungsgesamtpreis in Euro als Nettowert. |  |
| (Dat)EquipmentOriginalPrice | Decimal | Listenneupreis der Ausstattungen |  |
| (Dat)EquipmentPrice | Decimal | Bewertungspreis der Ausstattungen |  |
| (Dat)UpperBodiesPrice | Decimal | Restwert der Aufbauten |  |
| (Dat)ValuationCorrection | Decimal | Bewertungskorrektur; Betragswert zu ConditionCorrectionPerc |  |
| (Dat)BasePrice3 | Decimal | Grundwert nach DAT Ermittlung, netto auf Basis der Regelbesteuerung (inkl. Ausstattungen) |  |
| (Dat)ConditionCorrectionPerc | Decimal | Anpassungsfaktor (%): Zustandswertkorrektur in Prozent auf den Händlerverkaufspreis. |  |
| (Dat)SalesPrice | Decimal | Händler-Verkaufspreis netto (inkl. Ausstattungen), unter Berücksichtigung der gewählten Besteuerungsart VatType. |  |
| (Dat)SalesPriceRounded | Decimal | Händler-Verkaufspreis netto (inkl. Ausstattungen) gerundet, unter Berücksichtigung der gewählten Besteuerungsart VatType. |  |
| SalesPricePrognosis | Decimal | Prognostizierter Händler-Verkaufspreis netto (inkl. Ausstattungen) der Zukunftsprognose |  |
| (Dat)SalesPriceGross | Decimal | Händler-Verkaufspreis brutto (inkl. Ausstattungen), unter Berücksichtigung der gewählten Besteuerungsart VatType. |  |
| (Dat)SalesPriceGrossRounded | Decimal | Händler-Verkaufspreis brutto (inkl. Ausstattungen) gerundet, unter Berücksichtigung der gewählten Besteuerungsart VatType. |  |
| SalesPricePrognosisGross | Decimal | Prognostizierter Händler-Verkaufspreis brutto (inkl. Ausstattungen) der Zukunftsprognose |  |
| (Dat)PurchasePrice | Decimal | Händler-Einkaufspreis netto (inkl. Ausstattungen), unter Berücksichtigung der gewählten Besteuerungsart VatType.  Bei Differenzbesteuerung: (DAT)PurchasePrice=(DAT)PurchasePriceGross |  |
| (Dat)PurchasePriceRounded | Decimal | Händler-Einkaufspreis netto (inkl. Ausstattungen) gerundet, unter Berücksichtigung der gewählten Besteuerungsart VatType. |  |
| PurchasePricePrognosis | Decimal | Prognostizierter Händler-Einkaufspreis netto (inkl. Ausstattungen) der Zukunftsprognose |  |
| (Dat)PurchasePriceGross | Decimal | Händler-Einkaufspreis brutto (inkl. Ausstattungen), unter Berücksichtigung der gewählten Besteuerungsart VatType.  Bei Differenzbesteuerung: (DAT)PurchasePrice=(DAT)PurchasePriceGross |  |
| (Dat)PurchasePriceGrossRounded | Decimal | Einkaufspreis brutto (inkl. Ausstattungen) gerundet, unter Berücksichtigung der gewählten Besteuerungsart VatType.  Bei Differenzbesteuerung: (DAT)PurchasePrice=(DAT)PurchasePriceGross |  |
| PurchasePricePrognosisGross | Decimal | Prognostizierter Einkaufspreis (inkl. Ausstattungen) der Zukunftsprognose (Brutto) |  |
| RoundedPurchasePrice | Decimal | Händler-Einkaufspreis netto (inkl. Ausstattungen), basierend auf PurchasePrice gerundet. |  |
| RoundedPurchasePriceGross | Decimal | Händler-Einkaufspreis brutto (inkl. Ausstattungen), basierend auf PurchasePriceGross gerundet. |  |
| (Dat)Margin | Decimal | Handelsspanne (Netto) |  |
| (Dat)MarginRounded | Decimal | Handelsspanne (Netto gerundet) |  |
| MarginPrognosis | Decimal | Prognostizierte Handelsspanne Netto der Zukunftsprognose |  |
| (Dat)MarginGross | Decimal | Handelsspanne (Brutto) |  |
| (Dat)MarginGrossRounded | Decimal | Handelsspanne (Brutto gerundet) |  |
| MarginPrognosisGross | Decimal | Prognostizierte Handelsspanne Brutto der Zukunftsprognose |  |
| MarginPerc | Decimal | Handelsspanne in Prozent |  |
| LastValuationDataYear | Integer | Datenstand (Jahr) als Basis der Bewertung |  |
| LastValuationDataMonth | Integer | Datenstand (Monat) als Basis der Bewertung |  |
| LastValuationDataMonthSer | Integer |  | noch nicht aktiv |
| PrognosisMileageDat | Integer | Voraussichtliche Laufleistung laut DAT (km) der Zukunftsprognose |  |
| PrognosisMileageUser | Integer | Benutzervorgabe für die voraussichtliche Laufleistung (km) der Zukunftsprognose |  |
| LastValuationDate | DateTime | Zeitpunkt dieser Bewertung |  |
| ExpertsSurveyDate | Date |  | noch nicht aktiv |
| SurveyorUserId | String |  | noch nicht aktiv |
| Currency | String | Währung des Bewertungsergebnisses |  |
| DefaultPlatformPresent | String | Gibt an, ob ein Serienaufbau verfügbar und verbaut ist.  present = Serienaufbau vorhanden designed but missing = Serienaufbau abgewählt not designed and missing = nicht vorhanden |  |
| SignMilageUnit | String | Einheit der Laufleistung (kilometers) |  |
| Obsolete | String | Kennzeichen  up to date - aktuell obsolete - veraltet |  |
| ObsoletePrognosis | Integer | Kennzeichen für die Zukunftsprognose  0 - aktuell 1 - veraltet |  |
| DisplayGross | Boolean | Kennzeichen  true - Anzeige als Bruttopreise  false - Anzeige als Nettopreise |  |
| DisplayRounded | Boolean | Kennzeichen  true - Anzeige gerundeter Wertangaben |  |
| ResultInformation | String |  | noch nicht aktiv |
| (Dat)DefaultTiresPrice | Decimal | Berücksichtigter Wert der Serienbereifung (50%) |  |
| SignDeterminatedDate | Boolean | Kennzeichen  true - Stichtagbewertung ist aktiv |  |
| DeterminatedDate | Date | Stichtag für die Bewertung |  |
| Version | String | Versionsangabe für das neue Verfahren, max. 4 Zeichen |  |
| Approval | String | Hashwert für die Freigabe der rückwirkenden Bewertung, für die eine zusätzliche Gebühr erhoben wird.  In diesem Fall Pflicht für SilverDAT 3 valuateExpert /valuateExpertPlusPartner |  |
| ContractNo | String |  | noch nicht aktiv |
| ValuationType | String | Bewertungsart |  |
| ExtendedMileageCorrection | Boolean | Kennzeichen; ohne Auswirkung, da die Berechnung immer mit erweiterter Kilometerkorrektur stattfindet. |  |
| LimitationMileageCorrPerc | Decimal | Begrenzung der Kilometerkorrektur |  |
| ResidualValueModel | String | Restwertmodell |  |
| Condition | Condition |  |  |
| Parameters | Parameters |  |  |
| Forecasts | Forecasts |  |  |
| DossierIdvPro | Integer | Für Vorgänge aus der Datenübernahme: DossierId des Vorgangs in SilverDAT 3 valuatePro |  |
| InspectionDate | Date | Besichtigungsdatum |  |
| InspectedBy | String | Name der Person, die das Fahrzeug besichtigt hat |  |
| ValuationRepairParameters | ValuationRepairParameters |  |  |
| ValuationRepairPositions | ValuationRepairPositions |  |  |
| ValuationRepairCosts | ValuationRepairCosts |  |  |
| Warning | String | Warnmeldung zur Bewertung |  |
