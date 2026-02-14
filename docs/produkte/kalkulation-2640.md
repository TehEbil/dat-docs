---
title: "Kalkulation"
topic_id: "2640"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation"
---

# Kalkulation

Die Soap Schnittstelle der SilverDAT 3 PRO bietet zusätzlich die Funktionen des VehicleRepairService zum Verwalten von Kalkulationen und Reparaturkosten.

Übersicht der Kalkulationsfunktionen innerhalb SilverDAT 3 Pro und die dazugehörige Webservice zum Serviceaufruf:

|  |  |  |  |
| --- | --- | --- | --- |
| SilverDAT calculatePro Funktion | SilverDAT 3 Pro Funktion | myClaim Service | Hinweis |
| [calculateN](#showid/18882 "Reparaturkostenkalkulation ohne Speicherung ") | [calculateN](#showid/18896 "Reparaturkostenkalkulation ohne Speicherung ") | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |
| [calculateContract](#showid/18900 "(Nach-) Kalkulieren eines bestehenden Vorgangs") | [calculateContract](#showid/18905 "(Nach-) Kalkulieren eines bestehenden Vorgangs") | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |
| [exportDossierToDocument](#showid/2338 "Exportieren von Dokumenten") | nicht vorhanden |  |  |
| exportToDocument | nicht vorhanden |  |  |
| [getCalculationResultN](#showid/19752 "Abrufen eines Kalkulationsergebnisses") | nicht vorhanden |  |  |
| [getContract](#showid/1469 "Abrufen eines bestimmten Vorgangs") | getContract | [myClaimExternalService](#showid/2190 "Schnittstellenoperationen") | Neue Parameter |
| [getContractList](#showid/2417 "Abfrage der Vorgangsübersicht") | nicht vorhanden |  |  |
| [getContractPriceGenerations](#showid/2343 "Abruf aller vorhandenen Preisständen eines Vorgangs") | [getContractPriceGenerations](#showid/18651 "Abruf aller vorhandenen Preisständen eines Vorgangs") | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |
| [getDVNEquipments](#showid/2363 "Abruf von Ausstattungen zu DVN") | [getDVNEquipments](#showid/18654 "Abruf von Ausstattungen zu DVN") | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |
| [getAdditionalItems](#showid/22521 "Abrufen der Zusatzpositionen anhand des DAT €urope-Codes") | getAdditionalItems | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |
| [getFillingQuantities](#showid/22892 "Abrufen der Füllmengen anhand des DAT €urope-Codes") | [getFillingQuantities](#showid/22898 "Abrufen der Füllmengen anhand des DAT €urope-Codes") | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |
| [getInsurances](#showid/2333 "Abrufen von länderspezifischen Versicherungen") | [getInsurances](#showid/18657 "Abrufen von länderspezifischen Versicherungen") | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |
| [getLacquerTypeKeys](#showid/2345 "Abrufen von Lackartschlüsseln") | [getLacquerTypeKeys](#showid/18660 "Abrufen von Lackartschlüsseln") | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |
| [getLockedInfo](#showid/2347 "Abfrage des Bearbeitungsstatus/ -benutzer eines Vorgangs") | nicht vorhanden |  |  |
| [getMaintanceIntervals](#showid/2361 "Abruf von Wartungsintervallen: getMaintenanceIntervals") | [getMaintanceIntervals](#showid/18663 "Abruf von Wartungsintervallen: getMaintenanceIntervals") | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |
| [getSparePartsDetails](#showid/17159 "Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie") | [getSparePartsDetails](#showid/17314 "Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie") | [VehicleRepairService](#showid/2413 "VehicleRepairService") / PartsService |  |
| [getSparePartsDetailsByVIN](#showid/17163 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie") | [getSparePartsDetailsByVIN](#showid/17318 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie") | [VehicleRepairService](#showid/2413 "VehicleRepairService") / PartsService |  |
| [getSparePartsDetailsForDPN](#showid/17164 "Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie ") | [getSparePartsDetailsForDPN](#showid/17322 "Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie ") | [VehicleRepairService](#showid/2413 "VehicleRepairService") / PartsService |  |
| [getSparePartsDetailsForDPNByVIN](#showid/17165 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie ") | [getSparePartsDetailsForDPNByVIN](#showid/17326 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie ") | [VehicleRepairService](#showid/2413 "VehicleRepairService") / PartsService |  |
| [getTemplates](#showid/2349 "Abruf aller existierenden Druckvorlagen") | nicht vorhanden |  |  |
| [getVaildDATProcesses](#showid/2366 "Abfragen von DVNs anhand von DAT €uropa-Code, Bauzeit und AVs") | [getVaildDATProcesses](#showid/18666 "Abfragen von DVNs anhand von DAT €uropa-Code, Bauzeit und AVs") | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |
| [importDossier](#showid/1367 "Erstellen, Aktualisiern und Überschreiben eines Vorgangs") | [createOrUpdateContract](#showid/16529 "Erstellen eines neuen Auftrags mit Option zum Aktualisieren/Überschreiben")N | [myClaimExternalService](#showid/2190 "Schnittstellenoperationen") | Neue Parameter |
| listTemplates | nicht vorhanden |  |  |
| [setContractPriceGeneration](#showid/2351 "Änderung eines Preisstands eines Vorgangs") | [setContractPriceGeneration](#showid/18669 "Änderung eines Preisstands eines Vorgangs") | [VehicleRepairService](#showid/2413 "VehicleRepairService") |  |

Die spezifischen Schnittstellenfunktionen der SilverDAT 3 PRO zum Verwalten der Kalkulationen und ihre Beschreibungen rufen Sie über folgende URL's
auf:

WSDL

VehicleRepairService

[https://www.dat.de/myClaim/soap/v2/VehicleRepairService?wsdl](https://www.dat.de/myClaim/soap/v2/VehicleRepairService)

PartsService

[https://www.dat.de/myClaim/soap/v2/VehicleRepairService?wsdl](https://www.dat.de/myClaim/soap/v2/VehicleRepairService)

myClaimExternalService

<https://www.dat.de/myClaim/soap/v2/MyClaimExternalService?wsdl>

Serviceaufruf

VehicleRepairService

<https://www.dat.de/myClaim/soap/v2/VehicleRepairService>

PartsService

[https://www.dat.de/myClaim/soap/v2/PartsService](https://www.dat.de/myClaim/soap/v2/VehicleRepairService)

myClaimExternalService

[https://www.dat.de/myClaim/soap/v2/MyClaimExternalService](http://www.dat.de/myClaim/soap/v2/MyClaimExternalService)
