---
title: "Zugang (Admission)"
topic_id: "12745"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Handelstätigkeit (TradingActivity) > Zugang (Admission)"
---

# Zugang (Admission)

Das Element <Admission> ist ein Unterelement von <TradingActivity> und enthält die Details zum Zugang eines Fahrzeugs.

Zum Setzen der Daten rufen Sie die Methode setAdmissionData auf. Bitte lesen Sie den entsprechenden Kapitel "Status umbuchen" durch.

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| AdmissionDate | Date | Ankaufsdatum | Format [YYYY-MM-DD] |
| AdmissionPriceNet | Decimal | Ankaufspreis (EUR) Netto |  |
| AdmissionPriceGross | Decimal | Ankaufspreis (EUR) Brutto |  |
| AcceptanceDate | Date | Hereinnahmedatum | Format [YYYY-MM-DD] |
| AcceptanceDetails | String | Hereinnahmedetails |  |
| MileageVehicle | Integer | Fahrzeug Laufleistung (km) |  |
| MileageOdometer | Integer | Laufleistung entsprechend der Tachoanzeige bei der Hereinnahme des Fahrzeugs (km) |  |
| Location | String | Standort des Fahrzeugs |  |
| DeregistrationDate | Date | Abmeldedatum |  |
| ResidualWarrantyType | String | Restgarantieart |  |
| ResidualWarrantyUntil | Date | Restgarantie bis | Format [YYYY-MM-DD] |
| ResidualWarrantyValueNet | Decimal | Restgarantiewert Netto |  |
| ResidualWarrantyValueGross | Decimal | Restgarantiewert Brutto |  |
| PaymentAgreements | String | Zahlungsvereinbarungen |  |
| OtherAgreements | String | Sonstige Vereinbarungen |  |
| ProvisionOn | Date | Bereitstellung am | Format [YYYY-MM-DD] |
| BuyerId | String | Id des Einkäufers |  |
| VehicleGroup | String | Fahrzeuggruppe |  |
