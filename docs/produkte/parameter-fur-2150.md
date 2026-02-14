---
title: "Parameter für Auftragserfassung mit VXS-Datei"
topic_id: "2150"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Aufruf der Anwendungsoberfläche über Schnittstelle > Parameter für Auftragserfassung mit VXS-Datei"
---

# Parameter für Auftragserfassung mit VXS-Datei

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld Y/N |
| --- | --- | --- | --- | --- |
| customerNumber | String | DAT-Kunden-Nr. | DAT-Kunden-Nr. | Y |
| userLogin | String | Login-Name | Login-Name | Y |
| signature | String | s. Beschreibung | Codierter Base64 String, analog zum Kapitel [Authentifizierung der SilverDAT Webservices](#showid/1294 "Authentifizierung der SilverDAT Webservices") | Y |
| productVariant | String | - glassrep.mbg für Mercedes Benz Glas  - glassrep.vwg für Volkswagen Glas  - glassrep.sdg für SilverDAT calculateGlass  - glassrep.agp für autoglas Plus  - glassrep.aug für Audi Glas  - glassrep.nsg für Nissan Glas | Kürzel für die zugeordnete Glas-Anwendung | Y |
| vxsFile | file | VXS-Datei | Die Daten, die Sie übergeben, müssen in einer validen VXS-Datei übergeben werden. | Y |
