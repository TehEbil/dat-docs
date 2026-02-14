---
title: "getGearingOptions"
topic_id: "1950"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getGearingOptions"
---

# getGearingOptions

Beschreibung

Funktion zur Auswahl der verfügbaren Getriebe-Ausstattungsvarianten in Abhängigkeit
vom Basiscode (Fahrzeugart, Hersteller, Haupttyp, Untertyp) und (optional) bereits
gewählten Ausstattungsvarianten

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| restriction | Enumeration | ALL / REPAIR / APPRAISAL | Alle Daten / nur FI-Daten / nur FB-Daten durchsuchen | X |
| vehicleType | Integer | getVehicleTypes | Fahrzeugart | X |
| manufacturer | Integer | getManufacturers | Hersteller | X |
| baseModel | Integer | getBaseModels | Haupttyp | X |
| subModel | Integer | getSubModels | Untertyp | X |
| AvailableOptions | Integer |  | Bereits gewählte klassifizierende Ausstattungen, die die Ausstattungsmenge weiter einschränken. |  |

Parameter constructionTime...

| Name | Datentyp | mögliche Werte | Beschreibung | Pflichtfeld Y/N |
| --- | --- | --- | --- | --- |
| constructionTimeFrom | Integer | [getConstructionPeriods](#showid/8152 "getConstructionPeriodsN") oder 0 - 9999 | Bauzeit von | N |
| constructionTimeTo | Integer | [getConstructionPeriods](#showid/8152 "getConstructionPeriodsN") oder 0 - 9999 | Bauzeit bis | N |

Die Übergabe der beiden Parameter erfolgt optional. Wird die Bauzeit mit übergeben,
erfolgt die Einschränkung der zurückgegebenen Daten abhängig vom Parameter restriction:

| Wert im Parameter restriction | Ergebnis der Einschränkung |
| --- | --- |
| ALL | Die übergebene Bauzeit wird gegen die Bauzeit des Untertyps geprüft. Wird mit dieser Kombination später versucht, Bewertungsdaten zu erhalten, kann das Ergebnis leer sein. |
| APPRAISAL | Die übergebene Bauzeit wird gegen die Bauzeit des Marktindex geprüft. Im Ergebnis kommen nur Werte zurück, die für eine Bewertung geeignet sind. |
| REPAIR | Die übergebene Bauzeit wird gegen die Bauzeit des Untertyps geprüft. Im Ergebnis kommen nur Werte zurück, die für den Bereich der Fahrzeuginstandsetzung geeignet sind. Wird mit dieser Kombination später versucht, Bewertungsdaten zu erhalten, kann das Ergebnis leer sein. |

Rückgabe

Liste der verfügbaren Getriebe-Ausstattungsvarianten und ihren Bezeichnungen analog
zum übergebenen Basiscode (Fahrzeugart, Hersteller, Haupttyp, Untertyp) und der (optional)
bereits gewählten Ausstattungsvarianten.

WSDL

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>?wsdl

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | services | VehicleSelectionService |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | services | VehicleSelectionService |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | services | VehicleSelectionService |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | soap | VehicleSelectionService |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | soap | VehicleSelectionService |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | soap/v2 | VehicleSelectionService |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | soap/v2 | VehicleSelectionService |
