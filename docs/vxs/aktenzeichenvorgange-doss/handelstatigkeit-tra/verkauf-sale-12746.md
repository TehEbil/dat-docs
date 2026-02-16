---
title: "Verkauf (Sale)"
topic_id: "12746"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Handelstätigkeit (TradingActivity) > Verkauf (Sale)"
---

# Verkauf (Sale)

Das Element <Sale> ist ein Unterelement von <TradingActivity> und enthält die Details zum Verkauf eines Fahrzeugs.

Zum Setzen der Daten rufen Sie setSalesData auf. Bitte lesen Sie das entsprechende Kapitel "Status umbuchen" durch.

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| OrderDate | Date | Auftragsdatum | Format [YYYY-MM-DD] |
| SellerId | Integer | Eindeutige ID des Verkäufers (Ansprechpartner) | numerisch |
| BusinessType | String | Geschäftsart |  |
| VehicleGroup | String | Fahrzeuggruppe |  |
| SalesPriceNet | Integer | Verkaufspreis (Netto) |  |
| SalesPriceGross | Integer | Verkaufspreis (Brutto) |  |
| DeliveryDate | Date | Auslieferungsdatum | Format [YYYY-MM-DD] |
| MileageVehicle | Integer | Fahrzeug Laufleistung |  |
| MileageOdometer | Integer | Laufleistung entsprechend der Tachoanzeige (km) |  |
| RegistrationNumber | String | Amtliches Kennzeichen |  |
| SalesDetails | String | Verkaufsangaben |  |
| LicenseNumberPurchase | String | Amtliches Kennzeichen zum Zeitpunkt des Ankaufs |  |
| PaymentAgreements | String | Zahlungsvereinbarungen |  |
| OtherAgreements | String | Sonstige Vereinbarungen |  |
| RenewEmissionVehicleInspectionCheck | Boolean | Hauptuntersuchung wird durch den Wert true zum Pflichtfeld | true, false |
| AcceptanceDate | Date | Annahmedatum |  |
| ResidualWarrantyType | String | Restgarantieart |  |
| ResidualWarrantyUntil | Date | Restgarantie bis |  |
| ResidualWarrantyValueNet | Decimal | Restgarantiewert (Netto) |  |
| ResidualWarrantyValueGross | Decimal | Restgarantiewert (Brutto) |  |
| Provider | String | Garantieanbieter |  |
| RepaymentTerm | Integer | Rückzahlungsdauer (Monate) |  |
| StartDate | Date | Beginn der Garantie |  |
| EndDate | Date | Ende der Garantie |  |
| WarrantyNumber | String | Garantienummer |  |
| WarrantyAmountNet | Decimal | Garantiebetrag (Netto) |  |
| WarrantyAmountGross | Decimal | Garantiebetrag (Brutto) |  |
| NextVehicleInspectionDate | Date | Nächste Hauptuntersuchung |  |
| NextEmissionsTestDate | Date | Nächste Abgasuntersuchung |  |
| [Labelling](auszeichnung-l-23960.md) | Labelling | Auszeichnung |  |
| AgreementOnDeviationsCheck | Boolean | Vereinbarung über Abweichungen | true, false |
| ShorteningLimitationPeriodCheck | Boolean | Verkürzung der Verjährungsfrist | true, false |
| ExclusionOfObligationToUpdateCheck | Boolean | Ausschluss der Aktualisierungspflicht | true, false |
| UpdateInformationCheck | Boolean | Information zur Aktualisierung | true, false |
| InfoReqUpdatesAndInstallation | String | Angaben zu den erforderlichen Aktualisierungen und deren Installation |  |
| AgreementOnDeviationsList |  | Vereinbarung über Abweichungen |  |
| WarrantyType | String | Garantietyp |  |
| WarrantyPeriod | Integer | Garantiezeitraum |  |

Element AgreementOnDeviationsList

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| AgreementPosition | Integer | Position in der Liste | numerisch |
| Feature | String | Merkmal der Abweichung |  |
| State | String | Tatsächliche Beschaffenheit |  |
