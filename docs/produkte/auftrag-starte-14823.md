---
title: "Auftrag starten"
topic_id: "14823"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Neubewertung und Nachbewertung der Dossiers > Auftrag starten"
---

# Auftrag starten

Mit der Funktion startTask fassen Sie ein oder mehrere Dossiers zu einem Auftrag zusammen. Diese Dossiers werden
nach- oder neubewertet. Es muss entweder DossierList, DossierCSVList oder RevaluateAllFlag angegeben werden.

Parameter startTask

| Name | Datentyp | Beschreibung | Schreibweise | Default-Wert | Pflicht |
| --- | --- | --- | --- | --- | --- |
| DossierList | Integer [] Array | Eine Liste von Dossiers, die bewertet werden sollen. Enthält 0 bis n Positionen des Unterelements DossierId |  |  | bedingt\* |
| DossiersCsvList | String | Kommaseparierte Liste der DossierIds, die bewertet werden sollen | 123456, 654321 |  | bedingt\* |
| RevaluateAllFlag | Boolean | Wenn dieser Paramter den Wert true besitzt, werden alle existierenden Dossiers bewertet. | true false | false | bedingt\* |
| ValuationResultFlag | Boolean | Wenn dieser Paramter den Wert true besitzt, dann wird ein Dokumentenname ausgegeben. Mit der Methode getDocument kann man den Inhalt holen. | true false | false |  |
| GrossValue | Boolean | Wenn dieser Parameter den Wert true besitzt, dann enthält die Ergebnisdatei Bruttobeträge. Mit dem Wert false enthält die Ergebnisdatei Nettobeträge. | true false | false |  |
| ValuationType | String | Wenn dieser Parameter den Wert RESET\_AND\_VALUATE besitzt, dann wird der Auftrag neubewertet, ansonsten wird der Auftrag nachbewertet. | VALUATE, RESET\_AND\_VALUATE | VALUATE |  |
| Locale | Attribut | Für die englische Dokumentenausgabe in der Methode getDocument, muss der Parameter locale mit den folgenden Wert belegt werden <Locale country="GB" datCountryIndicator="GB" language="en"/> | Deutsche Ausgabe des Dokuments: <Locale country="DE" datCountryIndicator="DE" language="de"/> |  |  |

Elements DossierList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Integer | DossierId, die bewertet werden soll |  | bedingt\* |
