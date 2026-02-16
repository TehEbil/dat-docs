---
title: "Zustandsdaten ändern"
topic_id: "11059"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Zustandsdaten ändern"
---

# Zustandsdaten ändern

Mit der Funktion changeConditionDetails verändern Sie die Zustandsdaten zu einem bestehenden Vorgang.

Parameter changeConditionDetails

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Eindeutige Vorgangskennung | numerisch | X |
| AccidentDamage | String | Unfallkennzeichen (nur beschreibend, ohne Einfluss auf Wertkorrektur) | UNKN=unbekannt  ACFRE=unfallfrei  ACDNR=nicht reparierter Unfallschaden  ACDR=reparierter Schaden  Yes=Ja  No=Nein |  |
| Comments | String | Bemerkungen |  |  |
| Condition | String | Zustand | VGOOD=sehr gut  GOOD=gut  NORML=normal  SUFNT=ausreichend  INADQT=mangelhaft  INSUFNT=unzureichend |  |
| LastServiceDate | DateTime | Letzter Kundendienst Datum | YYYY-MM-DD |  |
| LastServiceMileage | Decimal | Letzter Kundendienst Kilometerstand |  |  |
| NextServiceDate | DateTime | Nächster Kundendienst Datum | YYYY-MM-DD |  |
| NextServiceMileage | Decimal | Nächster Kundendienst Kilometerstand |  |  |
| NextVehicleInspectionDate | DateTime | Hauptuntersuchungsdatum | MM-YYYY |  |
| TiresMountedValueGross | Decimal | Zu-/Abschlag der montierten Reifen (Differenz zur Serienbereifung) (EUR) in Brutto | ###########.## |  |
| TiresMountedValueNet | Decimal | Zu-/Abschlag der montierten Reifen (Differenz zur Serienbereifung) (EUR) in Netto | ###########.## |  |
| TiresUnmountedValueGross | Decimal | Restwert der unmontierten Reifen (EUR) in Brutto | ###########.## |  |
| TiresUnmountedValueNet | Decimal | Restwert der unmontierten Reifen (EUR) in Netto | ###########.## |  |
| RepairCostList | changeRepairCostDetailsRequest | Die zugehörigen Kindelemente enthalten die Zustandsdetails der Kategorie: Reparaturkosten |  |  |
| ValueIncreaseList | changeValueIncreaseDetailsRequest | Die zugehörigen Kindelemente enthalten die Zustandsdetails der Kategorie: Werterhöhungen |  |  |
| ValueReductionList | changeValueReductionDetailsRequest | Die zugehörigen Kindelemente enthalten die Zustandsdetails der Kategorie: Wertminderungen |  |  |
| ConditionRegistrationDate | Date | Datum der letzten Fahrzeuganmeldung | YYYY-MM-DD |  |
| ConditionDeregistrationDate | Date | Datum der letzten Fahrzeugabmeldung | YYYY-MM-DD |  |

Element vxs:RepairCostList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| RepairCost | changeRCConditionDetails | Beschreibung |  |  |
| UserDefinedValueGross | Decimal | Geldbetrag (EUR) in Brutto | +###########.## |  |
| UserDefinedValueNet | Decimal | Geldbetrag (EUR) in Netto | +###########.## |  |

Element vxs:RepairCost

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| RepairCostId | Long | Eindeutige Nummerierung  der Reparaturkosten |  |  |
| Description | String | Beschreibung |  |  |
| ValueGross | Decimal | Geldbetrag (EUR) in Brutto | +###########.## |  |
| ValueNet | Decimal | Gelsbetrag (EUR) in Netto | +###########.## |  |

Element vxs:ValueIncreaseList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ValueIncrease | changeVIConditionDetails | Beschreibung |  |  |
| UserDefinedValueGross | Decimal | Geldbetrag (EUR) in Brutto | +###########.## |  |
| UserDefinedValueNet | Decimal | Geldbetrag (EUR) in Netto | +###########.## |  |

Element vxs:ValueIncrease

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ValueIncreaseId | Long | Eindeutige Nummerierung  der Werterhöhung |  |  |
| Description | String | Beschreibung |  |  |
| ValueGross | Decimal | Geldbetrag (EUR) in Brutto | +###########.## |  |
| ValueNet | Decimal | Geldbetrag (EUR) in Netto | +###########.## |  |

Element vxs:ValueReductionList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ValueReduction | changeVRConditionDetails | Beschreibung |  |  |
| UserDefinedValueGross | Decimal | Geldbetrag (EUR) in Brutto | +###########.## |  |
| UserDefinedValueNet | Decimal | Geldbetrag (EUR) in Netto | +###########.## |  |

Element vxs:ValueReduction

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ValueReductionId | Long | Eindeutige Nummerierung  der Wertminderung |  |  |
| Description | String | Beschreibung |  |  |
| ValueGross | Decimal | Geldbetrag (EUR) in Brutto | +###########.## |  |
| ValueNet | Decimal | Geldbetrag (EUR) in Netto | +###########.## |  |
