---
title: "executeVehicleSelectionInteractive"
topic_id: "11424"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > interaktive Fahrzeugauswahl > executeVehicleSelectionInteractive"
---

# executeVehicleSelectionInteractive

Die Schnittstellenfunktion executeVehicleSelectionInteractive liefert zu gewählten Filterkriterien, die Anzahl der gefundenen Fahrzeuge und bei
entsprechend gewählten Filterkriterien eine oder mehrere Fahrzeuge mit DAT €uropa -Code® und Marktindex. Die vom Anwender getätigte Auswahl der Filterkriterien wird über
einen erneuten Schnittstellenaufruf dem System übermittelt. Das System ist zustandslos.
Die Ausgabe der Funktion ist direkt von den gewählten Eingabeparametern abhängig.
Es liefert als Ergebnis die mit den getätigten Filtereinstellungen noch möglichen
weiteren Filter sowie die gefundenen Fahrzeuge.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| locale | complex | Beispiel: "locale": { "country": "de", "datCountryIndicator": "de", "language": "de" } | Sprach- und Dateneinstellung. ISO 3166 ALPHA-2: country, ISO 639-1: language und datCountryIndicator | X |
| restriction | enumeration | APPRAISAL | Nur FB-Daten durchsuchen | X |
| allowedVehicleTypes | String | Eine oder mehrere Fahrzeugarten (1, 2, ...) | Möglichkeit zur Einschränkung auf bestimmte Fahrzeugarten |  |
| registrationDate | String | Datum (YYYY-MM-DD) | Einschränkung auf Fahrzeuge mit dieser Erstzulassung |  |
| withEquipmentMatrix | Boolean | true / false | Mit dem setzen dieser Option auf „true“ werden bei gefundenen Fahrzeugen die möglichen Ausstattungen (Serie- und Sonder-) als Matrix ausgegeben. |  |
| datECode | String | DAT €uropa-Code | Falls ein DAT €uropa-Code® bereits bekannt ist (15 oder 20 Zeichen). |  |
| datECodes | String | Ein oder mehrere DAT €uropa-Codes | Die möglichen Filter können mit einem oder mehreren DAT €uropa-Codes® (auch Fragmente) vorbelegt werden. |  |
| filter | String |  | Key/Value Listen mit den gewählten Filtereinstellungen für manufacturer, vehicleTypeSummarized, mainTypeGroupFb, structureType, structureTypeHgv, mainTypeForMotorcycles, subTypeForMotorcycles, fuelMethod, countOfDoors, driveType, constructionYearHgv, axleCount, tonnage, emissionClass, powerKw, constructionYear, engine, wheelbase, drivingCab, suspension, propulsion, gearType, countOfGears, gearbox, mainTypeFb, subType |  |

Rückgabe

Als Antwort wird ein JSON-String mit den unten aufgeführten Elementen geliefert, in
der keine überflüssigen Leerzeichen enthalten sind. Falls man die Ausgabe in einer
besser lesbaren Form möchte, also mit Leerzeichen und Zeilenumbrüchen, kann das gesteuert
werden durch Übergabe des Elements X-DAT-REST-BEAUTY: true im HTTP-Header.

| Name | Ebene 1 | Ebene 2 | Beschreibung |  |
| --- | --- | --- | --- | --- |
| count |  |  | Anzahl der gefundenen Fahrzeuge |  |
| filters |  |  | Mögliche Filtereinstellungen für manufacturer, vehicleTypeSummarized, mainTypeGroupFb, structureType, structureTypeHgv, mainTypeForMotorcycles, subTypeForMotorcycles, fuelMethod, countOfDoors, driveType, constructionYearHgv, axleCount, tonnage, emissionClass, powerKw, constructionYear, engine, wheelbase, drivingCab, suspension, propulsion, gearType, countOfGears, gearbox, mainTypeFb, subType. |  |
|  | key |  | Schlüssel |  |
|  | label |  | Text in der im Locale eingestellten Sprache |  |
|  | proposals |  | Mögliche Werte für den Schlüssel |  |
|  |  | k | Wert des Schlüssels |  |
|  |  | v | Bezeichnung des Schlüssels |  |
|  |  | a | Zusatzinformation zur Bezeichnung des Schlüssels, wird in den Fällen verwendet, in denen die Bezeichnungen nicht eindeutig sind. |  |
| vehicles |  |  | Gefundene Fahrzeuge. Diese sind in der Antwort enthalten, sobald die Anzahl gefundener Fahrzeuge kleiner oder gleich 30 ist. |  |
|  | vehicleTypeName |  | Fahrzeugart Bezeichnung |  |
|  | manufacturerName |  | Hersteller Bezeichnung |  |
|  | mainTypeName |  | Haupttyp Bezeichnung |  |
|  | subTypeName |  | Untertyp Bezeichnung |  |
|  | containerName |  | Container Bezeichnung |  |
|  | constructionTimeFrom |  | Bauzeit von |  |
|  | constructionTimeTo |  | Bauzeit bis |  |
|  | equipments |  | klassifizierende Ausstattungen |  |
|  | equipmentsSuper |  | übergeordnete Ausstattungen (z.B. Sondermodellpaket) |  |
|  | exFactoryPrice |  | Listenneupreis (netto, ohne Sonderausstattungen) |  |
|  | currency |  | Währung |  |
|  | ecode |  | DAT €uropa-Code® |  |
| equipmentMatrix |  |  | Matrix der Ausstattungen aller gefundenen Fahrzeuge |  |
|  | av |  | DAT–Ausstattungsnummer |  |
|  | name |  | Bezeichnung |  |
|  | available |  | Verfügbar für jeden DAT €uropa-Code® |  |
|  |  | DAT €uropa-Code® | „X“ = Sonderausstattung oder „S“ = Serienausstattung |  |

Serviceaufruf

URL : https://www.datgroup.com/DATECodeSelection/rest/VehicleSelectionService

Protokoll : REST

Funktion : executeVehicleSelectionInteractive

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Verwendung in den DAT Produkten

| SilverDAT Anwendung | URL |
| --- | --- |
| SilverDAT 3 PRO | https://www.datgroup.com/myClaim/rest/VehicleSelectionService |
| [SilverDAT 3 valuateFinance](#showid/1520 "SilverDAT 3 valuateFinance") | https://www.datgroup.com/FinanceLine/rest/VehicleSelectionService |
| SilverDAT 3 valuateExpert/  Partner/Pluspartner | https://www.datgroup.com/valuateNG/rest/VehicleSelectionService |
| DAT €uropa-Code® Fahrzeugauswahl | https://www.datgroup.com/DATEcodeSelection/rest/VehicleSelectionService |
