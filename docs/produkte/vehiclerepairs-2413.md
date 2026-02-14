---
title: "VehicleRepairService"
topic_id: "2413"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService"
---

# VehicleRepairService

Die technische Metabeschreibung des Services als WSDL (Web Services Description Language) kann unter der Adresse https://www.dat.de/VehicleRepairOnline/services/VehicleRepairService?wsdl abgerufen werden.

Bitte beachten Sie beim gewünschten Aufruf des Produkts SilverDat calculateExpert muss die Produktvariante "DAT-ProductVariant = calculateExpert" im SOAP-Header beim Authentifizierungsverfahren mit übergeben werden.

Der Service stellt die folgenden Funktionen zur Verfügung:

- [calculateN()](#showid/18882 "Reparaturkostenkalkulation ohne Speicherung ")
- [calculateContract()](#showid/18900 "(Nach-) Kalkulieren eines bestehenden Vorgangs")
- [exportDossierToDocument()](#showid/2338 "Exportieren von Dokumenten")
- [getCalculationResultN()](#showid/19752 "Abrufen eines Kalkulationsergebnisses")
- [getContract()](#showid/1469 "Abrufen eines bestimmten Vorgangs")
- [getContractList()](#showid/2417 "Abfrage der Vorgangsübersicht")
- [getContractPriceGenerations()](#showid/2343 "Abruf aller vorhandenen Preisständen eines Vorgangs")
- [getDVNEquipments()](#showid/2363 "Abruf von Ausstattungen zu DVN")
- [getAdditionalItems()](#showid/22521 "Abrufen der Zusatzpositionen anhand des DAT €urope-Codes")
- [getFillingQuantities()](#showid/22892 "Abrufen der Füllmengen anhand des DAT €urope-Codes")
- [getInsurances()](#showid/2333 "Abrufen von länderspezifischen Versicherungen")
- [getLacquerTypeKeys()](#showid/2345 "Abrufen von Lackartschlüsseln")
- [getLockedInfo()](#showid/2347 "Abfrage des Bearbeitungsstatus/ -benutzer eines Vorgangs")
- [getMaintenanceIntervals()](#showid/2361 "Abruf von Wartungsintervallen: getMaintenanceIntervals")
- [getSparePartsDetails()](#showid/17159 "Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie")
- [getSparePartsDetailsByVIN()](#showid/17163 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie")
- [getSparePartsDetailsForDPN()](#showid/17164 "Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie ")
- [getSparePartsDetailsForDPNByVIN()](#showid/17165 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie ")
- [getSparePartVariants](#showid/18568 "Abruf aller Ersatzteilevarianten")()
- [getTemplates()](#showid/2349 "Abruf aller existierenden Druckvorlagen")
- [getValidDATProcesses()](#showid/2366 "Abfragen von DVNs anhand von DAT €uropa-Code, Bauzeit und AVs")
- [importDossier()](#showid/1367 "Erstellen, Aktualisiern und Überschreiben eines Vorgangs")
- [manageAttachments()](#showid/26088 "Hochladen, Überschreiben und Löschen von Dokumenten")
- [setBlanketCalculation()](#showid/2353 "Festlegen von Überschläge Kalkulationswerte")
- [setContractPriceGeneration()](#showid/2351 "Änderung eines Preisstands eines Vorgangs")
- [getLastPriceGenerationByMfr()](#showid/9195 "Abfrage letzter Preisstand eines Herstellers")
- [exportManualPositions()](#showid/11885 "Exportieren von manuellen Positionen")
- [importManualPositions()](#showid/11892 "Importieren von manuellen Positionen")
- [listAttachments()](#showid/26391 "Auflisten von Dokumenten")
- [deleteAllManualPositions()](#showid/11904 "Löschen von manuellen Positionen")
- [deleteDossier()](#showid/7783 "Löschen eines Dossiers/Vorgangs")
