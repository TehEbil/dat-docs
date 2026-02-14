---
title: "Auflisten der Verrechnungssätze"
topic_id: "2613"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Auflisten von Informationen innerhalb einer Kundennummer > Auflisten der Verrechnungssätze"
---

# Auflisten der Verrechnungssätze

Mit der Funktion listInvoiceRates ist es möglich Verrechnungssätze innerhalb einer Kundennummer aufzulisten.

Über den boolschen Pflichtparameter isFiType werden dann nur Verrechnungssätze für die Fahrzeuginstandsetzung ausgegeben.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| isFiType | boolean | 1,0 | Verrechnungssatz Flag:  true= FI (Fahrzeuginstandsetzung)  false= Glas | X |
| isoCountryCode | String | DE | Ländercode in ISO Format | X |
| network | NetworkType |  | Name des Netzwerks |  |
| insuranceName | String | Allianz | Name der Versicherung |  |
| brandName | String | BMW, Audi | Name des Herstellers |  |
| partnerCustomerNumber | String |  | Kundennummer des Partners (nur für FI) |  |

Rückgabe

Liste der Verrechnungssätze im REP-DB Format
