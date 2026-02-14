---
title: "Verkaufsangebote (SalesOfferList)"
topic_id: "22414"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Weitere Handelsdaten (TradingAdditional) > Verkaufsangebote (SalesOfferList)"
---

# Verkaufsangebote (SalesOfferList)

Element vxs:SalesOfferList

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| SalesOffer | SalesOffer | enthält Daten eines Verkaufsangebots |  |

Element vxs:PurchaseOffer

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| SalesPriceNet | Decimal | Verkaufspreis (EUR) netto |  |
| SalesPriceGross | Decimal | Verkaufspreis (EUR) Brutto |  |
| SalesOfferNumber | String | Angebotsnummer |  |
| OfferDate | Date | Angebotsdatum | YYYY-MM-DD |
| ResubmissionDate | Date | Wiedervorlagedatum | YYYY-MM-DD |
| GuaranteeDate | Date | Garantie | YYYY-MM-DD |
| OfferedBy | String | ID des Anbieters | numerisch |
| Titles | String | Anrede |  |
| Comments | String | Bemerkung |  |
| Agreements | String | Vereinbarung |  |
| NextEmissionsTestDate | Date | Nächste Abgasuntersuchung. | MM-YYYY |
| NextVehicleInspectionDate | Date | Hauptuntersuchungsdatum | MM-YYYY |
| RenewEmissionVehicleInspectionCheck | Boolean | Hauptuntersuchung wird durch den Wert true zum Pflichtfeld |  |
