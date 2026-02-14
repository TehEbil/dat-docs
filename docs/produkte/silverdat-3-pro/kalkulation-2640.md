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
| [calculateN](../silverdat-calculat/reparaturkoste-18882.md) | [calculateN](reparaturkoste-18896.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |
| [calculateContract](../silverdat-calculat/nach-kalkulier-18900.md) | [calculateContract](nach-kalkulier-18905.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |
| [exportDossierToDocument](../silverdat-calculat/exportieren-vo-2338.md) | nicht vorhanden |  |  |
| exportToDocument | nicht vorhanden |  |  |
| [getCalculationResultN](../silverdat-calculat/abrufen-eines-19752.md) | nicht vorhanden |  |  |
| [getContract](../silverdat-calculat/abrufen-eines-1469.md) | getContract | [myClaimExternalService](../silverdat-3-valuat/schnittstellen-2190.md) | Neue Parameter |
| [getContractList](../silverdat-calculat/request-getdvn-2417.md) | nicht vorhanden |  |  |
| [getContractPriceGenerations](../silverdat-calculat/abruf-aller-vo-2343.md) | [getContractPriceGenerations](abruf-aller-vo-18651.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |
| [getDVNEquipments](../silverdat-calculat/abruf-von-auss-2363.md) | [getDVNEquipments](abruf-von-auss-18654.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |
| getAdditionalItems | getAdditionalItems | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |
| [getFillingQuantities](../silverdat-calculat/abrufen-der-fu-22892.md) | [getFillingQuantities](abrufen-der-fu-22898.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |
| [getInsurances](../silverdat-calculat/abrufen-von-la-2333.md) | [getInsurances](abrufen-von-la-18657.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |
| [getLacquerTypeKeys](../silverdat-calculat/abrufen-von-la-2345.md) | [getLacquerTypeKeys](abrufen-von-la-18660.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |
| [getLockedInfo](../silverdat-calculat/abfrage-des-be-2347.md) | nicht vorhanden |  |  |
| [getMaintanceIntervals](../silverdat-calculat/abruf-von-wart-2361.md) | [getMaintanceIntervals](abruf-von-wart-18663.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |
| [getSparePartsDetails](../silverdat-calculat/ermittlung-von-17159.md) | [getSparePartsDetails](ermittlung-von-17314.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) / PartsService |  |
| [getSparePartsDetailsByVIN](../silverdat-calculat/ermittlung-von-17163.md) | [getSparePartsDetailsByVIN](ermittlung-von-17318.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) / PartsService |  |
| [getSparePartsDetailsForDPN](../silverdat-calculat/ermittlung-der-17164.md) | [getSparePartsDetailsForDPN](ermittlung-der-17322.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) / PartsService |  |
| [getSparePartsDetailsForDPNByVIN](../silverdat-calculat/ermittlung-von-17165.md) | [getSparePartsDetailsForDPNByVIN](ermittlung-von-17326.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) / PartsService |  |
| [getTemplates](../silverdat-calculat/abruf-aller-ex-2349.md) | nicht vorhanden |  |  |
| [getVaildDATProcesses](../silverdat-calculat/abfragen-von-d-2366.md) | [getVaildDATProcesses](abfragen-von-d-18666.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |
| [importDossier](../silverdat-calculat/erstellen-aktu-1367.md) | [createOrUpdateContract](../silverdat3-myclaim/erstellen-eine-16529.md)N | [myClaimExternalService](../silverdat-3-valuat/schnittstellen-2190.md) | Neue Parameter |
| listTemplates | nicht vorhanden |  |  |
| [setContractPriceGeneration](../silverdat-calculat/anderung-eines-2351.md) | [setContractPriceGeneration](anderung-eines-18669.md) | [VehicleRepairService](../silverdat-calculat/vehiclerepairs-2413.md) |  |

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
