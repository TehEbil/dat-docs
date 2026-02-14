---
title: "Handelsdaten (TradingData)"
topic_id: "1402"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Handelsdaten (TradingData)"
---

# Handelsdaten (TradingData)

Das <TradingData>-Element enthält Informationen für den An- und Verkauf und gehört zum <Dossier>. In Unterelementen sind u.a. die Adress-Informationen der Ansprechpartner enthalten.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| PurchasePriceNet | decimal | Einkaufspreis netto |
| PurchasePriceGross | decimal | Einkaufspreis brutto |
| SalesPriceNet | decimal | Verkaufspreis netto |
| SalesPriceGross | decimal | Verkaufspreis brutto |
| SalesPriceMarket | decimal | Auszeichnungspreis |
| SalesPriceMinimum | decimal | Mindestverkaufspreis |
| SalesPriceReseller | decimal | Verkaufspreis für Wiederverkäufer |
| OwnType | string | Eigentyp |
| EuVehicle | boolean | EU-Fahrzeug? |
| Location | string | Fahrzeug-Standort |
| ExportReportState | string | Meldestatus für Börsen (abhängig vom Partner) |
| ClaimFormId | string | Meldekartennummer |
| Owner |  | [s. Address](adressdaten-ad-1375.md) |
| PrevOwner |  | [s. Address](adressdaten-ad-1375.md) |
| Reservation |  | [s. Address](adressdaten-ad-1375.md) |
| Insurance |  | s. Address |
| Insurant |  | s. Address |
| Driver |  | [s. Address](adressdaten-ad-1375.md) |
| Opponent |  | [s. Address](adressdaten-ad-1375.md) |
| Expert |  | [s. Address](adressdaten-ad-1375.md) |
| Dealership |  | [s. Address](adressdaten-ad-1375.md) |
| Prospects |  | [s. Address](adressdaten-ad-1375.md) |
| [AddonList](#expandblock-1402-d2e10783)  Element vxs:AddonList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | [Addon](#expandblock-1402-12756-d2e212994)  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | name="LabellingPrice" | String | Auszeichnung (EUR) Netto |  | | name="LabellingPriceGross" | String | Auszeichnung (EUR) Brutto |  | | name="ResellerPrice" | String | Wiederverkäuferpreis Netto |  | | name="ResellerPriceGross" | String | Wiederverkäuferpreis Brutto |  | | name="SPMinimum" | String | Mindest-Verkaufspreis Netto |  | | name="SPMinimumGross" | String | Mindest-Verkaufspreis Brutto |  | | name="DEVIATING\_MARKETPLACE\_PRICE" | String | Abweichender Börsenpreis | true, false | | name="MarketPriceLabelling" | String | Angebotspreis Börse Netto |  | | name="MarketPriceLabellingGross" | String | Angebotspreis Börse Brutto |  | | name="MarketplaceProductionCountryVersion" | String | Landesversion |  | |  | Enthält Werte im Attribut Name siehe Link |  | | Liste | Börsenaufbereitung Preise, falls der Parameter Coverage auf MARKETPLACEEXPORT gesetzt ist.  Details siehe Link |
