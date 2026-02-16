---
title: "Summe Reparatur-Kalkulation (RepairCalculationSummary)"
topic_id: "2919"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Summe Reparatur-Kalkulation (RepairCalculationSummary)"
---

# Summe Reparatur-Kalkulation (RepairCalculationSummary)

Im Element <RepairCalculationSummary>, das sich unter den in "[Kalkulationsergebnisse](kalkulationser-1409.md)" aufgeführten Elementen befindet, sind die Summierungen der Reparatur-Kalkulation
(für die Glas-Kalkulation) enthalten.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| SparePartsCosts | complexType, optional,  [SparePartsCostsSummary](sparepartscost-15105.md) | Summenblock Ersatzteile |
| AuxiliaryCosts | complexType, optional,  [AuxiliaryCostsSummary](auxiliarycosts-15531.md) | Summenblock Nebenkosten |
| InspectionCosts | complexType, optional [InspectionCostsSummary](inspectioncost-22886.md) | Summenblock aller Kosten im Zusammenhang mit HU/AU-Positionen |
| LabourCosts | complexType, optional,  [LabourCostsSummary](labourcostssum-15107.md) | Summenblock Arbeitslohn |
| LacquerCosts | complexType, optional,  [LacquerCostsSummary](lacquercostssu-15481.md) | Summenblock Lackierung |
| VATReplacementPart | Decimal, optional | VATReplacementPart ist der Wert des Altteiles wird pauschal mit 10% vom Wert des Austauschteiles angenommen (§10 Umsatzsteuergesetz (UStG). |
| [SurchargesDiscountsCosts](surchargesdisc-15556.md) | complextype, optional,  [SurchargesDiscountsCostsSummary](surchargesdisc-15556.md) | Neu: Summenblock weitere Auf- und Abschläge |
| TotalNetCosts | Decimal, optional | Reparaturkostenkalkulation netto |
| TotalVAT | Decimal, optional | Betrag der Mehrwertsteuer / EUR |
| TotalGrossCosts | Decimal, optional | Reparaturkostenkalkulation brutto |
| TotalNetDiscount | Decimal, optional | Rabatte netto / EUR |
| TotalVATDiscount | Decimal, optional | Betrag der Mehrwertsteuer / EUR aller Rabatte |
| TotalGrossDiscount | Decimal, optional | Rabatte brutto / EUR |
| TotalNetDeductible | Decimal, optional |  |
| TotalVATDeductible | Decimal, optional |  |
| TotalGrossDeductible | Decimal, optional |  |
| TotalNetCorrected | Decimal, optional | korrigierte Reparaturkosten netto |
| TotalVATCorrected | Decimal, optional | korrigierter Mehrwertsteuerbetrag |
| TotalGrossCorrected | Decimal, optional | korrigierter Reparaturkosten brutto |
| TotalAppreciationExVAT | Decimal, optional | Steuerneutrale Wertverbesserung    Die Eingabe bzw. Übergabe ist ausschließlich in der SilverDAT calculateExpert erlaubt.  In der SilverDAT myClaim (SilverDAT 3 Pro Netz) und SilverDAT calculatePRO ist der Import einer steuerneutralen Wertverbesserung aus der SilverDAT calculateExpert möglich.  In diesem Fall fließt die Wertverbesserung ohne Auswirkung oder Ausweis der Mehrwertsteuer ein.  Das Überschreiben dieses Wertes ist nicht gestattet. |
| TotalInspectionCosts | Decimal, optional | Summe für Inspektionspositionen (HU/AU-Positionen) (nicht-steuerneutralen Kosten ) |
| TotalTaxNeutralCosts | Decimal, optional | Summe der steuerneutralen Kosten für Inspektionspositionen (HU/AU-Positionen) |
| RetentionTotalNet | Decimal, optional |  |
| RetentionTotalGross | Decimal, optional |  |
| DiffCommonToOptimizedAmount | Decimal, optional |  |
| DiffCommonToOptimizedPerc | Decimal, optional |  |
| DiffToUpe | Decimal, optional |  |
| UpeInProcent | Decimal, optional |  |
| AmountCustomer | Decimal, optional | Anteil Auftraggeber |
| AmountInsurance | Decimal, optional | Anteil Versicherung |
| SumNet | Decimal, optional | Gesamtsumme netto |
| SumGross | Decimal, optional | Gesamtsumme brutto |
| SumSparePartCosts | Decimal, optional | Zwischensumme Ersatzteile |
| SumSmallSparePartCosts | Decimal, optional | Zwischensumme Kleinersatzteile |
| SumOtherMaterialCosts | Decimal, optional |  |
| SumMiscellaneousCosts | Decimal, optional | Summe "auftragsbezogene Nebenkosten" |
| SumLabourCosts | Decimal, optional | Zwischensumme Arbeitslohn |
| CalculationDeductionsSummary | complexType,optional,  DeductionsSummary | Schluss-Summen (NFA, Wertverbesserung, Vorschaden) |
| AdditionalCostsFlatAmount | Decimal, optional |  |
| TotalNetDiscountExpert | Decimal, optional |  |
| TotalVATDiscountExpert | Decimal, optional |  |
| TotalGrossDiscountExpert | Decimal, optional |  |
| TotalPriceWear | Decimal, optional | Gesamtpreis mit Verschleiß, russische MTPL Berechnung (nur für das Datenland Russland) |
| TotalPriceWearRound | Decimal, optional | Gesamtpreis mit Verschleiß, russische MTPL Berechnung, gerundet nach russischem Recht Anforderungen (nur für das Datenland Russland) |
| BaseNetForWasteDisposalCosts | Decimal, optional | Grundwert der prozentualen Müllentsorgungskosten Berechnung (Betrag in Netto, nur für das Datenland Italien) |
| BaseVatForWasteDisposalCosts | Decimal, optional | Mehrwertsteuerbetrag der Grundwert der prozentualen Müllentsorgungskosten Berechnung (nur für das Datenland Italien) |
| BaseGrossForWasteDisposalCosts | Decimal, optional | Grundwert der prozentualen Müllentsorgungskosten Berechnung (Betrag in Brutto, nur für das Datenland Italien) |
| TotalNetWasteDisposalCosts | Decimal, optional | Gesamtpreis der Müllentsorgungskosten (Betrag in Netto, nur für das Datenland Italien) |
| TotalVatWasteDisposalCosts | Decimal, optional | Mehrwertsteuerbetrag der Müllentsorgungskosten (nur für das Datenland Italien) |
| TotalGrossWasteDisposalCosts | Decimal, optional | Gesamtpreis der Müllentsorgungskosten (Betrag in Brutto, nur für das Datenland Italien) |
| MetaPositions | complexType, optional,  MetaPosition | Key:  TOTAL\_NET\_RISK = Summe der Risiko Positionen als Netto-Wert  VAT\_RISK = Mehrwertsteuer der Risiko Positionen  TOTAL\_GROSS\_RISK = Summe der Risiko Positionen als Brutto Wert  FLAT\_PRICE\_WORK = Gesamtsumme Arbeitslohn Pauschalvorgabe(n)  FLAT\_PRICE\_LACQUER\_POSITIONS = Gesamtsumme Lackierung Pauschalvorgabe(n)  deprecationMethod = Berechnungsmethode der merkantilen Wertminderung  originalPriceWithVat = Neupreis inkl. Mwst.  salesValueWithVat = Veräußerungswert inkl. MwSt.  commercialValueReduction = Merkantile Wertminderung  replacementValueWithVat = Wiederbeschaffungswert inkl. MwSt  DAT\_EUROLACQUER\_IN\_HOURS = DAT Eurolack in Stunden  PRINT\_OPTION\_WITHOUT\_EQUIPMENT = Drucken ohne Ausstattungen  PRINT\_OPTION\_WITHOUT\_EXTENSION = Drucken ohne Reparaturkostenausweitung  FLAT\_PERCENTAGE\_BASE = Grundwert der prozentualen Lackmaterialberechnung  LACQUER\_MATERIAL\_LUMP\_SUM\_SPECIFICATION = Summe der Lackmaterial – Pauschalvorgaben  TIREPROFILE\_FRONTLEFT = Reifenprofiltiefe vorne links  TIREPROFILE\_FRONTRIGHT = Reifenprofiltiefe vorne rechts  TIREPROFILE\_FRONTLEFT2 = Reifenprofiltiefe vorne links 2  TIREPROFILE\_FRONTRIGHT2 = Reifenprofiltiefe vorne rechts 2  TIREPROFILE\_BACK = Reifenprofiltiefe hinten  TIREPROFILE\_BACKLEFT = Reifenprofiltiefe hinten links  TIREPROFILE\_BACKLEFTINSIDE = Reifenprofiltiefe hinten links innen  TIREPROFILE\_BACKRIGHTINSIDE = Reifenprofiltiefe hinten rechts innen  TIREPROFILE\_BACKRIGHT = Reifenprofiltiefe hinten rechts  TIREPROFILE\_BACKLEFTINSIDE2 = Reifenprofiltiefe hinten links innen 2  TIREPROFILE\_BACKRIGHTINSIDE2 = Reifenprofiltiefe hinten rechts innen 2  TIREPROFILE\_BACKRIGHT2 = Reifenprofiltiefe hinten rechts 2  TIREPROFILE\_SPARE = Reifenprofiltiefe Reserverad |
