---
title: "Validierung von Fahrzeugkonfigurationen"
topic_id: "27916"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Funktionsreferenz > Validierung von Fahrzeugkonfigurationen"
---

# Validierung von Fahrzeugkonfigurationen

| Funktionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| validateConfiguration | POST | Ermittelt, ob die angegebene Fahrzeugkonfiguration für das angegebene Derivat zulässig ist. | Objekt mit Validierungsergebnis |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| derivativeId | String | Derivat-ID | Eine der Derivat-Kennungen, die von getDerivatives geliefert werden | ja |
| version | Dezimalzahl | Gültige Workbook-Version | Version des Workbooks dessen Fahrzeugkonfiguration validiert werden soll | nein |
| equipmentIds | Array | Ausstattungs-IDs | Ein oder mehrere Kennungen von optionalen Ausstattungen, die für das angegebene Derivat verfügbar sind. Die Regeln zur Validierung finden Sie im Anhang. | nein |

Das ausgegebene Objekt hat die folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung |
| --- | --- | --- | --- |
| errorCode | Zahl |  | 0, wenn die Konfiguration gültig ist, sonst ein Code aus der unten angegebenen Code-Liste, der die Art des Fehlers angibt |
| logicErrorCode | Zahl |  | Nur angegeben, wenn errorCode ERR\_LOGIC ist; gibt den Typ des aufgetretenen Logikfehlers an (für Berichtszwecke) |
| errorDetails | Array |  | Nur angegeben, wenn errorCode nicht 0 ist; Inhalt abhängig vom Fehlertyp |
| configurationResult | Objekt | ``` {   "equipmentIds": [     <id>, ...   ] } ``` | Nur angegeben, wenn errorCode 0 ist; enthält die resultierende Fahrzeugkonfiguration mit den angegebenen und den enthaltenen Ausstattungspositionen |

Die gelieferten Fehler und Details können folgende Werte haben:

| Fehlercode | Bedeutung | Beschreibung | Gelieferte Fehlerdetails | Beschreibung der Fehlerdetails |
| --- | --- | --- | --- | --- |
| 1 | ERR\_ALREADY\_INCLUDED | Die angegebenen Positionen sind bereits in einer anderen Position enthalten | [<id1>, <id2>, ...] | Kennungen der enthaltenen Ausstattungen |
| 2 | ERR\_REQUIRED\_MISSING | Eine oder mehrere Positionen, die von einer anderen Position benötigt werden, sind nicht enthalten und nicht angegeben | [<id1>, <id2>, ...] | Kennungen der benötigten Ausstattungen |
| 3 | ERR\_EXCLUDED\_SPECIFIED | Die angegebenen Positionen werden durch eine andere enthaltene oder angegebene Position ausgeschlossen | [<id1>, <id2>, ...] | Kennungen der ausgeschlossenen Ausstattungen |
| 4 | ERR\_DUPLICATE\_SPECS | Die angegebenen Ausstattungen definieren Merkmale mehrfach, die nur einmalig vorkommen dürfen, z.B. Lenkrad | [<id1>, <id2>, ...] | Array von Ausstattungskennungen, die die duplizierte Fahrzeugeigenschafts-Position spezifizieren |
| 5 | ERR\_UNKNOWN\_ITEM | Die angegebenen Ausstattungskennungen existieren nicht oder sind für das Derivat nicht verfügbar | [<id1>, <id2>, ...] | Kennungen der unbekannten Ausstattungen |
| 6 | ERR\_MISSING\_INPUT | Der Parameter derivativeId wurde nicht angegeben oder es ist keine Farbe / kein Polster definiert, weder durch Parameter noch mittels Umfasst-Logik | [<pn1>, <pn2>, ...] | Array fehlender Parameternamen |
| 7 | ERR\_ILLEGAL\_SELECTION | Mehr als eine Position einer erforderlichen Auswahl / keine oder mehr als eine Position einer "Umfasst"-Auswahl wurde angegeben | [<id>] | Kennung der fehlerhaften Ausstattungen |
| 8 | ERR\_LOGIC | Es liegt ein Fehler in der logischen Definition einer Ausstattung vor | [<id1>, <id2>, ...] | [<type1>, <type2>, ...] | Kennungen der fehlerhaften Ausstattungen, oder Logiktypnamen |
| 9 | ERR\_NOT\_AN\_OPTION | Mindestens eine angegebene Ausstattung ist keine optionale Ausstattung | [<id1>, <id2>, ...] | Kennungen der fehlerhaften Ausstattungen |

Eine Beschreibung der Validierungslogik und Beispiele finden Sie im Anhang.
