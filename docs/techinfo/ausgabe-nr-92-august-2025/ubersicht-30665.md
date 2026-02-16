---
title: "Übersicht"
topic_id: "30665"
breadcrumb: "Technische Informationen > Ausgabe Nr. 92 August 2025 > Übersicht"
---

# Übersicht

Sehr geehrte DAT Schnittstellenpartner,

in dieser Ausgabe Newsletter 092 geben wir Ihnen einen Ausblick auf die Neuerungen der Schnittstellen, die mit dem
nächsten Release 2025-004 bereitgestellt werden:

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

Bitte beachten Sie, dass mit dem Dezember-Release 2025 die Endpunkte der veralteten
API-Version 0.1 des Image Analysis Service nach der Abkündigungszeit von 6 Monaten
aus der Schnittstelle entfernt werden. Dies betrifft die Produkte SilverDAT calculatePro/calculateExpert
und myClaim.

Bitte berücksichtigen Sie dies in Ihrer eigenen Implementierung und stellen Sie rechtzeitig
auf die API-Version v2 um!

Folgende Endpunkte der API-Version 0.1 werden entfernt:

- https://imageanalysisservice.dat.de/0.1/calculate/
- https://imageanalysisservice.dat.de/0.1/myClaim/

Neue Endpunkte der API-Version v2:

- https://imageanalysisservice.dat.de/v2/calculate/
- https://imageanalysisservice.dat.de/v2/myClaim/

Fragen zum Schnittstellen-Kompendium beantwortet Ihnen unser Kundendienst für Schnittstellenpartner
[interfaces@dat.eu](mailto:interfaces@dat.eu "Mail an DAT interfaces").

Bitte geben Sie uns bei Anfragen die folgenden Informationen:

- Kundennummer <DAT-Kundennummer des Mandanten>
- Adresse anstelle der Kundennummer
- Ansprechpartner
- Rückrufnummer

Bei Anfragen zu Schnittstellenfunktionen bitte:

- Angabe des Produkts, zu dem die Funktion gehört
- Request und Response des Funktionsaufrufes

Mit diesen Angaben können wir Ihr Anliegen rasch bearbeiten.

Bitte arbeiten Sie immer mit der aktuellsten Version!

Mit freundlichen Grüßen

Ihr DAT Schnittstellenpartner-Team

© Dieses Dokument ist Eigentum der DAT GmbH.

Es ist ausdrücklich nur für Schnittstellenpartner der DAT erstellt.

Alle Rechte vorbehalten. Jede Art der Vervielfältigung ohne Erlaubnis der DAT GmbH
ist unzulässig.
