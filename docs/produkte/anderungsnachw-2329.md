---
title: "Änderungsnachweis"
topic_id: "2329"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Änderungsnachweis"
---

# Änderungsnachweis

Mit der jeweils aktuellsten Fassung verlieren alle früheren Versionen ihre Gültigkeit.

| Version | Datum | Änderung |
| --- | --- | --- |
| 5.5 | 02.09.2025 | Neue Werte maintenanceSchedule, withoutInsuranceData, withoutOwnerData, withoutDriverData, withoutGarageData, withoutOpponentData, withoutEquipments und withoutRepairCostExpansion im Parameter printProduct in der Request der Funktion [exportDossierToDocument()](#showid/2338 "Exportieren von Dokumenten").  Neuer Parameter finisNumber in der Request der Funktionen [getSparePartsDetails()](#showid/17314 "Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie"),  [getSparePartsDetailsByVIN](#showid/17318 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie")(), [getSparePartsDetailsForDPN()](#showid/17322 "Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie ") und [getSparePartsDetailsForDPNByVIN()](#showid/17326 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie ").  Neues Attribut finisNumber im Element [SparePartsInformation.](#showid/17192 "SparePartsInformation") |
| 5.4 | 12.03.2025 | Neues Attribut damageSegmentNumber in der Request der Funtkion [exportDossierToDocument()](#showid/2338 "Exportieren von Dokumenten") |
| 5.3 | 15.10.2024 | Neue Funktion [listAttachments()](#showid/26391 "Auflisten von Dokumenten") in [VehicleRepairService](https://www.dat.de/myClaim/soap/v2/VehicleRepairService) |
| 5.2 | 16.08.2024 | Neue Funktion [manageAttachments()](#showid/26088 "Hochladen, Überschreiben und Löschen von Dokumenten") in [VehicleRepairService](https://www.dat.de/myClaim/soap/v2/VehicleRepairService) |
| 5.1 | 26.04.2024 | Neue Eingabeparameter hideContractCreation, FasttrackWorkflow für die Integration der SilverDAT calculatePro/calculateExpert Oberfläche siehe [Aufbereitung der Eingabeparameter](#showid/2393 "Aufbereitung der Eingabeparameter") |
| 5.0 | 26.04.2024 | Neuer Wert für das Attribut crud "OVERWRITE\_KEEP\_ATTACHMENTS" in der Funktion [importDossier()](#showid/1367 "Erstellen, Aktualisiern und Überschreiben eines Vorgangs") |
| 4.9 | 17.01.2024 | Neue Funktion [getFillingQuantities()](#showid/22892 "Abrufen der Füllmengen anhand des DAT €urope-Codes") in [VehicleRepairService](#showid/2413 "VehicleRepairService")  Neuer Wert für das Attribut coverage in der Funktion getValidDATProcesses()  Neue Elemente in der Response der Funktionen getSparePartsDetails() und getSparePartsDetailsByVIN()  Neues Element Hint in der Response der Funktion getMaintenanceIntervals() |
| 4.8 | 10.10.2023 | Neue Funktion [getAdditionalItems()](#showid/22521 "Abrufen der Zusatzpositionen anhand des DAT €urope-Codes") in [VehicleRepairService](#showid/2413 "VehicleRepairService")  Neues Attribut automaticVinRequest in der Funktion [importDossier()](#showid/1367 "Erstellen, Aktualisiern und Überschreiben eines Vorgangs")  Neues Attribut createUser in der Funktion [getContractList()](#showid/2417 "Abfrage der Vorgangsübersicht") |
| 4.7 | 31.07.2023 | Neuer Webservice [PartsService](#showid/22419 "PartsService") in VehicleRepairOnline |
| 4.6 | 13.01.2023 | Neue Schnittstellenfunktion [getCalculationResultN()](#showid/19752 "Abrufen eines Kalkulationsergebnisses") in VehicleRepairService |
| 4.5 | 02.12.2022 | Erweiterung der Funktion [exportDossierToDocument](#showid/2338 "Exportieren von Dokumenten")() im Parameter printProduct um den Wert depreciationinformation |
| 4.4 | 17.10.2022 | Erweiterung der Funktionen [getContract()](#showid/1469 "Abrufen eines bestimmten Vorgangs") und getCalculationResults() um das Element includeAttachments |
| 4.3 | 13.10.2022 | Neue Schnittstellenfunktion [calculateContract()](#showid/18900 "(Nach-) Kalkulieren eines bestehenden Vorgangs") in VehicleRepairService |
| 4.2 | 13.10.2022 | Neue Schnittstellenfunktion [calculateN()](#showid/18882 "Reparaturkostenkalkulation ohne Speicherung ") in VehicleRepairService |
| 4.1 | 22.07.2022 | Neue Schnittstellenfunktion [getSparePartVariants()](#showid/18568 "Abruf aller Ersatzteilevarianten") in VehicleRepairService |
| 4.0 | 25.04.2022 | Neue Schnittstellenfunktion [deleteDossier()](#showid/7783 "Löschen eines Dossiers/Vorgangs") in VehicleRepairService |
| 3.9 | 10.03.2022 | Erweiterung der Funktion [exportDossierToDocument](#showid/2338 "Exportieren von Dokumenten")() im Parameter printProduct um den Wert summary |
| 3.8 | 01.03.2022 | Neue Schnittstellenfunktionen: [getSparePartsDetails()](#showid/17159 "Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie"), [getSparePartsDetailsByVIN()](#showid/17163 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie"), [getSparePartsDetailsForDPN()](#showid/17164 "Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie "), [getSparePartsDetailsForDPNByVIN()](#showid/17165 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie "). |
| 3.7 | 24.02.2022 | Erweiterung der Funktion [exportDossierToDocument](#showid/2338 "Exportieren von Dokumenten")() im Parameter printProduct um den Wert calculationWithProtocol  Erweiterung der Funktion [getValidDATProcesses](#showid/2366 "Abfragen von DVNs anhand von DAT €uropa-Code, Bauzeit und AVs")() im Parameter coverage um den Wert GLASS und HAIL |
| 3.6 | 18.10.2021 | Entfernung der Funktion getCalculationResultsWithProtocol  Erweiterung der Funktion [getContractList](#showid/2417 "Abfrage der Vorgangsübersicht") um ExternalId  Erweiterung der Funktion [exportDossierToDocument](#showid/2338 "Exportieren von Dokumenten") im Parameter printProduct um den Wert calculationWithImages |
| 3.5 | 30.03.2021 | Entfall der veralteten Funktion createContract  Neue Schnittstellenfunktion: calculateContractN |
| 3.4 | 30.04.2020 | Neue Eingabeparameter für die Integration der SilverDAT calculatePro/calculateExpert Oberfläche siehe [Aufbereitung der Eingabeparameter](#showid/2393 "Aufbereitung der Eingabeparameter")  Neues Komplettbeispiel der Oberflächenintegration mit der JWT-Authentifizierung siehe [Komplettbeispiel](#showid/2505 "Komplettbeispiel") |
| 3.4 | 30.04.2020 | Überarbeitung Hagelkalkulation, neues Berechnungsmodus "Vorziehen und Lackieren" (Deutsche Kommission für Lack und Karosserieinstandsssetzung) siehe [DENTS](#showid/2377 "DENTS (Veraltet!)") |
| 3.4 | 30.04.2020 | Entfernen der Funktionen: createContract und getCalculationResultsWithProtocol |
| 3.3 | 24.04.2019 | Neue Schnittstellenfunktionen: [importManualPositions](#showid/11892 "Importieren von manuellen Positionen"), [exportManualPositions](#showid/11885 "Exportieren von manuellen Positionen") und [deleteAllManualPositions](#showid/11904 "Löschen von manuellen Positionen") |
| 3.2 | 24.07.2018 | Deaktivierung von createContractN ab 04/2018. |
| 3.1 | 11.04.2018 | Erweiterung Funktion getCalculationResults um das Element includeProtocol |
| 3.0 | 07.03.2018 | Neue Schnittstellenfunktion: [getLastPriceGenerationByMfr](#showid/9195 "Abfrage letzter Preisstand eines Herstellers") |
| 2.9 | 21.07.2017 | Angleichen der Funktionen createContract und createContractN  Neue Dossier-Funktionen: createDossier und [deleteDossier](#showid/7783 "Löschen eines Dossiers/Vorgangs"). |
| 2.8 | 04.05.2017 | Angleichen der Dokumentation DE / EN |
| 2.7 | 05.12.2016 | Neue Schnittstellenfunktionen: createContractN, exportToDocument, getCalculationResultsWithProtocol, [getContract](#showid/1469 "Abrufen eines bestimmten Vorgangs"), [getContractPriceGenerations](#showid/2343 "Abruf aller vorhandenen Preisständen eines Vorgangs"), [getInsurances](#showid/2333 "Abrufen von länderspezifischen Versicherungen"), [getLacquerTypeKeys](#showid/2345 "Abrufen von Lackartschlüsseln"), [getLockedInfo](#showid/2347 "Abfrage des Bearbeitungsstatus/ -benutzer eines Vorgangs"), [getTemplates](#showid/2349 "Abruf aller existierenden Druckvorlagen"), [setContractPriceGeneration](#showid/2351 "Änderung eines Preisstands eines Vorgangs"), [setBlanketCalculation](#showid/2353 "Festlegen von Überschläge Kalkulationswerte") |
| 2.6 | 11.02.2015 | Erweiterung Funktion getDossier |
| 2.5 | 23.07.2014 | Erweiterung Funktion getContractList |
| 2.4 | 07.05.2014 | Übersicht der Fehlermeldungen Webservice VehicleRepairOnline |
| 2.3 | 08.01.2014 | Änderung von locale und constructionTime für den gesamten Webservice; Erweiterung der Parameter für calculate |
| 2.2 | 21.08.2013 | Überarbeitung der Parameterlisten über alle Schnittstellenoperationen |
| 2.1 | 14.01.2013 | Erweiterung [Nutzungsvoraussetzungen](#showid/2359 "Nutzungsvoraussetzungen") und [Abruf von Wartungsintervallen](#showid/2361 "Abruf von Wartungsintervallen: getMaintenanceIntervals"); hinzugefügt [Abruf von Ausstattungen zu DVN](#showid/2363 "Abruf von Ausstattungen zu DVN") und [Abruf von DVNs anhand von DAT europa-Code, Bauzeit und AVs](#showid/2366 "Abfragen von DVNs anhand von DAT €uropa-Code, Bauzeit und AVs") |
| 2.0 | 06.11.2012 | Rückgabe der Ölfüllstandsmengen in calculateContract, [getMaintenanceIntervals](#showid/2361 "Abruf von Wartungsintervallen: getMaintenanceIntervals"), getCalculationResults |
| 1.9 | 23.08.2012 | Neue Schnittstellenfunktion [Exportieren von Dokumenten](#showid/2391 "Response getMaintenanceIntervals"), Vorgangsbezeichnung jetzt unique |
| 1.8 | 22.05.2012 | Neues [values-Objekt](#showid/2393 "Aufbereitung der Eingabeparameter") für den Oberflächenaufruf |
| 1.7 | 11.01.2012 | Mögliche Fehlercodes calculate; [Aufruf der SilverDAT calculatePro Oberfläche](#showid/2395 "Aufruf der SilverDAT calculatePro / calculateExpert Oberfläche") |
| 1.6 | 19.09.2011 | Überarbeitung Kapitel [Nutzungsvoraussetzungen](#showid/2359 "Nutzungsvoraussetzungen") |
| 1.5 | 25.08.2011 | Mögliche Fehlercodes calculate |
| 1.4 | 02.06.2011 | Erweiterung Request Request createContract  um optionale Parameter; neue Funktion Kalkulieren eines Vorgangs mit Vorgangs-Nr. |
| 1.3 | 19.05.2011 | [Aufbereitung der Eingabeparameter](#showid/2393 "Aufbereitung der Eingabeparameter") |
| 1.2 | 01.03.2011 | Neue Funktion [getMaintenanceIntervals](#showid/2361 "Abruf von Wartungsintervallen: getMaintenanceIntervals"), Erweiterung getCalculationResults um Parameter locale; neuer Aufruf [der SilverDAT calculatePro Oberfläche](#showid/2395 "Aufruf der SilverDAT calculatePro / calculateExpert Oberfläche") |
| 1.1 | 23.11.2010 | Fehlercodes ergänzt |
| 1.0 | 08.11.2010 | Erst-Erstellung |
