---
title: "Abrufen der Füllmengen anhand des DAT €urope-Codes"
topic_id: "22892"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen der Füllmengen anhand des DAT €urope-Codes"
---

# Abrufen der Füllmengen anhand des DAT €urope-Codes

Die Funktion getFillingQuantities() dient dem Abrufen der Füllmengen anhand des DAT €uropa-Code®.

Parameter Request

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| locale | complexType, Locale | Landeseinstellung, Datenland und Spracheinstellung |
| datECode | String, Pflicht | Gültiger DAT €uropa-Code® |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| FillingQuantities | complexType, Fluid[] | Liste der Füllmengen |
