---
title: "Zustandsdaten anlegen"
topic_id: "11055"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Zustandsdaten anlegen"
---

# Zustandsdaten anlegen

Mit der Funktion setConditionDetails legen Sie Zustandsdaten zu einem bestehenden Vorgang an. Für die drei Kategorien:
Kosten noch durchzuführender Reparaturen, Werterhöhungen und Wertminderungen können
Sie Zustandsdetails anlegen und bearbeiten. Sie legen ein neues Zustandsdetail an,
indem Sie die Unterelemente von RepairCostList, ValueIncreaseList und ValueReductionList mit Werten belegen.

Die Zustandsdetails können Sie ebenfalls im Dossier unter dem Element Condition einsehen mithilfe der Methode getDossier. Die Details werden im Dossier nicht einzeln aufgelistet (siehe auf dieser Seite
unten für weitere Details). Die Bewertung im Dossier wird sofort nach dem Aufruf der
Funktion setConditionDetails aktualisiert. Die Funktion updateDossier wird hierfür nicht benötigt.

Parameter setConditionDetails

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Eindeutige Vorgangskennung | numerisch | X |
| AccidentDamage | String | Unfallkennzeichen (nur beschreibend, ohne Einfluss auf Wertkorrektur) | UNKN=unbekannt  ACFRE=unfallfrei  ACDNR=nicht reparierter Unfallschaden  ACDR=reparierter Schaden  Yes=Ja  No=Nein |  |
| Comments | String | Bemerkungen |  |  |
| Condition | String | Zustand | VGOOD=sehr gut  GOOD=gut  NORML=normal  SUFNT=ausreichend  INADQT=mangelhaft  INSUFNT=unzureichend |  |
| LastServiceDate | DateTime | Letzter Kundendienst Datum | YYYY-MM-DD |  |
| LastServiceMileage | Decimal | Letzter Kundendienst Kiilometerstand |  |  |
| NextServiceDate | DateTime | Nächster Kundendienst Datum | YYYY-MM-DD |  |
| NextServiceMileage | Decimal | Nächster Kundendienst Kiilometerstand |  |  |
| NextVehicleInspectionDate | DateTime | Hauptuntersuchungsdatum | MM-YYYY |  |
| TiresMountedValueGross | Decimal | Zu-/Abschlag der montierten Reifen (Differenz zur Serienbereifung) (EUR) Brutto | ###########.## |  |
| TiresMountedValueNet | Decimal | Zu-/Abschlag der montierten Reifen (Differenz zur Serienbereifung) (EUR) Netto | ###########.## |  |
| TiresUnmountedValueGross | Decimal | Restwert der unmontierten Reifen (EUR) Brutto | ###########.## |  |
| TiresUnmountedValueNet | Decimal | Restwert der unmontierten Reifen (EUR) Netto | ###########.## |  |
| RepairCostList | repairCostDetailsRequest | Die zugehörigen Kindelemente enthalten die Zustandsdetails der Kategorie: Reparaturkosten |  |  |
| ValueIncreaseList | valueIncreaseDetailsRequest | Die zugehörigen Kindelemente enthalten die Zustandsdetails der Kategorie: Werterhöhungen |  |  |
| ValueReductionList | valueReductionDetailsRequest | Die zugehörigen Kindelemente enthalten die Zustandsdetails der Kategorie: Wertminderungen |  |  |
| ConditionRegistrationDate | Date | Datum der letzten Fahrzeuganmeldug | YYYY-MM-DD |  |
| ConditionDeregistrationDate | Date | Datum der letzten Fahrzeugabmeldung | YYYY-MM-DD |  |

Element vxs:RepairCostList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| RepairCost | conditionDetailsRequest | Beschreibung |  |  |
| UserDefinedValueGross | Decimal | Geldbetrag (EUR) Brutto | +###########.## |  |
| UserDefinedValueNet | Decimal | Geldbetrag (EUR) Netto | +###########.## |  |

Element vxs:RepairCost

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Description | String | Beschreibung |  |  |
| ValueGross | Decimal | Geldbetrag (EUR) Brutto | +###########.## |  |
| ValueNet | Decimal | Geldbetrag (EUR) Netto | +###########.## |  |

Element vxs:ValueIncreaseList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ValueIncrease | conditionDetailsRequest | Beschreibung |  |  |
| UserDefinedValueGross | Decimal | Geldbetrag (EUR) Brutto | +###########.## |  |
| UserDefinedValueNet | Decimal | Geldbetrag (EUR) Netto | +###########.## |  |

Element vxs:ValueIncrease

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Description | String | Beschreibung |  |  |
| ValueGross | Decimal | Geldbetrag (EUR) Brutto | +###########.## |  |
| ValueNet | Decimal | Geldbetrag (EUR) Netto | +###########.## |  |

Element vxs:ValueReductionList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ValueReduction | conditionDetailsRequest | Beschreibung |  |  |
| UserDefinedValueGross | Decimal | Geldbetrag (EUR) Brutto | +###########.## |  |
| UserDefinedValueNet | Decimal | Geldbetrag (EUR) Netto | +###########.## |  |

Element vxs:ValueReduction

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Description | String | Beschreibung |  |  |
| ValueGross | Decimal | Geldbetrag (EUR) Brutto | +###########.## |  |
| ValueNet | Decimal | Geldbetrag (EUR) Netto | +###########.## |  |

Zustandsdetails im Dossier

Falls es einen Benutzerwert gibt, dann finden Sie

- den Wert des Elements RepairCostsDetail.SumValueGross im Response von setConditionDetails ebenfalls im Element Condition.RepairCostsGross der Funktion getDossier.
- den Wert des Elements ValueIncreaseDetails.SumValueGross im Response von setConditionDetails ebenfalls im Element Condition.IncreaseInValue der Funktion getDossier.
- den Wert des Elements ValueReductionDetails.SumValueGross im Response von setConditionDetails ebenfalls im Element Condition.DecreaseInValueGross der Funktion getDossier.

Falls es einen Benutzerwert gibt, dann finden Sie

- den Wert des Elements RepairCostsDetail.UserDefinedValueGross im Response von setConditionDetails ebenfalls im Element Condition.RepairCostGross der Funktion getDossier.
- den Wert des Elements ValueIncreaseDetails.UserDefinedValueGross im Response von setConditionDetails ebenfalls im Element Condition.ValueIncreaseGross der Funktion getDossier.
- den Wert des Elements ValueReductionDetails.UserDefinedValueGross im Response von setConditionDetails ebenfalls im Element Condition.ValueReductionGross der Funktion getDossier.

Der Paramter ConditionDetailSubTotal1 wird aus den folgenden Parameter im createDossierResponse zusammengerechnet: basicValue + increaseInValue - decreaseInValue + tyresMountedValue + tyresUnmountedValue.

Der Paramter ConditionDetailSubTotal2 wird aus den folgenden Parameter im createDossierResponse zusammengerechnet: conditionSubTotal1 + ownerCorrectionAmount + conditionFactorAmount.
