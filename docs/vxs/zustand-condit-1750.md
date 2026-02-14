---
title: "Zustand (Condition)"
topic_id: "1750"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Aufbauten (UpperBodies) > Zustand (Condition)"
---

# Zustand (Condition)

<Condition> ist ein Unter-Element von <Valuation> und <UpperBody> und enthält die Informationen zum Zustand eines Fahrzeugs oder Aufbaus.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| (Dat)OwnerCorrectionPerc | Integer | Wertkorrektur aufgrund der Anzahl der Vorbesitzer in Prozent. Bei fehlendem Eingangsparameter ein Standardwert abhängig von Parameter NumberOfOwnersN. Mögliche Werte liegen zwischen 0 und 15. |
| OwnerCorrectionAmount | Decimal | Korrektursumme ermittelt anhand des Parameters OwnerCorrectionPerc als Netto Wert |
| OwnerCorrectionAmountGross | Decimal | Korrektursumme ermittelt anhand des Parameters OwnerCorrectionPerc als Brutto Wert |
| (Dat)ConditionCorrectionFactorPerc | Decimal | Benutzertwert der Zustandskorrektur in Prozent auf den Händlerverkaufspreis. Mögliche Werte liegen zwischen 70 und 130. |
| ConditionCorrectionAmount | Decimal | Korrektursumme ermittelt anhand des Parameters ConditionCorrectionFactorPerc als Netto Wert |
| ConditionCorrectionAmountGross | Decimal | Korrektursumme ermittelt anhand des Parameters ConditionCorrectionFactorPerc als Brutto-Wert |
| NumberOfOwners | Integer | Anzahl der Halter(veraltet) |
| NumberOfOwnersN | String | Anzahl der Halter |
| NumberOfProprietors | String | Anzahl der Besitzer |
| AccidentDamage | String | Unfallkennzeichen; nur beschreibend, ohne Einfluss auf die Wertkorrektur  weitere Infos siehe Popup-Fenster |
| (Dat)IncreaseInValue | Decimal | Werterhöhung als Netto Wert |
| (Dat)IncreaseInValueGross | Deicmal | Werterhöhung als Brutto Wert |
| CommentIncreaseInValue | String | Kommentar zur Werterhöhung |
| (Dat)TiresMountedValue | Decimal | Wertanpassung aufgrund der montierten Bereifung; Im Fahrzeuggrundwert ist der Neupreis der Serienbereifung mit 50 % enthalten als Netto Wert |
| (Dat)TiresMountedValueGross | Decimal | Wertanpassung aufgrund der montierten Bereifung; Im Fahrzeuggrundwert ist der Neupreis der Serienbereifung mit 50 % enthalten als Brutto-Wert |
| (Dat)TiresUnmountedValue | Decimal | Wertanpassung aufgrund der unmontierten Reifen als Netto Wert |
| (Dat)TiresUnmountedValueGross | Decimal | Wertanpassung aufgrund der unmontierten Reifen als Brutto-Wert |
| (Dat)RepairCosts | Decimal | Kosten noch durchzuführender Reparaturen als Netto Wert |
| (Dat)RepairCostsGross | Decimal | Kosten noch durchzuführender Reparaturen als Brutto-Wert |
| ConditionSubTotal1 | Decimal | Zwischensumme 1, eingerechnet sind: IncreaseInValue, DecreaseInValue, TiresMountedValue, TiresUnmountedValue als Netto Wert |
| ConditionSubTotal1Gross | Decimal | Zwischensumme 1, eingerechnet sind: IncreaseInValue, DecreaseInValue, TiresMountedValue, TiresUnmountedValue als Brutto-Wert |
| ConditionSubTotal2 | Decimal | Zwischensumme 2, eingerechnet sind: OwnerCorrectionAmount, ConditionCorrectionAmount, RepairCosts als Netto Wert |
| ConditionSubTotal2Gross | Decimal | Zwischensumme 2, eingerechnet sind: OwnerCorrectionAmount, ConditionCorrectionAmount, RepairCosts als Brutto-Wert |
| (Dat)DecreaseInValue | Decimal | Wertminderung als Netto Wert |
| (Dat)DecreaseInValueGross | Decimal | Wertminderung als Brutto-Wert |
| CommentDecreaseInValue | String | Kommentar zur Wertminderung |
| NextGeneralInspection | Date | Nächstes Hauptuntersuchungsdatum |
| NextServiceDate | Date | Nächster Kundendiensttermin |
| LastServiceDate | Date | Letzter Kundendiensttermin |
| NextServiceMileage | Integer | Nächster Service bei Kilometerstand |
| LastServiceMileage | Integer | Letzter Service bei Kilometerstand |
| ConditionComment | String | Kommentar zum Zustand |
| DamageAmount | Integer | Schadenhöhe;Voraussetzung: Der Parameter AccidentDamage muss gesetzt sein |
| Damage | String | Art des Schadens bei Neufahrzeugen |
| DamageExtend | Decimal | Schadenshöhe; Voraussetzung: Der Parameter Damage muss gesetzt sein. |
| RepairCostsInTradeMargin | Boolean | Verkauf im reparierten Zustand |
| ConditionRegistrationDate | Date | Datum der letzten Fahrzeuganmeldug |
| ConditionDeregistrationDate | Date | Datum der letzten Fahrzeugabmeldung |
| ConditionCorrectionDescription | String | Grund des Anpassungsfaktors; Voraussetzung: Der Parameter ConditionCorrectionFactorPerc muss gesetzt sein |
| (Dat)BatteryStateOfHealth | Decimal | State of Health der Traktionsbatterie in Prozent |
| (Dat)BatteryCorr | Decimal | Korrekturwert für die Traktionsbatterie in Netto |
| (Dat)BatteryCorrGross | Decimal | Korrekturwert für die Traktionsbatterie in Brutto |
| IdentificationProcedureStateOfHealth | String | Identifikationsverfahren für den Ist-State of Health der Traktionsbatterie |
| ConditionDataAvailable | Boolean | veraltet |
| NextExhaustInspection | Date | Datum der nächsten Abgasinspektion |
| CommentRepairCosts | String | Kommentar zu den Instandsetzungskosten |
| ValueIncreaseList | ValueIncreaseList |  |
| ValueDecreaseList | ValueDecreaseList |  |
| RepairCostList | RepairCostList |  |
