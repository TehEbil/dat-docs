---
title: "Auflisten der Partner"
topic_id: "2569"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Auflisten von Informationen innerhalb einer Kundennummer > Auflisten der Partner"
---

# Auflisten der Partner

Über die Funktion listPartners wird eine Übersicht aller vorhandenen Partner innerhalb einer Kundennummer angezeigt.
Das Ergebnis kann über die optionalen Filter (PLZ, Rolle, Netztyp) weiter eingeschränkt
werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| postalCode | String |  | Postleitzahl des Partners |  |
| customerRole | String | INSURANCE, MANUFACTURER, EXPERT, REPAIRER | Rolle des Partners |  |
| networkType | String |  | Netzwerktyp des Partners |  |

Rückgabe

Liste aller vorhandenen Partner mit jeweils dessen Daten wie die Kundennummer, Identifikationsnummer,
ID, Rolle, Anschrift usw.
