---
title: "Validierung von Fahrzeugkonfigurationen"
topic_id: "15767"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Funktionsreferenz > Validierung von Fahrzeugkonfigurationen"
---

# Validierung von Fahrzeugkonfigurationen

| Funktionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| validateConfiguration | POST | Ermittelt, ob die angegebene Fahrzeugkonfiguration für das angegebene Derivat zulässig ist. | Objekt mit Validierungsergebnis |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| derivativeId | String | Derivat-ID | Eine der Derivat-Kennungen, die von getDerivatives geliefert werden | ja |
| version | Number | Gültige Workbook-Version | Version des Workbooks dessen Fahrzeugkonfiguration validiert werden soll | nein |
| optionIds | Array | Options-IDs | Ein oder mehrere Kennungen von Optionen, die für das angegebene Derivat verfügbar sind | nein |
| colourId | String | ID der Außenfarbe | Eine der Kennungen von Außenfarben, die für das angegebene Derivat verfügbar sind | ja, wenn keine Farbe indirekt mittels Umfasst-Logik definiert ist |
| upholsteryId | String | ID der Polster | Eine der Kennungen von Polsterpositionen, die für das angegebene Derivat verfügbar sind | ja, wenn kein Polster indirekt mittels Umfasst-Logik definiert ist |

Das ausgegebene Objekt hat die folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung |
| --- | --- | --- | --- |
| errorCode | Zahl |  | 0, wenn die Konfiguration gültig ist, sonst ein Code aus der unten angegebenen Code-Liste, der die Art des Fehlers angibt |
| logicErrorCode | Zahl |  | Nur angegeben, wenn errorCode ERR\_LOGIC ist; gibt den Typ des aufgetretenen Logikfehlers an (für Berichtszwecke) |
| errorDetails | Array |  | Nur angegeben, wenn errorCode nicht 0 ist; Inhalt abhängig vom Fehlertyp |
| configurationResult | Objekt | ``` {   "optionIds": [     <id>, ...   ],   "colourId": <id>,   "upholsteryId": <id> } ``` | Nur angegeben, wenn errorCode 0 ist; enthält die resultierende Fahrzeugkonfiguration mit den angegebenen und den enthaltenen Ausstattungspositionen |

Die gelieferten Fehler und Details können folgende Werte haben:

| Fehlercode | Bedeutung | Beschreibung | Gelieferte Fehlerdetails | Beschreibung der Fehlerdetails |
| --- | --- | --- | --- | --- |
| 1 | ERR\_ALREADY\_INCLUDED | Die angegebenen Optionen / Farben / Polsterpositionen sind bereits in einer anderen Option / Farbe / Polsterposition enthalten | [<id1>, <id2>, ...] | Kennungen der enthaltenen Optionen / Farben / Polster |
| 2 | ERR\_REQUIRED\_MISSING | Eine oder mehrere Positionen, die von einer anderen Position benötigt werden, sind nicht enthalten und nicht angegeben | [<id1>, <id2>, ...] | Kennungen der benötigten Optionen / Farben / Polster |
| 3 | ERR\_EXCLUDED\_SPECIFIED | Die angegebenen Positionen werden durch eine andere enthaltene oder angegebene Position ausgeschlossen | [<id1>, <id2>, ...] | Kennungen der ausgeschlossenen Optionen / Farben / Polster |
| 4 | ERR\_DUPLICATE\_SPECS | Die angegebenen Optionen definieren zusammen mehrere Instanzen einer singulären Fahrzeugeigenschaft, z.B. Lenkrad; oder die Fahrzeugkonfiguration definiert mehr als eine Farbe oder ein Polster | [<id1>, <id2>, ...] | Array von Optionskennungen, die die duplizierte Fahrzeugeigenschafts-Position spezifizieren; oder Array von Kennungen konfigurierter Farben / Polster |
| 5 | ERR\_UNKNOWN\_ITEM | Die angegebenen Options- / Farb- / Polsterkennungen existieren nicht oder sind für das Derivat nicht verfügbar | [<id1>, <id2>, ...] | Kennung der unbekannten Optionen / Farben / Polsterungen |
| 6 | ERR\_MISSING\_INPUT | Der Parameter derivativeId wurde nicht angegeben oder es ist keine Farbe / kein Polster definiert, weder durch Parameter noch mittels Umfasst-Logik | [<pn1>, <pn2>, ...] | Array fehlender Parameternamen |
| 7 | ERR\_ILLEGAL\_SELECTION | Mehr als eine Position einer erforderlichen Auswahl / keine oder mehr als eine Position einer Umfasst-Auswahl wurde angegeben | [<id>] | Kennung der enthaltenen / erforderlichen Options- / Farb- / Polsterpositionen |
| 8 | ERR\_LOGIC | Es liegt ein Fehler in der logischen Definition einer Option / Farbe / eines Polsters vor | [<id1>, <id2>, ...] | [<type1>, <type2>, ...] | Kennungen der fehlerhaften Options- / Farb- / Polsterpositionen oder Logiktypnamen |

Der Fehlercode 4 wird gemeldet, wenn die bereitgestellten Konfigurationsdaten mehr
als eine Auswahl für mindestens eine der folgenden Positionen ergeben, die in dieser
Reihenfolge überprüft werden:

- specs.interior.steeringWheel.wheelType
- specs.wheelsTyres.rimType
- specs.infotainment.navigation.navType
- specs.warranty.months

Eine Beschreibung der Validierungslogik und Beispiele finden Sie im Anhang.
