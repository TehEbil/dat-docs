---
title: "Neues der SilverDAT Schnittstellen für 2026"
topic_id: "7458"
breadcrumb: "Allgemeine Informationen > Neues der SilverDAT Schnittstellen für 2026"
---

# Neues der SilverDAT Schnittstellen für 2026

Sehr geehrte DAT Schnittstellenpartner,

Die Neuigkeiten zum Update Februar 2026:

Anpassungen in der Service Authentication

Bitte beachten Sie, dass die Funktion authenticateUser mit dem Februar Release im Jahr 2026 nach Einhaltung der Abkündigungszeit von 6 Monaten
endgültig aus der Schnittstelle entfernt wird. Die folgenden Elemente aus der Schemadatei
Authentication (Authentication\_schema1.xsd) werden ebenfalls endgültig aus der Schnittstelle entfernt:

- datCredentials
- datrcbkb
- datrcpda
- baseBusinessObject
- datrcpkk
- datrcpan
- authenticationMethod
- httpMethodEnum
- interfaceType
- authorizationErrorCode
- localDateTime

Wichtige Änderung der Endpunkte des Image Analysis Service

Bitte beachten Sie, dass mit dem April-Release 2026 die Endpunkte der veralteten API-Version
0.1 des Image Analysis Service nach der Abkündigungszeit von 6 Monaten aus der Schnittstelle
entfernt werden. Dies betrifft die Produkte SilverDAT calculatePro/calculateExpert
und myClaim.

Bitte berücksichtigen Sie dies in Ihrer eigenen Implementierung und stellen Sie rechtzeitig
auf die API-Version v2 um!

Folgende Endpunkte der API-Version 0.1 werden entfernt:

- https://imageanalysisservice.dat.de/0.1/calculate/
- https://imageanalysisservice.dat.de/0.1/myClaim/

Neue Endpunkte der API-Version v2:

- https://imageanalysisservice.dat.de/v2/calculate/
- https://imageanalysisservice.dat.de/v2/myClaim/

Fahrzeugauswahl und Fahrzeugidentifikation

Bitte beachten Sie den Umzug unserer Schnittstellenfunktionen getExistingEquipmentN,
getExistingEquipmentN und getEquipmentFromManufacturerCodeN vom ConversionFunctionsService
in den VehicleSelectionService.

Weitere Details finden Sie in Technische Information Nr. 94 unter [Umzug von Funktionen](../techinfo/ausgabe-nr-94-dezember-20/fahrzeugidentifikati/umzug-von-funk-31561.md).

Für die Nutzung unserer VIN-Abfrage sprechen Sie bitte über den VIN-Lizenzvertrag
mit dem DAT-Vertrieb: [sales-support@dat.de](mailto:sales-support@dat.de "Mail an DAT Sales Support") oder [vertrieb@dat.de](mailto:vertrieb@dat.de "Mail an DAT Vertrieb").

DAT Kundenservice für Schnittstellenpartner

Bitte geben Sie uns bei Anfragen Ihre Kundennummer <DAT-Kundennummer des Mandanten>, alternativ Ihre Adresse sowie einen Ansprechpartner
und eine Rückrufnummer an.

Bei Anfragen zu Schnittstellenfunktionen brauchen wir die Angabe des SilverDAT Produkts, zu dem die Schnittstelle gehört sowie Request und Response der betreffenden Funktion. Mit diesen Angaben können wir Ihr Anliegen schneller bearbeiten.

Wünschen Sie mehr Informationen oder Beratung?  
Bitte nehmen Sie Kontakt mit uns auf: [interfaces@dat.eu](mailto:interfaces@dat.eu "Mail DAT interfaces")

Mit den besten Empfehlungen  
Ihr DAT Team für die DAT Schnittstellenpartner

© Dieses Dokument ist Eigentum der DAT GmbH.

Alle Rechte vorbehalten. Jede Art der Vervielfältigung ohne Erlaubnis der DAT GmbH
ist unzulässig.
