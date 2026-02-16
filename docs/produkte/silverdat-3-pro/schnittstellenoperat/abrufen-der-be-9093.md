---
title: "Abrufen der Bewertungsausdrucke"
topic_id: "9093"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Abrufen der Bewertungsausdrucke"
---

# Abrufen der Bewertungsausdrucke

Zum Abrufen der Ausdrucke der Bewertung verwenden Sie die Basisfunktion getPrintReport. Sie finden die Beschreibung der Basisfunktion getPrintReport im Kapitel [Abrufen einer Druckvorlage](../../silverdat3-myclaim/schnittstellenoperat/abrufen-eines-2609.md).

Mindestvorraussetzungen zum Generieren der Druckprodukte der Bewertung:

- Für alle Druckprodukte der Bewertung benötigen Sie die Auftrags ID contractId. Die Auftrags ID contractId entspricht der DossierId.
- Für alle Druckprodukte der Bewertung benötigen Sie einen zusätzlichen Identifier reportIdentification. Sie finden den Identifier in der nachfolgenden Tabelle: "Übersicht der Reports".
- Für alle Druckprodukte der Bewertung muss der entsprechende Vorgang eine vollständige
  Fahrzeugidentifikation beinhalten.

Je nach Druckprodukt werden eventuell weitere Angaben im Vorgang benötigt, siehe Tabelle
"Übersicht der Reports".

Übersicht der Reports

| Reportname | reportIdentification | Vorrausetzungen | | | | |
| --- | --- | --- | --- | --- | --- | --- |
|  |  | Bewertung | Einkaufsangebot | Ankauf | Verkaufsangebot | Verkauf |
| Gebrauchtfahrzeugbewertung Einkauf | UsedVehicleEvaluation\_purchase | X |  |  |  |  |
| Gebrauchtfahrzeugbewertung Verkauf | UsedVehicleEvaluation\_sales | X |  |  |  |  |
| Protokoll Gebrauchtfahrzeugbewertung | EvaluationProtocol | X |  |  |  |  |
| Checkliste Sonderausstattung | ChecklisteSonderausstattung | X |  |  |  |  |
| Checkliste zur Gebrauchtfahrzeugbewertung | ChecklisteZurGebrauchtfahrzeugbewertung | X |  |  |  |  |
| Einzelnachweis Differenzbesteuerung | EinzelnachweisDifferenzbesteuerung | X |  |  |  |  |
| Preisschild Barzahlung | PreisschildBarzahlung | X |  |  |  |  |
| Preisschild mit Bild | PreisschildmitBild | X |  |  |  |  |
| Preisschild Finanzierung | PreisschildFinanzierung | X |  |  |  |  |
| Preisschild Freitext | PreisschildFreitext | X |  |  |  |  |
| Preisschild Leasing | PreisschildLeasing | X |  |  |  |  |
| Fahrzeugdaten | Fahrzeugdaten | X |  |  |  |  |
| Ankaufsangebot | Ankaufsangebot | X | X |  |  |  |
| Ankaufsvertrag | Ankaufsvertrag | X |  | X |  |  |
| Verkaufsangebot | Verkaufsangebot | X |  |  | X |  |
| Verbindliche Bestellung Gebrauchtwagen | VerbindlicheBestellungGebrauchtwagen | X |  |  |  | X |
| Verkaeuferinformation | Verkaeuferinformation | X |  |  |  | X |
| Vorkalkulation | Vorkalkulation | X |  |  |  | X |
| Zwischenkalkulation | Zwischenkalkulation | X |  |  |  | X |
| Nachkalkulation | Nachkalkulation | X |  |  |  | X |
| Vorvertragliche Information | VorvertraglicheInformation | X |  |  |  | X |

Zusatzoptionen

Für die Ausdrucke Gebrauchtfahrzeugbewertung Einkauf, Gebrauchtfahrzeugbewertung Verkauf
und Protokoll Gebrauchtfahrzeugbewertung können zusätzlich im Eltern-Element attributes die nachfolgend beschriebenen Optionen gesetzt werden.

Übersicht der attributes Kind-Elemente

| Parameter | Datentyp | Beschreibung der Option |
| --- | --- | --- |
| isNetto | Booelean | Netto |
| isWithNewPrices | Booelean | inklusive Listenneupreise |
| isWithEquipment | Booelean | inklusive Ausstattungsliste |

attributes Kind-Elemente sind nur zulässig für folgende Bewertungen:

| Parameter | Gebrauchtfahrzeugbewertung Einkauf | Gebrauchtfahrzeugbewertung Verkauf | Protokoll Gebrauchtfahrzeugbewertung |
| --- | --- | --- | --- |
| isNetto | X | X | X |
| isWithNewPrices | X | X | X |
| isWithEquipment | X | X | X |

Das zugehöriges Beispiel für den Request finden sie unter [Abrufen einer Druckvorlage](../../silverdat3-myclaim/schnittstellenoperat/abrufen-eines-2609.md).
