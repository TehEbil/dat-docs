---
title: "SpareParts"
topic_id: "7755"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > SpareParts"
---

# SpareParts

Sowohl für das Produkt SilverDAT PartsInfo als auch für das bereits abgekündigte SilverDAT calculationAudit kann die technische Metabeschreibung des Services als WSDL (Web Services Description Language) unter der Adresse <https://www.dat.de/PartsInfo/services/SpareParts?wsdl> abgerufen werden.

Beim Zugriff auf das noch bestehende SilverDAT calculationAudit Produkt muss die Produktvariante "productVariant = etn" im SOAP-Header beim Authentifizierungsverfahren übergeben werden.

Der Service stellt die folgenden Funktionen zur Verfügung:

- [getExtPartNoInfoByFullVehicleAndIntPartNo](#showid/2513 "Rückgabe von ETN über DAT europa-Code Ausstattung und DVN  ")
- [getExtPartNoInfoByMfrAndExtPartNo](#showid/2543 "Informationsermittlung mit Herstellerschlüssel und ETN ")
- [getExtPartNoInfoByModelAndExtPartNo](#showid/2539 "Informationsermittlung mit Untertyp und ETN")
- [getExtPartNoInfoByVinAndIntPartNo](#showid/2535 "Rückgabe ETN über VIN und DVN")
- [getModelInfoByMfrAndExtPartNo](#showid/2520 "Rückgabe von Modellinfo über HST und ETN")
