---
title: "getPriceFocusCases"
topic_id: "1979"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getPriceFocusCases"
---

# getPriceFocusCases

Beschreibung

Zusätzlich zum Code, der die technischen Daten des Fahrzeugs verschlüsselt, gibt es
den sogenannten Marktindex. Dieser Code verschlüsselt Daten, die für die Fahrzeugbewertung
relevant sind. Es sind Daten über Fahrzeugwerte, Länder und unterschiedliche Märkte.
Diese Daten sind im sogenannten Marktindex. Die Funktion getPriceFocusCases ermittelt
alle potentiellen Marktindizes, die ein Array mit 1 bis n stringbasierten Wertepaaren
zurückliefert. Das ist beispielsweise DE000 als Schlüssel und DE - Lim3 A 200 CDI,
Elegance DPF, 2005-2007 als Textrepräsentation.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| datECode | String | DAT €uropa-Code® | Gültiger DAT €uropa-Code® | X |

Parameter constructionTime...

| Name | Datentyp | mögliche Werte | Beschreibung | Pflichtfeld Y/N |
| --- | --- | --- | --- | --- |
| constructionTimeFrom | Integer | [getConstructionPeriods](getconstructio-8152.md) oder 0 - 9999 | Bauzeit von | N |
| constructionTimeTo | Integer | [getConstructionPeriods](getconstructio-8152.md) oder 0 - 9999 | Bauzeit bis | N |

Die Übergabe der beiden Parameter erfolgt optional. Wird die Bauzeit mit übergeben,
erfolgt die Einschränkung der zurückgegebenen Daten abhängig vom Parameter restriction:

| Wert im Parameter restriction | Ergebnis der Einschränkung |
| --- | --- |
| ALL | Die übergebene Bauzeit wird gegen die Bauzeit des Untertyps geprüft. Wird mit dieser Kombination später versucht, Bewertungsdaten zu erhalten, kann das Ergebnis leer sein. |
| APPRAISAL | Die übergebene Bauzeit wird gegen die Bauzeit des Marktindex geprüft. Im Ergebnis kommen nur Werte zurück, die für eine Bewertung geeignet sind. |
| REPAIR | Die übergebene Bauzeit wird gegen die Bauzeit des Untertyps geprüft. Im Ergebnis kommen nur Werte zurück, die für den Bereich der Fahrzeuginstandsetzung geeignet sind. Wird mit dieser Kombination später versucht, Bewertungsdaten zu erhalten, kann das Ergebnis leer sein. |

Rückgabe

Potentiell mögliche Marktindizes zum DAT €uropa-Code®

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
