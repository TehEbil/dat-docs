---
title: "Abrufen der Merkmalskataloge"
topic_id: "31066"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Abrufen der Merkmalskataloge"
---

# Abrufen der Merkmalskataloge

Für die Nutzung der Schnittstellenfunktion getEquipmentAttributes sind die zugrunde liegenden Merkmalskataloge der Ausstattungsmerkmale erforderlich.
Die statische Dokumentation der Merkmalskataloge im SilverDAT Schnittstellenkompendium
wird künftig nicht mehr benötigt.

Beschreibung

Die Schnittstellenfunktion getEquipmentAttributeValueLists stellt die Merkmalskataloge bereit. Der Markt wird durch den Parameter datCountryIndicator im Element locale bestimmt, während die Ausgabesprache über die Parameter country und language festgelegt wird. Optional kann die Abfrage auf eine oder mehrere spezifische Baugruppen
eingegrenzt werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| constructionGroup | enumeration | ALL / ENGINE / TRANSMISSION / AXLES\_CHASSIS / BODY\_EXTERIOR / INTERIOR / LIGHTING / AUDIO\_NAVI\_INFORMATION\_COMMUNICATION / FUNCTION\_SAFETY\_COMFORT / OTHER | Einschränkung auf eine oder mehrere Baugruppe(n) |  |

Rückgabe

Es wird eine strukturierte Übersicht der verfügbaren Ausstattungsmerkmale bereitgestellt,
die in der ersten Ebene die Baugruppen darstellt. Diese Baugruppen umfassen:

- Motor
- Kraftübertragung
- Achsen, Fahrwerk
- Karosserie, Exterieur
- Interieur
- Beleuchtung
- Audio, Navi, Information, Kommunikation
- Funktion, Sicherheit, Komfort
- Sonstiges

Im Folgenden werden die Funktionsgruppen innerhalb der jeweiligen Baugruppe dargestellt.
Die dritte Ebene umfasst die Funktionen, die die spezifischen Merkmale enthalten.

1. Baugruppe mit Beschreibung und Schlüssel (constructionGroup)
2. Funktionsgruppe mit Beschreibung und Schlüssel (functionGroup)
3. Funktion mit Beschreibung und Schlüssel (feature)
4. Merkmal mit Beschreibung und Schlüssel (property)

Die Beschreibungen variieren je nach gewählter Sprache. Für eine sprachunabhängige
Auswertung in Verbindung mit getEquipmentAttributes ist daher die Nutzung der Schlüssel erforderlich.

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
