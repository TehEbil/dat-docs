---
title: "Hole Dokumentenergebnis eines Auftrags"
topic_id: "12682"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Neubewertung und Nachbewertung der Dossiers > Hole Dokumentenergebnis eines Auftrags"
---

# Hole Dokumentenergebnis eines Auftrags

Mit der Funktion getDocument holen Sie die Ergebnisdatei des abgeschlossenen Auftrags.

Parameter getDocument

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| TaskId | Integer | Auftragsnummer |  | X |
| FileName | String | Dokumentenname mit Formatangabe CSV. Diesen Wert bekommt man von der Methode startTaskNResponse, getTaskNResponse oder getAllTaskResponse. Eine CSV-Datei beinhaltet derzeit die Ergebnisse von maximal 15 Vorgängen. | \*.csv Format; max. 50 Zeichen zulässig | X |
