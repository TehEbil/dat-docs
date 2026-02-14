---
title: "Abruf von Ausstattungen zu DVN"
topic_id: "2363"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abruf von Ausstattungen zu DVN"
---

# Abruf von Ausstattungen zu DVN

Die Funktion getDVNEquipments() liefert entsprechende AVs für übergegebene DVNs, sofern auch der entsprechende DAT €uropa-Code und die Bauzeit übergeben werden.

Parameter

Übergeben muss ein DAT €uropa-Code und eine gültige Bauzeit, zusammen mit den entsprechenden DVNs. Durch den Parameter
"[locale](#showid/1352 "Element locale ")" lässt sich das Kalkulationsergebnis in der gewünschten Sprache abrufen.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| constructionTime | Integer, optional | Bauzeit nach DAT-Notation, 4stellig |
| datECode | String, Pflicht | Gültiger DAT €uropa-Code |
| datProcessIds | Integer[], Pflicht | DVN-Nummer, mehrfach Übergabe möglich |
| locale | Locale, optional | [Element locale](#showid/1352 "Element locale ") |

Rückgabe

Zurückgeliefert werden die Ausstattungen zur jeder übergebenen DVN.

| Name | Datentyp | Beschreibung | Kind-Elemente |
| --- | --- | --- | --- |
| dvnEquipmentsResult | DvnEquipmentsResult[] | Ergebnisse der DAT-interne Datenverarbeitungsnummer (DVN) | [datProcessId | equipments]    datProcessId (Integer): DAT-interne Datenverarbeitungsnummer (DVN)  equipments (Equipment): Austattungen mit Beschreibungen, die für diese DVN und das Fahrzeug relevant sind. |
