---
title: "Abrufen von Lackartschlüsseln"
topic_id: "2345"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen von Lackartschlüsseln"
---

# Abrufen von Lackartschlüsseln

Die Funktion getLacquerTypeKeys gibt eine Liste der Lackarten pro Lackmethode zurück, optional kann auch für Herstellerlack
(MANUFACTURER\_SPECIFIC) ein entsprechender Herstellercode übergeben werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| locale | Locale, optional |  | [Element locale](../../../allgemein/dat-developers-guide/arbeiten-mit-den-web/element-locale-1352.md) |
| mainType | Integer, optional |  | Fahrzeughaupttyp |
| manufacturer | Integer, optional |  | Hersteller |
| paintMethod | String, optional | [EURO\_LACQUER |  MANUFACTURER\_SPECIFIC |  AZT | Die Lackiermethode kann mit einer dieser Konstanten übergeben werden:  EURO\_LACQUER (Lackiermethode=Eurolack) oder  MANUFACTURER\_SPECIFIC (Lackiermethode=Lack-Hersteller-System)  AZT (Lackiermethode=Allianz Zentrum für Technik) |
| vehicleType | Integer, optional |  | Fahrzeugart |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| lacquerTypes | [lacquerType](../datentypen/lacquertype-22518.md) [] | Enthält eine Liste der Lackarten pro Lackmethode |
