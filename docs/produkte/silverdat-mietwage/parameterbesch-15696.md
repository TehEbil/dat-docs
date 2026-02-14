---
title: "Parameterbeschreibung für exportRentalOffers"
topic_id: "15696"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenprotokoll erstellen > Parameterbeschreibung für exportRentalOffers"
---

# Parameterbeschreibung für exportRentalOffers

Mit der Funktion exportRentalOffers erzeugen Sie ein Ausdruck mit den angegeben Fahrzeugdaten. Weitere Daten wie Nutzungsausfalldaten,
Mietwagenklasse und Mietdauer können ebenfalls angegeben werden.

Parameter

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Locale | Locale | Beispiel: <Locale country="DE"  datCountryIndicator="DE" language="de"/> |  | X |
| exportProduct | String | Bezeichnung des Reports | RENTAL\_PRICES\_FOR\_REPAIR\_COSTS | X |
| DATECode | String | DAT €uropa-Code® | 24-stellig Mindestens eine der beiden Angaben DATECode oder VIN muss angegeben sein. Sind beide Angaben vorhanden wird der Wert von DATECode zur Fahrzeugidentifikation verwendet. | bedingt |
| rentalCarClass  Die DAT hat sämtliche Fahrzeuge im DAT-Fahrzeugbestand in 11 Mietwagenklassen eingestuft. Die Mietwagenklassen wurde dabei definiert durch Fahrzeugkosten und Motorisierung.  Die Mietwagenklassen gehen bei PKW von 1 – 11, bei Transportern von 21 – 31, wobei in der Praxis bei Transportern aufgrund der Preisstrukturen die Klassen 24 – 31 Verwendung finden.  Für jedes Modelljahr, beginnend mit dem Jahr 2003, werden die Klassen anhand der aktuellen Fahrzeugangebote, Preise und Ausstattungskriterien ergänzt, überarbeitet und ggf. angepasst.  Durch die modelljahrbezogene Datenerhebung können die Kosten und Angebotssituationen auch rückblickend ab dem Jahr 2013 ermittelt werden. | Integer | Mietwagenklasse | weitere Infos siehe Popup-Fenster |  |
| VIN | String | Fahrzeug-Identifizierungsnummer | 17stellig, alphanumerisch Mindestens eine der beiden Angaben DATECode oder VIN muss angegeben sein. | bedingt |
| firstRegistration  Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex darf nicht größer als 1 Jahr sein. In der Fahrzeugbewertung kann sonst kein Wert ermittelt werden. | Date | Erstzulassung | YYYY-MM-DD  weitere Infos siehe Popup-Fenster | X |
| mileage | Integer | Laufleistung |  |  |
| beginnigOfRental | Date | Anfangsdatum der Vermietung | Datum, [firstRegistration+50 Jahre] YYYY-MM-DD |  |
| endOfRental | Date | Enddatum der Vermietung | Datum, [firstRegistration+50 Jahre] YYYY-MM-DD |  |
| postalCode | String | Postleitzahl für die Suche im entsprechenden Umkreis |  | X |
| duration | Integer | Leihdauer in Tagen. Wenn der Mietbeginn und das Mietende angegeben wurden, müssen diese Werte mit der Leihdauer übereinstimmen. | numerisch [1-30] |  |
| radius | Integer | Radius für die Suche im entsprechenden Umkreis | numerisch [1-50] |  |
| priceType | String | Preistyp | GROSS, NET |  |
| fileReference | String | Aktenzeichen |  |  |
| damageNumber | String | Schadensnummer |  |  |
| specificConditions | Boolean | Auswahl der Mietoption oder Miettarif | true= detaillierte Kostenrechnung auf Basis spezifischer Preislisten. Mietoptionen können für die Berechnung der Mete gesetzt werden gesetzt werden  false =Darstellung der Einzelbeträge ohne Summenbildung. Reiner Miettarif ohne Berücksichtigung von Mietoptionen. |  |
| deliveryInTown | Boolean | Zustellung/Abholung Mietfahrzeug innerorts pauschal | true, false |  |
| deliveryOutOfTown | Boolean | Zustellung/Abholung Mietfahrzeug außerorts pauschal | true, false |  |
| emergencyFee | Boolean | Gebühr Notdienst/ außerhalb Öffnungszeiten | true, false |  |
| oneWayRental | Boolean | Einwegmiete | true, false |  |
| deductibleOf0 | Boolean | SB-Reduzierung auf 0 € | true, false |  |
| deductibleOf100 | Boolean | SB-Reduzierung auf 100 € | true, false |  |
| deductibleOf150 | Boolean | SB-Reduzierung auf 150 € | true, false |  |
| deductibleOf300 | Boolean | SB-Reduzierung auf 300 € | true, false |  |
| deductibleOf450 | Boolean | SB-Reduzierung auf 450 € | true, false |  |
| additionalDriver | Boolean | Gebühr zusätzliche Fahrer | true, false |  |
| driverUnder25 | Boolean | Fahrer unter 25 Jahren | true, false |  |
| winterTire | Boolean | Winterreifengebühr | true, false |  |
| navigationDevice | Boolean | Navigationsgerät | true, false |  |
| trailerHitch | Boolean | Anhängerkupplung | true, false |  |
| snowChains | Boolean | Schneeketten | true, false |  |
| roofRack | Boolean | Dachgepäckträger | true, false |  |
| drivingSchoolEquipment | Boolean | Fahrschulausrüstung | true, false |  |
| withoutAdvancedFinancing | Boolean | Tarife ohne Vorfinanzierung durch Mieter sowie ohne Kaution | true, false |  |
| openEndRentalPeriod | Boolean | Tarife mit offenem Mietende | true, false |  |
| minimumAdvanceBookingPeriod | Boolean | Tarife ohne Vorbuchungsfrist | true, false |  |
| withoutDriverMinimumAge | Boolean | Tarife ohne Mindestalter | true, false |  |
