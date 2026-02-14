---
title: "Parameter createContract"
topic_id: "2109"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Methodenüberblick > Methoden > automatische Erzeugung eines Vorgangs mit createContract > Parameter createContract"
---

# Parameter createContract

Pflichtfelder sind alle Felder der Auftragseröffnung. Es müssen nicht alle Pflichtfelder
übergeben werden, aber dann erfolgt eine Nacherfassung in der Auftragseröffnungsmaske.

In jedem Fall muss immer eine OrderNumber mit übergeben werden, da diese nicht in der Auftragseröffnung nacherfasst werden
kann. Fehlt sie in der VXS-Datei, führt dies zu einem Fehler.

Dossier

|  |  |  |  |
| --- | --- | --- | --- |
| Name | Datentyp | Mögliche Werte | Beschreibung |
| Country | String | Land (Country) | Landeskürzel |
| Language | String | Sprachkürzel (Language) | Sprachkürzel |
| Currency | String | Währung (Currency) | Währungskürzel |
| DatCustomerId | String |  | DAT Kundennr. |

VAT

|  |  |  |  |
| --- | --- | --- | --- |
| Name | Datentyp | Mögliche Werte | Beschreibung |
| VatAtCalculationTime | Decimal | z.B. 19 | MWSt. zum Zeitpunkt der Kalkulation |

Owner

|  |  |  |  |
| --- | --- | --- | --- |
| Name | Datentyp | Mögliche Werte | Beschreibung |
| LastName | String |  | Nachname |
| FirstName | String |  | Vorname |
| Title | String | Anrede (Title) | Titel |
| Country | String | s.o. | Landeskürzel |
| VatEntitled | Boolean | true / false | Kalkulation mit oder ohne MWSt. |
| Street | String |  | Straße |
| StreetNumber | String |  | Hausnummer |
| StreetZipCode | String |  | PLZ |
| StreetCity | String |  | Ort |

Vehicle

|  |  |  |  |
| --- | --- | --- | --- |
| Name | Datentyp | Mögliche Werte | Beschreibung |
| VehicleIdentNumber | String |  | 17stellige Vehicle identification number |
| DatECode | String |  | 15stelliger DAT €uropa-Code® |
| InitialRegistration | Date | YYYY-MM-DD | Erstzulassungsdatum |
| MileageOdometer | Integer |  | Kilometerstand |

RegistrationData

|  |  |  |  |
| --- | --- | --- | --- |
| Name | Datentyp | Mögliche Werte | Beschreibung |
| LicenseNumber | String |  | Kfz-Kennzeichen |

RepairOrder

|  |  |  |  |
| --- | --- | --- | --- |
| Name | Datentyp | Mögliche Werte | Beschreibung |
| DamageDate | Date | YYYY-MM-DDTHH:MI:SS | Schadensdatum |
| RepairCoverage | String | Reparaturumfang | Reparaturumfang |
| OrderNumber | String |  | Auftragsnr. |
| DamageNumber | Sstring |  | Schadensnummer |
| PolicyNumber | String |  | Versicherungsscheinnr. |
| Retention | Boolean | true / false | Selbstbehalt |
| RetentionAmount | Decimal |  | Wert des Selbstbehalts |
| InsuranceId | String | Versicherungen | Versicherungs-Nr. |
| DeclarationOfAssignment | Boolean | true / false | Abtretungserklärung liegt vor? |
