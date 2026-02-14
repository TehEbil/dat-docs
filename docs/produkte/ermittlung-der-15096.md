---
title: "Ermittlung der Ausstattungsmerkmale"
topic_id: "15096"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Ermittlung der Ausstattungsmerkmale"
---

# Ermittlung der Ausstattungsmerkmale

In unseren Anwendungen steht eine neue kostenpflichtige Schnittstellenfunktion zur
Ermittlung von herstellerübergreifenden Ausstattungsmerkmalen eines Fahrzeuges zur
Verfügung.

Beschreibung

Die Schnittstellenfunktion getEquipmentAttributes ermittelt die im Fahrzeug vorhandenen Eigenschaften (Attribute). Optional kann dabei
die Abfrage auf eine oder mehrere Baugruppen beschränkt werden, so wie für die Auswertung
die maximal mögliche Sonderausstattung für dieses Fahrzeug berücksichtigt werden.

Die Schnittstellenfunktion zur Ermittlung der Ausstattungsmerkmale ist ausschließlich
über REST verfügbar. Bei der Verwendung der Schnittstellenfunktion könnten zukünftig
Kosten entstehen (weitere Informationen erhalten Sie von unserem Vertrieb: [sales-support@dat.de](mailto:sales-support@dat.de "Mail an DAT Sales Support") oder [vertrieb@dat.de](mailto:vertrieb@dat.de "Mail an DAT Vertrieb")).

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| datECode | String | DAT €uropa-Code® | Gültiger DAT €uropa-Code® | X |
| container | String | Marktindex | Gültiger Marktindex | X |
| constructionTime | Integer | Bauzeit in DAT-Notation | Bauzeit | X |
| restriction | enumeration | ALL / REPAIR / APPRAISAL | alle / nur FI-Daten / nur FB-Daten durchsuchen | X |
| withEquipments | Boolean | true / false | Ausgabe der zugrundeliegenden Ausstattungen (datEquipmentId und description). DEFAULT: false |  |
| specialEquipmentId | Integer | 0-n DAT-AV-Codes | Liste der Sonderausstattungen |  |
| constructionGroup | enumeration | ALL / ENGINE / TRANSMISSION / AXLES\_CHASSIS / BODY\_EXTERIOR / INTERIOR / LIGHTING / AUDIO\_NAVI\_INFORMATION\_COMMUNICATION / FUNCTION\_SAFETY\_COMFORT / OTHER | Einschränkung auf eine oder mehrere Baugruppe(n) |  |
| coverage | enumeration | DEFAULT / WITH\_ALL\_SPECIAL\_EQUIPMENTS / NO\_STANDARD\_EQUIPMENT | Konfiguration der Menge der Ausstattungen die berücksichtigt werden: DEFAULT: Serienausstattung und übergebene Sonderausstattung WITH\_ALL\_SPECIAL\_EQUIPMENTS: zusätzliche Berücksichtigung der maximal möglichen Sonderausstattung NO\_STANDARD\_EQUIPMENT: keine Berücksichtigung der Serienausstattung |  |

Rückgabe

Es wird eine Struktur mit den Ermittelten Eigenschaften als JSON zurückgegeben. Darin
enthalten sind in erster Ebene die Baugruppen.

- Motor
- Kraftübertragung
- Achsen, Fahrwerk
- Karosserie, Exterieur
- Interieur
- Beleuchtung
- Audio, Navi, Information, Kommunikation
- Funktion, Sicherheit, Komfort
- Sonstiges

Nachfolgend wird die Ebene der Funktionsgruppen innerhalb der jeweiligen Baugruppe
ausgegeben. Die dritte Ebene sind die Funktionen, diese enthält die Merkmale und Ausprägungen.

1. Baugruppe (constructionGroup)
2. Funktionsgruppe (functionGroup)
3. Funktion (features)
4. Merkmale (property)

   - Name (propertyName)
   - Schlüssel (property)
   - Position (position) – Serienausstattung / Sonderausstattung
   - Wert (value) – optional
   - Genauigkeit (precision) – optional

Beispiel:

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>/getEquipmentAttributes

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | rest | VehicleIdentificationService |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | rest | VehicleIdentificationService |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | rest | VehicleIdentificationService |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | rest | VehicleIdentificationService |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | rest | VehicleIdentificationService |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | rest | VehicleIdentificationService |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | rest | VehicleIdentificationService |
