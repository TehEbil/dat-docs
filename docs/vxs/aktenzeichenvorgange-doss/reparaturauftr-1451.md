---
title: "Reparaturauftrag (RepairOrder)"
topic_id: "1451"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Reparaturauftrag (RepairOrder)"
---

# Reparaturauftrag (RepairOrder)

| Element | Typ | Beschreibung | Mögliche Werte |
| --- | --- | --- | --- |
| DamageDate | date | Tag des Schadens z. B 2016-09-12 |  |
| RepairCoverage | String | Reparaturumfang |  |
| OrderNumber | String | Ordnungsnummer (optional) |  |
| InvoiceNumber | String |  |  |
| JobNumber | String | Auftragsnummer |  |
| DamageNumber | String | Schadensnummer z. B 4711-08152145 |  |
| PolicyNumber | String | Versicherungsscheinnummer z. B. 1234567-66-66 |  |
| Retention | Boolean | Selbstbehalt (ja/nein) | true / false |
| RetentionAmount | Decimal | Wert des Selbstbehalts |  |
| InsuranceId | String | Eindeutige Kennungsnummer des Unternehmens in der Versicherungswirtschaft (nur selbstaendige Versicherungskonzerne, im Gegensatz zu InsuranceNumber), [hier](../wertelisten/versicherungen-2113.md) finden Sie eine Liste der Versicherungs-IDs und dazugehörige Versicherung. |  |
| InsuranceGroupId | String | Versicherungsgruppe (über die Funktion [getInsurances](../../produkte/silverdat-calculatepro-si/schnittstellenoperat/abrufen-von-la-2333.md) aufrufbar) |  |
| ServiceProviderId | String |  |  |
| InsuranceType | String | Versicherungsart | none = Haftpflicht  partial = Teilkasko  comprehensive = Vollkasko |
| InsuranceNumber | String | Eindeutige Kennungsnummer des Versicherungsunternehmens (im Gegensatz zu InsuranceID werden auch Tochterunternehmen des gleichen Konzerns unterschieden).  Über die Funktion [getInsurances](../../produkte/silverdat-calculatepro-si/schnittstellenoperat/abrufen-von-la-2333.md) aufrufbar. |  |
| InsuranceAgency | String | Versicherungsdienstleister |  |
| TypeOfInsurance | Integer | Versicherungsart des Versicherten | 0 = Haftpflicht,  1 = Teilkasko,  2 = Vollkasko |
| LossLocation | String | Schadenort |  |
| DamageType | Integer | Schadenart | für insuranceType: none:  510 = Kfz-Schaden mit/ohne sonstigem Sachschaden  520 = Sachschaden ohne Kfz-Schaden  610 = Todesfall mit Kfz-Schaden und Sachschaden  620 = Todesfall ohne Kfz-Schaden jedoch mit Sachschaden  710 = Verletztenfall mit Kfz-Schaden und Sachschaden  720 = Verletztenfall ohne Kfz-Schaden jedoch mit Sachschaden  875 = Zusatzhaftpflichtversicherung für Handel/Handwerk    für insuranceType: partial:  810 = Unfall/Kollision mit anderen KFZ (VK-Tatbestand)  850 = Unfall ohne Berührung mit anderen KFZ (VK-Tatbestand)  860 = Mut- und böswillige Beschädigung    für insuranceType: comprehensive:  911 = Brand  912 = Explosion  913 = Seng- und Schmorschäden, auch Schäden an Verkabelung  920 = Diebstahl von Fahrzeuginnenteilen  921 = versuchter Totaldiebstahl  922 = Diebstahl von Fahrzeugaußenteilen  930 = Totaldiebstahl  950 = Glasschaden  961 = Sturmschaden  962 = Hagelschaden  963 = Blitz  970 = Überschwemmungsschaden  980 = Wildschaden  981 = Marderbiss |
| InspectionDate | Date | Tag der Besichtigung z. B 2016-09-14 |  |
| BillingCategory | Decimal | Abrechnungsart (wird in autoglas Plus ignoriert und bleibt der internen Nutzung vorbehalten) |  |
| DeclarationOfAssignment | Boolean | Abtretungserklärung liegt vor ja/nein | true / false |
| InsuranceCase | Boolean | Versicherungsfall ja/nein | true / false |
| AdditionalData |  | s. [Zusatzdaten AdditionalData](reparaturauftrag-rep/zusatzdaten-ad-1457.md) |  |
| CreationDateTime | DateTime | Erstellungsnummer  Der Parameter ist vorbelegt, wird aber zurzeit nicht verwendet! |  |
| MetaPositions | MetaPosition |  |  |
| InvoiceDate | DateTime |  |  |
| CountryFlagDamageEvent | String |  |  |
| InsuranceName | String |  |  |
| TokenContributionInInsuranceCase | String |  |  |
| Deleted | Boolean |  | true / false |
| GDVRoutingType | String |  |  |
| Comment | String |  |  |
| DATProcessIdCommentList | complexType, optional  <DATProcessIdComment> | Dient als Elternelement für beliebig viele <DATProcessIdComment>-Elemente. Diese enthalten die vom Benutzer kommentierten Reparaturpositionen. |  |
| EstimatedRepairTimeInDays | Integer | Nur für das Datenland Schweiz: voraussichtliche Reparaturdauer |  |
| ReplacementCar | Boolean | Nur für das Datenland Schweiz:Ersatzwagen | true / false |
| ReplacementCarTimeInDays | Integer | Nur für das Datenland Schweiz:Leihzeit des Ersatzwagens |  |
| ReplacementCarCosts | Decimal | Nur für das Datenland Schweiz:Kosten Ersatzwagen pro Tag (<ReplacementCarTimeInDays>) |  |
| OtherCostsDescription | String | Nur für das Datenland Schweiz:Beschreibung der sonstigen Kosten |  |
| OtherCosts | Decimal | Nur für das Datenland Schweiz:Höhe der sonstigen Kosten (ein Betrag in einer Währung) |  |
| TowingRecoveryCosts | Decimal | Nur für das Datenland Schweiz:Abschlepp-/ Bergungskosten (ein Betrag in einer Währung) |  |
| OtherDeductionsDescription | String | Nur für das Datenland Schweiz:Beschreibung der sonstigen Abzüge |  |
| OtherDeductions | Decimal | Nur für das Datenland Schweiz:Höhe der sonstigen Abzüge (ein Betrag in einer Währung) |  |
| ExternalProcessId | String | Externe Vorgangsnummer |  |
| ExternalCalculationId | String | Externe Kalkulationsnummer |  |
