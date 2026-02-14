---
title: "Änderungsnachweis"
topic_id: "2329"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Änderungsnachweis"
---

# Änderungsnachweis

Mit der jeweils aktuellsten Fassung verlieren alle früheren Versionen ihre Gültigkeit.

| Version | Datum | Änderung |
| --- | --- | --- |
| 5.5 | 02.09.2025 | Neue Werte maintenanceSchedule, withoutInsuranceData, withoutOwnerData, withoutDriverData, withoutGarageData, withoutOpponentData, withoutEquipments und withoutRepairCostExpansion im Parameter printProduct in der Request der Funktion [exportDossierToDocument()](exportieren-vo-2338.md).  Neuer Parameter finisNumber in der Request der Funktionen [getSparePartsDetails()](../silverdat-3-pro/ermittlung-von-17314.md),  [getSparePartsDetailsByVIN](../silverdat-3-pro/ermittlung-von-17318.md)(), [getSparePartsDetailsForDPN()](../silverdat-3-pro/ermittlung-der-17322.md) und [getSparePartsDetailsForDPNByVIN()](../silverdat-3-pro/ermittlung-von-17326.md).  Neues Attribut finisNumber im Element [SparePartsInformation.](sparepartsinfo-17192.md) |
| 5.4 | 12.03.2025 | Neues Attribut damageSegmentNumber in der Request der Funtkion [exportDossierToDocument()](exportieren-vo-2338.md) |
| 5.3 | 15.10.2024 | Neue Funktion [listAttachments()](auflisten-von-26391.md) in [VehicleRepairService](https://www.dat.de/myClaim/soap/v2/VehicleRepairService) |
| 5.2 | 16.08.2024 | Neue Funktion [manageAttachments()](hochladen-uber-26088.md) in [VehicleRepairService](https://www.dat.de/myClaim/soap/v2/VehicleRepairService) |
| 5.1 | 26.04.2024 | Neue Eingabeparameter hideContractCreation, FasttrackWorkflow für die Integration der SilverDAT calculatePro/calculateExpert Oberfläche siehe [Aufbereitung der Eingabeparameter](aufbereitung-d-2393.md) |
| 5.0 | 26.04.2024 | Neuer Wert für das Attribut crud "OVERWRITE\_KEEP\_ATTACHMENTS" in der Funktion [importDossier()](erstellen-aktu-1367.md) |
| 4.9 | 17.01.2024 | Neue Funktion [getFillingQuantities()](abrufen-der-fu-22892.md) in [VehicleRepairService](vehiclerepairs-2413.md)  Neuer Wert für das Attribut coverage in der Funktion getValidDATProcesses()  Neue Elemente in der Response der Funktionen getSparePartsDetails() und getSparePartsDetailsByVIN()  Neues Element Hint in der Response der Funktion getMaintenanceIntervals() |
| 4.8 | 10.10.2023 | Neue Funktion getAdditionalItems() in [VehicleRepairService](vehiclerepairs-2413.md)  Neues Attribut automaticVinRequest in der Funktion [importDossier()](erstellen-aktu-1367.md)  Neues Attribut createUser in der Funktion [getContractList()](request-getdvn-2417.md) |
| 4.7 | 31.07.2023 | Neuer Webservice [PartsService](partsservice-22419.md) in VehicleRepairOnline |
| 4.6 | 13.01.2023 | Neue Schnittstellenfunktion [getCalculationResultN()](abrufen-eines-19752.md) in VehicleRepairService |
| 4.5 | 02.12.2022 | Erweiterung der Funktion [exportDossierToDocument](exportieren-vo-2338.md)() im Parameter printProduct um den Wert depreciationinformation |
| 4.4 | 17.10.2022 | Erweiterung der Funktionen [getContract()](abrufen-eines-1469.md) und getCalculationResults() um das Element includeAttachments |
| 4.3 | 13.10.2022 | Neue Schnittstellenfunktion [calculateContract()](nach-kalkulier-18900.md) in VehicleRepairService |
| 4.2 | 13.10.2022 | Neue Schnittstellenfunktion [calculateN()](reparaturkoste-18882.md) in VehicleRepairService |
| 4.1 | 22.07.2022 | Neue Schnittstellenfunktion [getSparePartVariants()](abruf-aller-er-18568.md) in VehicleRepairService |
| 4.0 | 25.04.2022 | Neue Schnittstellenfunktion [deleteDossier()](loschen-eines-7783.md) in VehicleRepairService |
| 3.9 | 10.03.2022 | Erweiterung der Funktion [exportDossierToDocument](exportieren-vo-2338.md)() im Parameter printProduct um den Wert summary |
| 3.8 | 01.03.2022 | Neue Schnittstellenfunktionen: [getSparePartsDetails()](ermittlung-von-17159.md), [getSparePartsDetailsByVIN()](ermittlung-von-17163.md), [getSparePartsDetailsForDPN()](ermittlung-der-17164.md), [getSparePartsDetailsForDPNByVIN()](ermittlung-von-17165.md). |
| 3.7 | 24.02.2022 | Erweiterung der Funktion [exportDossierToDocument](exportieren-vo-2338.md)() im Parameter printProduct um den Wert calculationWithProtocol  Erweiterung der Funktion [getValidDATProcesses](abfragen-von-d-2366.md)() im Parameter coverage um den Wert GLASS und HAIL |
| 3.6 | 18.10.2021 | Entfernung der Funktion getCalculationResultsWithProtocol  Erweiterung der Funktion [getContractList](request-getdvn-2417.md) um ExternalId  Erweiterung der Funktion [exportDossierToDocument](exportieren-vo-2338.md) im Parameter printProduct um den Wert calculationWithImages |
| 3.5 | 30.03.2021 | Entfall der veralteten Funktion createContract  Neue Schnittstellenfunktion: calculateContractN |
| 3.4 | 30.04.2020 | Neue Eingabeparameter für die Integration der SilverDAT calculatePro/calculateExpert Oberfläche siehe [Aufbereitung der Eingabeparameter](aufbereitung-d-2393.md)  Neues Komplettbeispiel der Oberflächenintegration mit der JWT-Authentifizierung siehe [Komplettbeispiel](komplettbeispi-2505.md) |
| 3.4 | 30.04.2020 | Überarbeitung Hagelkalkulation, neues Berechnungsmodus "Vorziehen und Lackieren" (Deutsche Kommission für Lack und Karosserieinstandsssetzung) siehe [DENTS](additional-ver-2377.md) |
| 3.4 | 30.04.2020 | Entfernen der Funktionen: createContract und getCalculationResultsWithProtocol |
| 3.3 | 24.04.2019 | Neue Schnittstellenfunktionen: [importManualPositions](importieren-vo-11892.md), [exportManualPositions](exportieren-vo-11885.md) und [deleteAllManualPositions](loschen-von-ma-11904.md) |
| 3.2 | 24.07.2018 | Deaktivierung von createContractN ab 04/2018. |
| 3.1 | 11.04.2018 | Erweiterung Funktion getCalculationResults um das Element includeProtocol |
| 3.0 | 07.03.2018 | Neue Schnittstellenfunktion: [getLastPriceGenerationByMfr](abfrage-letzte-9195.md) |
| 2.9 | 21.07.2017 | Angleichen der Funktionen createContract und createContractN  Neue Dossier-Funktionen: createDossier und [deleteDossier](loschen-eines-7783.md). |
| 2.8 | 04.05.2017 | Angleichen der Dokumentation DE / EN |
| 2.7 | 05.12.2016 | Neue Schnittstellenfunktionen: createContractN, exportToDocument, getCalculationResultsWithProtocol, [getContract](abrufen-eines-1469.md), [getContractPriceGenerations](abruf-aller-vo-2343.md), [getInsurances](abrufen-von-la-2333.md), [getLacquerTypeKeys](abrufen-von-la-2345.md), [getLockedInfo](abfrage-des-be-2347.md), [getTemplates](abruf-aller-ex-2349.md), [setContractPriceGeneration](anderung-eines-2351.md), [setBlanketCalculation](festlegen-von-2353.md) |
| 2.6 | 11.02.2015 | Erweiterung Funktion getDossier |
| 2.5 | 23.07.2014 | Erweiterung Funktion getContractList |
| 2.4 | 07.05.2014 | Übersicht der Fehlermeldungen Webservice VehicleRepairOnline |
| 2.3 | 08.01.2014 | Änderung von locale und constructionTime für den gesamten Webservice; Erweiterung der Parameter für calculate |
| 2.2 | 21.08.2013 | Überarbeitung der Parameterlisten über alle Schnittstellenoperationen |
| 2.1 | 14.01.2013 | Erweiterung [Nutzungsvoraussetzungen](nutzungsvoraus-2359.md) und [Abruf von Wartungsintervallen](abruf-von-wart-2361.md); hinzugefügt [Abruf von Ausstattungen zu DVN](abruf-von-auss-2363.md) und [Abruf von DVNs anhand von DAT europa-Code, Bauzeit und AVs](abfragen-von-d-2366.md) |
| 2.0 | 06.11.2012 | Rückgabe der Ölfüllstandsmengen in calculateContract, [getMaintenanceIntervals](abruf-von-wart-2361.md), getCalculationResults |
| 1.9 | 23.08.2012 | Neue Schnittstellenfunktion [Exportieren von Dokumenten](response-getma-2391.md), Vorgangsbezeichnung jetzt unique |
| 1.8 | 22.05.2012 | Neues [values-Objekt](aufbereitung-d-2393.md) für den Oberflächenaufruf |
| 1.7 | 11.01.2012 | Mögliche Fehlercodes calculate; [Aufruf der SilverDAT calculatePro Oberfläche](aufruf-der-sil-2395.md) |
| 1.6 | 19.09.2011 | Überarbeitung Kapitel [Nutzungsvoraussetzungen](nutzungsvoraus-2359.md) |
| 1.5 | 25.08.2011 | Mögliche Fehlercodes calculate |
| 1.4 | 02.06.2011 | Erweiterung Request Request createContract  um optionale Parameter; neue Funktion Kalkulieren eines Vorgangs mit Vorgangs-Nr. |
| 1.3 | 19.05.2011 | [Aufbereitung der Eingabeparameter](aufbereitung-d-2393.md) |
| 1.2 | 01.03.2011 | Neue Funktion [getMaintenanceIntervals](abruf-von-wart-2361.md), Erweiterung getCalculationResults um Parameter locale; neuer Aufruf [der SilverDAT calculatePro Oberfläche](aufruf-der-sil-2395.md) |
| 1.1 | 23.11.2010 | Fehlercodes ergänzt |
| 1.0 | 08.11.2010 | Erst-Erstellung |
