---
title: "getSubModelsByTextSearch"
topic_id: "1805"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getSubModelsByTextSearch"
---

# getSubModelsByTextSearch

Diese Funktion erlaubt eine Freitextsuche nach Fahrzeugen und liefert die möglichen
Untertypen. Zusätzlich zum Suchtext kann optional auch eine BauzeitVon (ConstructionTimeFrom)
und eine BauzeitBis (ConstructionTimeTo) zur Einschränkung der Suche mitgegeben werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| Restriction | Enumeration | ALL / REPAIR / APPRAISAL | Alle Daten / nur FI-Daten / nur FB-Daten durchsuchen | X |
| constructionTimeFrom | Integer | s. [date2ConstructionTime](date2construct-1807.md) | Bauzeit von |  |
| constructionTimeTo | Integer | s. date2ConstructionTime | Bauzeit bis |  |
| searchText | string |  | zu suchender Text | X |

Rückgabe

- Die Anzahl der maximal ermittelten Fahrzeuge (Untertypen) ist momentan auf 100 begrenzt.
- Die Funktion liefert die Anzahl der gefundenen und die Anzahl der zurückgelieferten
  Fahrzeuge zurück:

| Element | Beschreibung |
| --- | --- |
| countOfSubModelsFound | Anzahl der durch die Suche gefundenen Untertypen |
| countOfSubModelsReturned | Anzahl der zurückgelieferten Untertypen (momentan max. 100) |

- Die Ergebnisse werden nach der Anzahl der UTV für den jeweiligen Untertyp und danach
  alphabetisch geordnet.Gibt es kein Ergebnis für die Suche, dann sind die Werte für
  countOfSubModelsFound und countOfSubModelsReturned jeweils 0.
- Ist die Anzahl der gefundenen Untertypen größer als 100, sollte die Suche eventuell
  eingeschränkt werden.
- Die Ergebnismenge wird jeweils anhand eines [Response getSubModelsByTextSearch](response-getsu-1809.md) zurückgegeben.

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
