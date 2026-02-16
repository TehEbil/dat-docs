---
title: "Fahrzeugidentifikation in mehreren Sprachen"
topic_id: "2016"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation in mehreren Sprachen"
---

# Fahrzeugidentifikation in mehreren Sprachen

Beschreibung

Die Operation getVehicleTranslation vollzieht eine vollständige Fahrzeugidentifizierung mit dem DAT €uropa-Code®. Sie berücksichtigt Marktindex, Bauzeit und Sonderausstattungen wenn sie vorhanden
sind. Eine optionale Liste von Sprachen erzeugt die zusätzliche Ausgabe von Fahrzeugdaten
je angegebener Sprache. Es werden alle potenziellen Kombinationen aus DAT €uropa-Code® + Marktindex zuzüglich der Beschreibung aller Bestandteile in den gewünschten Sprachen
ermittelt.

Jede Fahrzeugidentifikation enthält die Datenschlüssel der DAT, Ausstattungsmerkmale,
Referenzfahrleistung und mehr. Der Benutzer kann das Fahrzeug mit diesen Angaben in
Fremdsystemen selbst auch dann finden, wenn die Fahrzeugidentifikation nicht eindeutig
ist. Er kann das Fahrzeug anhand der Datenschlüssel der DAT auswählen und eine individuelle
Bewertung oder Restwertprognose durchführen.

Der Benutzer bekommt bei dieser individuellen Fahrzeugauswahl eine Menge Informationen
über das Fahrzeug, ganz besonders über die verschiedenen Ausstattungsmerkmale. Er
muss mit der Fahrzeugidentifikation keine Bewertung oder Kalkulation durchführen.

Weitere Verwendungsmöglichkeit im Zusammenhang mit der VIN-Abfrage

Falls für ein Fahrzeug eine VIN-Abfrage mit der restriction APPRAISAL (Fahrzeugbewertung) durchgeführt wurde und im Nachgang dieses Fahrzeug für eine Schadenskalkulation
verwendet werden soll ist die restriction REPAIR erforderlich. Wenn nicht erneut eine VIN-Abfrage durchgeführt werden soll, kann über
getVehicleTranslation das Fahrzeug entsprechend transformiert werden. Die Vorgehensweise ist wie folgt.

Übernahme der Werte von DatECode, Container und ConstructionTime aus dem Ergebnis der VIN-Abfrage. Zusätzlich übergeben Sie als Sonderausstattungen
(specialEquipmentId) ebenfalls aus dem Ergebnis der VIN-Abfrage alle in VINResult enthaltenen AvNumberDat aus der Liste der VINEquipments. Als restriction verwenden Sie den für Ihren Fall gewünschten Wert. Bitte beachten Sie dabei, nicht
jedes Fahrzeug ist in den Daten der Fahrzeugbewertung und der Schadenskalkulation
verfügbar.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| datECode | String | DAT €uropa-Code® | Gültiger DAT €uropa-Code® | X |
| container | String | Marktindex | Gültiger Marktindex |  |
| constructionTime | Integer | DAT-Notation Bauzeit | Bauzeit | X |
| specialEquipmentId | Integer | DAT-AV-Code | Sonderausstattung (1-n) |  |
| language | String | Locale | Sprache und Land (1-n) |  |
| restriction | enumeration | ALL / REPAIR / APPRAISAL | alle / nur FI-Daten / nur FB-Daten durchsuchen | X |

Rückgabe

Es wird eine Liste möglicher Fahrzeugidentifikationen nach DAT im VXS-Format, Container
Vehicle, zurückgeliefert.

Bei Übergabe von DAT €uropa-Code® : bis auf weiteres in seltenen Fällen 1:N Fahrzeugidentifikationen, überwiegend exakt
eine Identifikation DAT €uropa-Code® + Container + Bauzeitangabe: exakt eine Identifikation.

Zusätzlich werden noch alle möglichen KBA-Nummern zurückgegeben.

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
