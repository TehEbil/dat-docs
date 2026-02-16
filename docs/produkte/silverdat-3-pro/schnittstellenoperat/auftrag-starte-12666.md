---
title: "Auftrag starten"
topic_id: "12666"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Neubewertung und Nachbewertung der Dossiers > Auftrag starten"
---

# Auftrag starten

Mit der Funktion startTaskN fassen Sie ein oder mehrere Dossiers zu einem Auftrag zusammen. Diese Dossiers werden
nach- oder neubewertet. Es muss entweder dossierList, dossierCsvList, revaluateAllFlag oder einen der Parameter stateSoldFilter, stateOpenedFilter, stateStockFilter oder stateDisposedFilter angegeben werden.

Parameter startTaskN

| Name | Datentyp | Beschreibung | Schreibweise | Default-Wert | Pflicht |
| --- | --- | --- | --- | --- | --- |
| dossierList | Integer [ ] Array | Liste der DossierIds, die bewertet werden sollen. Enthält 0 bis n Positionen des Unterelements DossierId |  |  | bedingt\* |
| dossiersCsvList | String | Kommaseparierte Liste der DossierIds, die bewertet werden sollen | 123456,123457 |  | bedingt\* |
| revaluateAllFlag | Boolean | Wenn dieser Parameter den Wert true besitzt, werden alle existierenden Dossiers bewertet | true false | false |  |
| valuationResultFlag | Boolean | Wenn dieser Parameter den Wert true besitzt, dann wird der Parameter FileName im Response ausgegeben. Mit der Methode getDocument kann man das dazugehörige Auftragsdokument holen | true false | false | bedingt\* |
| valuationType | String | Wenn dieser Parameter den Wert RESET\_AND\_VALUATE besitzt, dann wird der Auftrag entsprechend der Funktion resetValuation2defaultN neubewertet, ansonsten wird der Auftrag nachbewertet | VALUATE, RESET\_AND\_VALUATE | VALUATE |  |
| stateSoldFilter | Boolean | Alle Dossiers, die im Zustand Verkauft sind, werden nachbewertet | true false |  | bedingt\* |
| stateOpenendFilter | Boolean | Alle Dossiers, die im Zustand Erfasst sind, werden nachbewertet | true false |  | bedingt\* |
| stateDisposedFilter | Boolean | Alle Dossiers, die im Zustand Disponiert sind, werden nachbewertet | true false |  | bedingt\* |
| stateStockFilter | Boolean | Alle Dossiers, die im Zustand Bestand sind, werden nachbewertet | true false |  | bedingt\* |
| locale | Attribut | Für die englische Dokumentenausgabe in der Methode getDocument, muss der Parameter locale mit den folgenden Wert belegt werden <locale country="GB" language="en"/> | Deutsche Ausgabe des Dokuments: <locale country="DE" language="de"/> | englisch |  |

Element DossierList

| Name | Datentyp | Beschreibung | Schreibweise | Default-Wert | Pflicht |
| --- | --- | --- | --- | --- | --- |
| DossierId | Integer | DossierId, die bewertet werden soll. Die Identifikationsnummer DossierId ist identisch mit der contractID von getValuationN |  |  | X |

bedingt\* = Einer dieser Parameter ist Pflicht. Siehe Beschreibung oben.
