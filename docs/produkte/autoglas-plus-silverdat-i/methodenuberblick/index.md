---
title: "Methodenüberblick"
topic_id: "2080"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Methodenüberblick"
---

# Methodenüberblick

Mit dem September Release 2025 entfallen die calculateGlass Schnittstellen, die unter https://www.dat.de/GlassRep/services?wsdl zu finden sind. Der Aufruf der SilverDAT calculateGlass Oberflächenschnittstelle wird
ebenfalls nicht mehr unterstützt. Bitte beachten Sie, dass die Applikation SilverDAT calculateGlass zukünftig durch SilverDAT 3 Glas (SilverDAT myClaim https://www.dat.de/myClaim/soap/v2/MyClaimExternalService?wsdl) ersetzt wird.

Bitte lesen Sie das Kapitel [WSDL-URLs für das Produkt autoglas Plus /SilverDAT calculateGlass](../grundlagenwissen/wsdl-urls-fur-2082.md) bevor Sie mit diesem Kapitel fortfahren.

Die Schnittstellenmethoden für autoglas Plus / SilverDAT calculateGlass werden über zwei Webservices zur Verfügung gestellt.

1. https://www.dat.de/GlassRep/services/DMSCreateContract?wsdl
2. https://www.dat.de/GlassRep/services/DMSGetContracts?wsdl

Folgende Methoden werden über sie zur Verfügung gestellt:

| https://www.dat.de/GlassRep/services/DMSCreateContract?wsdl | |
| --- | --- |
| createContract(createContractRequest request) | Eröffnen eines neuen Glasvorgangs in autoglas Plus. Übergeben wird ein Dossier in VXS-Struktur. Der Vorgang muss über die Oberfläche vervollständigt werden. |

| https://www.dat.de/GlassRep/services/DMSGetContracts?wsdl | |
| --- | --- |
| getNewContractNumbers() | Abrufen einer Liste aller nicht abgerufenen und versendeten Vorgangsnummern (setzt Kalkulation voraus) |
| getNewContracts() | Abrufen aller nicht abgerufenen und versendeten Vorgänge inkl. Daten (setzt Kalkulation voraus) |

Grundsätzlich erhalten Sie zu jedem Funktionsaufruf den angegebenen Rückgabewert.
Im Fehlerfall wird jedoch stattdessen ein SOAPFault ausgelöst, der einen Fehler-Code und eine Kurzbeschreibung enthält. SOAPFaults können von SOAP-Bibliotheken üblicherweise als Exceptions weitergereicht werden. Sie finden die Exceptions
zu jeder Methode in den gleichnamigen Kapiteln, unterhalb jeder Methode.

In manchen Fällen wird es notwendig sein, dass eine Nacherfassung der Daten stattfindet.
Diese Nacherfassung wird über die Oberfläche durchgeführt. Auch die Kalkulation des
Glasschadenvorgangs wird über die Oberfläche durchgeführt.

In beiden Fällen müssen Sie die Oberflächen-Schnittstelle benutzen. Weitere Informationen
finden Sie im Kapitel [Aufruf der Anwendungsoberfläche über Schnittstelle](../aufruf-der-anwendung/index.md).

- [abrufen-einer-2088](abrufen-einer-2088.md)
- [abrufen-eines-2086](abrufen-eines-2086.md)
- [automatische-e-2084](automatische-e-2084.md)
- [beispiel-reque-2114](beispiel-reque-2114.md)
- [beispiel-reque-2123](beispiel-reque-2123.md)
- [beispiel-reque-2133](beispiel-reque-2133.md)
- [beispiel-reque-2142](beispiel-reque-2142.md)
- [beispiel-respo-2118](beispiel-respo-2118.md)
- [beispiel-respo-2128](beispiel-respo-2128.md)
- [beispiel-respo-2137](beispiel-respo-2137.md)
- [beispiel-respo-2147](beispiel-respo-2147.md)
- [mengen-abruf-v-2090](mengen-abruf-v-2090.md)
- [methoden-2076](methoden-2076.md)
- [mogliche-fehle-2120](mogliche-fehle-2120.md)
- [mogliche-fehle-2130](mogliche-fehle-2130.md)
- [mogliche-fehle-2149](mogliche-fehle-2149.md)
- [parameter-crea-2109](parameter-crea-2109.md)
- [parameter-getn-2132](parameter-getn-2132.md)
- [parameter-getn-2141](parameter-getn-2141.md)
- [ruckgabewert-2116](ruckgabewert-2116.md)
- [ruckgabewert-g-2125](ruckgabewert-g-2125.md)
- [ruckgabewert-g-2135](ruckgabewert-g-2135.md)
- [ruckgabewert-g-2144](ruckgabewert-g-2144.md)
- [zeichensatz-2097](zeichensatz-2097.md)
- [zwingend-erfor-2122](zwingend-erfor-2122.md)
