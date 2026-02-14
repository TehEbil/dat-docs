---
title: "Mögliche Fehlercodes getSparePartsDetailsForDPN"
topic_id: "24839"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > PartsService > Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie > Mögliche Fehlercodes getSparePartsDetailsForDPN"
---

# Mögliche Fehlercodes getSparePartsDetailsForDPN

| Fehlercode | Fehlertext | Beschreibung |
| --- | --- | --- |
| Server.wrongValueCode | Error while parsing property "request"  Error while parsing property "restriction"  Typemismatch for property "manufacturer". Integer expected, but found "?" | Der Parameter "manufacturer" von restriction darf nicht "?" oder "null" beinhalten. Bitte korrigieren Sie Ihre Vorgabe |
| Server.wrongValueCode | Error while parsing property "request"  Error while parsing property "restriction"  Typemismatch for property "vehicleType". Integer expected, but found "?" | Der Parameter "vehicleType" von restriction darf nicht "?" oder "null" beinhalten. Bitte korrigieren Sie Ihre Vorgabe |
| Server.wrongValueCode | Error while parsing property "request"  Error while parsing property "restriction"  Typemismatch for property "baseModel". Integer expected, but found "?" | Der Parameter "baseModel" von restriction darf nicht "?" oder "null" beinhalten. Bitte korrigieren Sie Ihre Vorgabe |
| Server.CountryError | wrong language value | Tritt auf, wenn beim Parameter "language" ein ungültiger oder kein Wert eingetragen wird. Bitte korrigieren Sie Ihre Vorgabe |
| Server.LocaleError | wrong country indicator value | Tritt auf, wenn beim Parameter "datCountryIndicator" ein ungültiger oder kein Wert eingetragen wird. Bitte korrigieren Sie Ihre Vorgabe |
| Server.CountryError | wrong country value | Tritt auf, wenn beim Parameter "country " ein ungültiger oder kein Wert eingetragen wird. Bitte korrigieren Sie Ihre Vorgabe |
| Server.authorizationFailed | Server.authorizationFailed | Der Fehler kann eintreten, wenn falsche Autorisierungsdaten eingegeben wurden oder wenn der Token nicht mehr gültig ist. |
