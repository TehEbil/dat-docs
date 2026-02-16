---
title: "Ankauf (Purchase)"
topic_id: "12744"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Handelstätigkeit (TradingActivity) > Ankauf (Purchase)"
---

# Ankauf (Purchase)

Das Element <Purchase> ist ein Unterelement von <TradingActivity> und enthält die Details zum Ankauf eines Fahrzeugs.

Zum Setzen der Daten rufen Sie die Methode setPurchaseData auf. Bitte lesen Sie den entsprechenden Kapitel "Status umbuchen" durch.

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| BuyerId | Integer | ID des Käufers | numerisch |
| VehicleGroup | String | Fahrzeuggruppe |  |
| DeregistrationDate | Date | Abmeldedatum | Format [YYYY-MM-DD] |
| ResidualWarrantyType | String | Restgarantieart |  |
| ResidualWarrantyUntil | Date | Restgarantie bis | Format [YYYY-MM-DD] |
| ResidualWarrantyValueNet | Decimal | Restgarantiewert (Netto) |  |
| ResidualWarrantyValueGross | Decimal | Restgarantiewert (Brutto) |  |
| PaymentAgreements | String | Zahlungsvereinbarungen |  |
| OtherAgreements | String | Sonstige Vereinbarungen |  |
| PurchaseDate | Date | Ankaufsdatum | Format [YYYY-MM-DD] |
| PurchasePriceNet | Decimal | Einkaufspreis (Netto) |  |
| PurchasePriceGross | Decimal | Einkaufspreis (Brutto) |  |
| MileageExpected | Integer | Voraussichtliche Laufleistung (km) |  |
| ProvisionOn | Date | Bereitstellung am | Format [YYYY-MM-DD] |
| AcceptanceDate | Date | geplantes Hereinnahmedatum |  |
| AcceptanceDetails | String | Hereinnahmedetails |  |
