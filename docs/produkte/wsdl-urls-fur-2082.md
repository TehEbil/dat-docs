---
title: "WSDL-URLs für das Produkt autoglas Plus /SilverDAT calculateGlass"
topic_id: "2082"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Grundlagenwissen > Definition Webservice > WSDL-URLs für das Produkt autoglas Plus /SilverDAT calculateGlass"
---

# WSDL-URLs für das Produkt autoglas Plus /SilverDAT calculateGlass

| Gewünschte Funktion | Pfad zur WSDL | Weitere Informationen finden Sie in |
| --- | --- | --- |
| Eröffnen eines neuen Vorgangs in autoglas Plus / SilverDAT calculateGlass | https://www.dat.de/GlassRep/services/DMSCreateContract?wsdl | [automatische Erzeugung eines Vorgangs](#showid/2084 "automatische Erzeugung eines Vorgangs mit createContract") |
| Abrufen eines bestimmten Vorgangs | https://www.dat.de/GlassRep/services/DMSGetContracts?wsdl | [Abrufen eines einzelnen Vorgangs mit getContract](#showid/2086 "Abrufen eines einzelnen Vorgangs mit getContract") |
| Abrufen einer Liste von Vorgangsnummern, die kalkuliert und versendet, aber noch nicht abgerufen wurden | https://www.dat.de/GlassRep/services/DMSGetContracts?wsdl | [Abrufen einer Liste von Vorgangsnrn mit getNewConctractNumbers](#showid/2088 "Abrufen einer Liste von Vorgangsnummern mit getNewConctractNumbers") |
| Abrufen aller Vorgänge, die kalkuliert und versendet, aber noch nicht abgerufen wurden. Mit Komplettdaten | https://www.dat.de/GlassRep/services/DMSGetContracts?wsdl | [Mengen-Abruf von Kalkulationen mit getNewContracts](#showid/2090 "Mengen-Abruf von Kalkulationen mit getNewContracts") |

In manchen Fällen wird es notwendig sein, dass eine Nacherfassung der Daten stattfindet.
Diese Nacherfassung wird über die Oberfläche durchgeführt. Auch die Kalkulation des
Glasschadenvorgangs wird über die Oberfläche durchgeführt.

In beiden Fällen müssen Sie die Oberflächen-Schnittstelle benutzen. Weitere Informationen
finden Sie im Kapitel [Aufruf der Anwendungsoberfläche über Schnittstelle](#showid/2064 "Aufruf der Anwendungsoberfläche über Schnittstelle").
