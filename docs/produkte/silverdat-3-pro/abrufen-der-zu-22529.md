---
title: "Abrufen der Zusatzpositionen anhand des DAT €urope-Codes"
topic_id: "22529"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abrufen der Zusatzpositionen anhand des DAT €urope-Codes"
---

# Abrufen der Zusatzpositionen anhand des DAT €urope-Codes

Die Funktion getAdditionalItems() dient dem Abrufen der Zusatzpositionen anhand des DAT €urope-Codes.

Parameter Request

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| locale | complexType, Locale | Landeseinstellung, Datenland und Spracheinstellung |
| datECode | String, Pflicht | Gültiger DAT €uropa-Code |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| AdditionalItems | [AdditionalItem []](../silverdat-calculat/additionalitem-22525.md) | Liste der Zusatzpositionen |
