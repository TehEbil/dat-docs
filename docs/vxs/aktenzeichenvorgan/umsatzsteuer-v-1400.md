---
title: "Umsatzsteuer (VAT)"
topic_id: "1400"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Umsatzsteuer (VAT)"
---

# Umsatzsteuer (VAT)

Das <VAT>-Element enthält Informationen zur Umsatzsteuer und gehört zum <Dossier>.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| VatType | String | Besteuerungsart, „difference" oder „regular" |
| (Dat)VatAtConstructionTime | Decimal | Steuersatz zur Bauzeit |
| (Dat)BaseVatAtConstructionTime | Decimal | Grundsteuersatz zur Bauzeit |
| AddOnTaxAtConstructionTime | Decimal | Zusätzlicher Steuersatz zur Bauzeit Für Datenland AT: NoVA in % |
| (Dat)VatAtValuationTime | Decimal | Steuersatz bei Bewertung |
| (Dat)VatAtSalesTime | Decimal | Steuersatz bei Verkauf |
| (Dat)VatAtPurchaseTime | Decimal | Steuersatz bei Ankauf |
| (Dat)VatAtCalculationTime | Decimal | Steuersatz bei Reparatur-Kalkulation |
