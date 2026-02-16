---
title: "Abrufen von länderspezifischen Versicherungen"
topic_id: "18657"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abrufen von länderspezifischen Versicherungen"
---

# Abrufen von länderspezifischen Versicherungen

Die Funktion getInsurances() liefert eine Liste der Versicherungen mit Versicherungsnummer und Versicherungsname
zurück.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| locale | Locale, optional |  | [Element locale](../../../allgemein/dat-developers-guide/arbeiten-mit-den-web/element-locale-1352.md) |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| gdvFlag | String | Der Gesamtverband der Deutschen Versicherungswirtschaft (Datenbank der Gemeinschaft der Autoversicherer) |
| insuranceGroupId | String | Versicherungsgruppen |
| insuranceName | String | Versicherungsname |
| insuranceNumber | String | Versicherungsnummer |
