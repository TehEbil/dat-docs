---
title: "Fahrzeugidentifikation anhand VIN (VIN-Abfrage)"
topic_id: "1798"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand VIN (VIN-Abfrage)"
---

# Fahrzeugidentifikation anhand VIN (VIN-Abfrage)

Die Funktion getVehicleIdentificationByVin liefert anhand der Vehicle Identification Number (VIN) alle DAT €uropa-Code® , (DAT) Containers und AV zuzügl. Farb-/Polsterangaben. Aufgrund der Masse der Informationen
erfolgt die Speicherung im VXS-Format.

Diese Operation führt eine vollständige Fahrzeugidentifizierung anhand der VIN durch.

Jedes Mal, wenn die VIN als Schlüssel benutzt wird, unerheblich, ob zur Fahrzeugidentifizierung
oder zur -bewertung, ist dies kostenpflichtig! Insbesondere ist dies auch der Fall,
wenn die VIN-Abfrage, nur die [Datenkarte](#showid/11682 "ECode not found  - Datenkarte") liefert (<faultcode>dat:dat:Server.valueNotFound). Weitere Informationen können Sie dann aus dem Element <faultstring> innerhalb <additionalInformation> entnehmen.  
Zusätzlich für den Hersteller BMW/MINI VIN gültig: Bei einer falschen Eingabe oder
bei einer Abfrage bei der kein Treffer erzielt wird, erfolgt die Rückmeldung "dat:dat:Server.valueNotFound"
zusammen mit einer leeren Datenkarte. Bitte beachten Sie, dass auch für diese Rückmeldung
Gebühren anfallen.

Die Funktion dient zur Identifizierung eines Fahrzeuges anhand Fahrzeugidentifikationsnummer
und liefert für eine VIN eine Liste mit Elementen des folgenden Umfangs:

- DAT €uropa-Code®
- Fahrzeugartbenennung
- Herstellerbenennung
- Haupttypbenennung
- Untertypbenennung
- Marktindex
- Bauzeit
- Bauzeit von - bis
- Preislisten-Bauzeit (optional)
- Liste der Serienausstattungen
- Liste der Sonderausstattungen
- Herstellertexte der Ausstattungen (optional)
- Liste der nicht zuordenbaren Ausstattungen gemeldet vom VIN-Hersteller
- Fahrzeugneupreis
- Alle möglichen KBA

Für die Abfrage der folgenden Hersteller über VIN gelten besondere Bedingungen:

- Renault / Dacia  
  Keine Ausgabe der originalen Ausstattungscodes- und Texte, sowie der Herstellerbauzeit.
- Fiat (einschl. Abarth, Alfa Romeo und Lancia)  
  Keine Ausgabe der originalen Ausstattungscodes.

Um die zusätzlichen Nutzungsinformationen zu klären und die erweiterte Schnittstellenfunktion
nutzen zu können, nehmen Sie bitte Verbindung zum Vertrieb der DAT über [sales-support@dat.de](mailto:sales-support@dat.de "Mail an DAT Sales Support") oder [vertrieb@dat.de](mailto:vertrieb@dat.de "Mail an DAT Vertrieb") auf. Außerdem erhalten Sie über diese Adressen auch den Passwortschlüssel, den Sie
als zusätzlichen Parameter benötigen.

Ausstattungen

Die zurückgelieferten Ausstattungen werden nach "Serie" und "Sonder" unterschieden.
Des Weiteren werden pro Ausstattung folgende Daten geliefert:

- DAT AV-Nummer (falls verfügbar)
- Hersteller Code (falls verfügbar)
- AV-Benennung
- AV-Gruppe (falls verfügbar)
- AV-Neupreis brutto gerundet auf ganze Euro

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| vin | String | Vehicle Identification Number | Gültige VIN-Nr. | X |
| coverage | enumeration | ALL / WITH\_MANUFACTURER\_TEXTS /WITH\_PRICE\_LIST\_TIME | Optional kann über den Parameter coverage die zusätzliche Ausgabe der Herstellertexte und/oder der Preislisten-Bauzeit gesteuert werden. |  |
| marketResearch | enumeration | USE\_DAT\_COUNTRY\_INDICATOR / CROSSBORDER | Legt den Marktplatz fest in dem die VIN-Abfrage durchgeführt werden soll. Wird beim Aufruf CROSSBORDER mitgegeben, dann erhält man, falls die VIN-Abfrage zu einem grenzübergreifenden Fall führt, ein Cross-Border-Ergebnis: Das heißt, man erhält die Dossier-Objekte des Originallandes plus die Dossier-Objekte des Ziellandes. |  |
| constructionTime | integer | 0-9999 | Bauzeit in DAT-Notation; die Übergabe ist nur in Verbindung mit den Herstellern Renault und Dacia möglich. Wird er bei anderen Herstellern übergeben, wird er ignoriert. |  |
| restriction | enumeration | ALL / REPAIR / APPRAISAL | keine Einschränkung / nur FI-Daten durchsuchen / nur FB-Daten durchsuchen | x |

Bei der Verwendung des Parameters marketResearch mit dem Wert CROSSBORDER muss zur Weiterverarbeitung der Daten des Ziellandes eine Lizenz für dieses Land
vorhanden sein.

Rückgabe

Es wird eine Liste möglicher Fahrzeugidentifikationen nach DAT im VXS-Format, beginnend
mit Element Dossier, zurückgeliefert. Zusätzlich werden noch alle möglichen KBA-Nummern zurückgegeben.

Im Falle eines nicht eindeutigen Ergebnisses aus einer VIN-Abfrage kann das Element
VinAccuracy bei der Entscheidung helfen, welches der gefundenen Fahrzeuge das richtige ist. Die
möglichen Werte sind 0 und 1, die 0 steht für den Treffer mit der größten Wahrscheinlichkeit.
Siehe beispielsweise Test-VIN WF0DATTESTSTUB003.

Im Element Vehicle befindet sich das Element VINResult, darin sind die Informationen vom Hersteller enthalten. Unter anderem Farbinformationen
mit dem Schlüssel ColorID. Dieser hat folgende Bedeutung:

- PF - Polster Farbe
- PM - Polster Material
- A1 - Außenfarbe 1 (Farbcode)
- A2 - Außenfarbe 2 (Farbcode)
- L1 - Lacknummer Außenfarbe 1 (derzeit nur für VAG-Gruppe)
- L2 - Lacknummer Außenfarbe 2 (derzeit nur für VAG-Gruppe)
- I1 - Innenfarbe 1
- ...
- In - Innenfarbe n

Wenn die Fahrzeugfarbe einer Standardfarbe zugeordnet werden kann, wird dieses im
Element StandardColor ausgegeben. Hierfür gilt folgender Wertebereich:

- 0 - weiß
- 1 - gelb/beige
- 2 - orange
- 3 - rot
- 4 - violett
- 5 - blau
- 6 - grün
- 7 - silber/grau
- 8 - braun
- 9 - schwarz

WSDL

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>?wsdl

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | services | VehicleIdentificationService |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | services | VehicleIdentificationService |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | services | VehicleIdentificationService |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | soap | VehicleIdentificationService |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | soap | VehicleIdentificationService |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | soap/v2 | VehicleIdentificationService |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | soap/v2 | VehicleIdentificationService |
