---
title: "Beschreibung getLossOfUseDatabyDATECodeResponse"
topic_id: "14960"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Nutzungsausfalldaten anhand DAT €uropa-Code® ermitteln > Beschreibung getLossOfUseDatabyDATECodeResponse"
---

# Beschreibung getLossOfUseDatabyDATECodeResponse

Elemente getLossOfUseDatabyDATECodeResponse

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| RentalVehicleResponse | rentalVehicleResponse | enthält Unterelemente mit Nutzungsausfalldaten |  |

Elemente RentalVehicleResponse

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| contingencyCostsPerDay | Decimal | Vorhaltekosten am Tag |  |
| lossOfUseClass | String | Nutzungsausfallklasse | A,B,C,D,E,F,G,H,J,K,L |
| lossOfUseClassExcVehAge | String | Nutzungsausfallklasse- ohne Berücksichtigung der Fahrzeugalters | A,B,C,D,E,F,G,H,J,K,L |
| lossOfUsePerDay | Decimal | Nutzungsausfallkosten am Tag |  |

Nutzungsausfallklasse

Das Fahrzeugalter ist dahingehend zu berücksichtigten, dass ab einem Alter von 5 Jahren
das Fahrzeug eine Gruppe niedriger eingestuft wird. Ab 10 Jahren wird die Einstufung
2 Klassen niedriger vorgenommen. Niedrigste Klasse ist die Klasse A.
