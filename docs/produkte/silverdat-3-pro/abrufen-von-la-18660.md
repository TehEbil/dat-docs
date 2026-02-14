---
title: "Abrufen von Lackartschlüsseln"
topic_id: "18660"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abrufen von Lackartschlüsseln"
---

# Abrufen von Lackartschlüsseln

Die Funktion getLacquerTypeKeys() gibt eine Liste der Lackarten pro Lackmethode zurück, optional kann auch für Herstellerlack
(MANUFACTURER\_SPECIFIC) ein entsprechender Herstellercode übergeben werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| locale | Locale, optional |  | [Element locale](../../allgemein/dat-developers-gui/element-locale-1352.md) |
| mainType | Integer, optional |  | Fahrzeughaupttyp |
| manufacturer | Integer, optional |  | Hersteller |
| paintMethod | String, optional | EURO\_LACQUER (Lackiermethode=Eurolack) oder  MANUFACTURER\_SPECIFIC (Lackiermethode=Lack-Hersteller-System) | Die Lackiermethode kann mit einer der beiden Konstanten übergeben werden:  EURO\_LACQUER (Lackiermethode=Eurolack) oder  MANUFACTURER\_SPECIFIC (Lackiermethode=Lack-Hersteller-System) |
| vehicleType | Integer, optional |  | Fahrzeugart |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| gdvFlag | String |  |
| insuranceGroupId | String |  |
| insuranceName | String | Versicherungsname |
| insuranceNumber | String | Versicherungsnummer |
