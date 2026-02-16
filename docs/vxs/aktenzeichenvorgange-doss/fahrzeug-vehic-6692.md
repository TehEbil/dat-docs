---
title: "Fahrzeug (Vehicle)"
topic_id: "6692"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle)"
---

# Fahrzeug (Vehicle)

<Vehicle>-Elemente gibt es theoretisch an mehreren Stellen. Wichtig ist im Normalfall das
<Vehicle>-Element unter dem benötigten Element (z.B. Valuation oder RepairCalculation).

Beim Hersteller "Mercedes-Benz" und Fahrzeugart "Lastkraftwagen" bleiben bei Bauzeit
2017 und später die folgenden Felder des Objekts "Vehicle" leer:  
OriginalPriceInfo, OriginalPrice, OriginalPriceGross.

Felder

| Element | Typ | Beschreibung |
| --- | --- | --- |
| VehicleIdentNumber | string17 | Fahrzeugidentifikationsnummer (Fahrgestellnummer) |
| DatECode | string15 | DAT-€uropa-Code |
| KbaNumbersN | string Sequence | Rückgabe aller zugeordneten KBA |
| Container | string5 | Marktindex (Ergänzung zum DAT-€uropa-Code zur weiteren Differenzierung) |
| ConstructionYear | integer | Baujahr (Ausgabe nur bei manueller Eingabe) |
| ConstructionMonth | integer | Bau-Monat (nur Eingabe, alternativ zu ConstructionTime) |
| ConstructionTime | integer | Bauzeit in DAT-Verschlüsselung |
| ConstructionTimeFrom | integer | Bauzeit von (kann leer sein); nur Fahrzeugauswahl und SilverDAT valuateFinance |
| ConstructionTimeTo | integer | Bauzeit bis (kann leer sein); nur Fahrzeugauswahl und SilverDAT valuateFinance |
| InitialRegistration | date | Erstzulassungsdatum |
| MileageEstimated | integer | km-Stand geschätzt |
| MileageOdometer | integer | km-Stand abgelesen |
| MileageInMiles | integer | Laufleistung in Meilen |
| MileageType | string60 | Angabe zur Laufleistung mit folgendem möglichen Inhalt: "FromTacho" (abgelesen vom Tacho), "Estimated" (geschätzt), "Indicated" (angegeben). |
| OperatingHours | integer | Betriebsstunden |
| (Dat)ManufacturerName | string80 | Herstellername |
| SalesDescription | string40 | Verkaufsbezeichnung |
| (Dat)BaseModelName | string80 | Haupttypname |
| (Dat)SubModelName | string80 | Untertypname |
| (Dat)VehicleTypeNameN | string80 | Fahrzeugartname |
| (Dat)ContainerNameN | string | Name/Benennung des Container |
| DATECodeEquipment | equipSequence | [Ausstattungen zum Ersatzteil (EquipmentPositions)](repaircalculation/ausstattungen-1379.md) |
| VehicleType | string | Fahrzeugart |
| Manufacturer | integer | Hersteller-Schlüssel |
| BaseModel | integer | Haupttyp |
| AlternativeBaseModel | integer | alternativer Haupttyp im Falle eines unvollständigen FI-Haupttyps |
| SubModel | integer | Untertyp |
| AlternativeSubModel | integer | alternativer Untertyp im Falle eines unvollständigen FI-Haupttyps |
| MainTypeGroup | string | Haupttypgruppe |
| MainTypeGroupName | string | Name/Benennung der Haupttypgruppe |
| EngineNameManual | string80 | manuell eingegebene Benennung des Motors |
| BodyNameManual | string80 | manuell eingegebene Benennung der Karosserie |
| WheelbaseNameManual | string80 | manuell eingegebene Benennung des Radstands |
| PropulsionNameManual | string80 | manuell eingegebene Benennung der Antriebsart |
| DrivingCabNameManual | string80 | manuell eingegebene Benennung der Fahrerkabine |
| TonnageNameManual | string80 | manuell eingegebene Benennung der Tonnage |
| ConstructionNameManual | string80 | manuell eingegebene Benennung der Bauart |
| SuspensionNameManual | string80 | manuell eingegebene Benennung der Federungsart |
| AxleCountNameManual | string80 | manuell eingegebene Benennung der Anzahl Achsen |
| EquipmentLineNameManual | string80 | manuell eingegebene Benennung der Ausstattungslinie |
| GearboxNameManual | string80 | manuell eingegebenen Benennungen des Getriebes |
| IdentificationSource | string | Enthält die Kennung der Herkunft der Fahrzeugidentifikation. Mögliche Werte sind: VIN | KBA | DATECODE |
| Country | string | Datenland als ISO-Code (DE, FR, IT usw.) |
| CountryTarget | string3 | Datenland als ISO-Code (DE, FR, IT usw.) für das Land des Zielmarktes im Falle einer grenzüberschreitenden Situation |
| isDisengagedN | fieldBoolean | Kennzeichen für nicht bewertbares Fahrzeug (freies Aktenzeichen) |
| IsUniversalSubModel | fieldBoolean | für die Schnittstellenfunktionalität zur Auswahl der Sammeluntertypen (momentan nur für Variante A) |
| withoutDistinctionEquStandardSpecialN | fieldBoolean | Flag für "ohne Unterscheidung zwischen Serien- und Sonderausstattung" (nur relevant im Falle "freies Aktenzeichen") |
| (Dat)OriginalPrice | decimal | Netto Preis (nur für getVehicleIdentificationByVin mit restriction=APPRAISAL) |
| (Dat)OriginalPriceGross | decimal | Brutto Preis (nur für getVehicleIdentificationByVin mit restriction=APPRAISAL) |
| OriginalPriceInfo | complexType | Zusammenfassung der Informationen zum Neupreis des Fahrzeuges |
| PaintTypes | string Sequence | Liste der möglichen Lackarten. Die Lackartermittlung wird nur in Verbindung einer VIN-Abfrage durchgeführt. Der VIN-Server liefert in den meisten Fällen für die Außenfarben eine Lackart zurück. |
| ReleaseIndicator | string | Freigabekennzeichen; mögliche Werte: NONE, ECODE, REPAIR, APPRAISAL, ALL |
| TokenOfVinResult | string | Token aus dem Ergebnis der VIN-Abfrage (wird erstellt beim Export und analysiert beim Import) |
| IsConnectedCarSupported | fieldBoolean | Kennzeichen Unterstützung der Connected-Car-Daten |
| IsConnectedCarEligible | fieldBoolean | Kennzeichen Berechtigt für Connected-Car-Daten |
| IsConnectedCarDataDeliveryPush | fieldBoolean | Kennzeichen Senden (Push) von Connected-Car-Daten verfügbar |
| IsConnectedCarDataDeliveryPull | fieldBoolean | Kennzeichen Empfangen (Pull) von Connected-Car-Daten verfügbar |
| [VehicleDataItaly](fahrzeug-vehicle/vehicledataita-1395.md) | [VehicleDataItaly](fahrzeug-vehicle/vehicledataita-1395.md) | Fahrzeugdaten für CalculateItalia (nur für Italien) |
