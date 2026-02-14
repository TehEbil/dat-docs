---
title: "PartsService"
topic_id: "22419"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > PartsService"
---

# PartsService

Die technische Metabeschreibung des Services als WSDL (Web Services Description Language) kann unter der Adresse https://www.dat.de/VehicleRepairOnline/services/PartsService?wsdl abgerufen werden.

Bitte beachten Sie beim gewünschten Aufruf des Produkts SilverDat calculateExpert muss die Produktvariante "DAT-ProductVariant = calculateExpert" im SOAP-Header beim Authentifizierungsverfahren mit übergeben werden.

Der Service stellt die folgenden Funktionen zur Verfügung:

- [getSparePartsDetails()](#showid/24823 "Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie")
- [getSparePartsDetailsByVIN()](#showid/24830 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie")
- [getSparePartsDetailsForDPN()](#showid/24837 "Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie")
- [getSparePartsDetailsForDPNByVIN()](#showid/24844 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie ")
