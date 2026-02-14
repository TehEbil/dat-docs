---
title: "Aufrufziele"
topic_id: "2503"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Integration der Oberfläche > Aufruf der SilverDAT calculatePro / calculateExpert Oberfläche > Aufrufziele"
---

# Aufrufziele

Folgende Aufrufziele können über die calculatePro Oberflächenschnittstelle angesprochen werden:

| Aufrufziel | Aufrufparameter | Beschreibung |
| --- | --- | --- |
| Vorgangsübersicht | ``` sphinx.init(sphinx.host + "/eventList/eventList.html", "eventList", document.getElementById('iframeContainer'),  "modelIFrame"); ``` | Die Vorgangsübersicht listet alle angelegten Vorgänge auf. |
| Auftragseröffnung | ``` sphinx.init(sphinx.host + "/vehicleRepair/contractOpening.tmpl", "contractOpening", document.getElementById('iframeContainer'), "modelIFrame"); ``` | Die Auftragseröffnungsmaske enthält u.a. auch die Halterdaten und ist die Einstiegsmaske, um einen Vorgang anzulegen. |
| Fahrzeugauswahl | ``` sphinx.init(sphinx.host + "/vehicleSelection/model.tmpl", "model", document.getElementById('iframeContainer'), "modelIFrame"); ``` | In der Fahrzeugauswahl kann ein Fahrzeug manuell ausgewählt oder per VIN oder DAT €uropa-Code® identifiziert werden. |
| Ausstattungen | ``` sphinx.init(sphinx.host + "/vehicleSelection/equipmentPage.tmpl", "equipmentPage", document.getElementById('iframeContainer'), "modelIFrame"); ``` | Die Ausstattungsmaske listet die Serien-, Sonder- und Zusatzausstattungen auf. |
| Vorgangsbezogene Daten | ``` sphinx.init(sphinx.host + "/vehicleRepair/vroActivityRelatedDataPage.tmpl", "activityRelatedData", document.getElementById('iframeContainer'),  "modelIFrame"); ``` | In der Maske Vorgangsbezogene Daten können - bezogen auf den aktuellen Vorgang - Parameter verändert oder ergänzt werden. Z.B. Ersatzteil- und Arbeitslohnfaktoren oder Lackfaktoren. |
| Graphische Teileauswahl | ``` sphinx.init(sphinx.host + "/vehicleRepair/graphicalPartSelectionPage.tmpl", "graphicSelectionPage", document.getElementById('iframeContainer'), "modelIFrame"); ``` | In der graphischen Teileauswahl können Sie Baugruppen und/oder Fahrzeugteile aus einer graphischen Fahrzeugdarstellung auswählen. Die Darstellung erfolgt in Form von Explosionszeichnungen, um die Auswahl zu vereinfachen. |
| Kalkulationsergebnis | ``` sphinx.init(sphinx.host + "/vehicleRepair/calculationResultPage.tmpl", "calculationResultPage", document.getElementById('iframeContainer'), "modelIFrame"); ``` | Die Maske Kalkulationsergebnis wird nach erfolgter Kalkulation angezeigt. Es unterteilt mehrere Bereiche, z.B. Halter, Fahrzeug, Lackierung, Ersatzteile etc. |
| Drucken und senden | ``` sphinx.init(sphinx.host + "/vehicleRepair/printAndSendPage.tmpl", "printAndSendPage", document.getElementById('iframeContainer'),"modelIFrame"); ``` | Über die Maske Drucken und senden kann das kalkulierte Ergebnis versandt und/oder ausgedruckt werden. |
| Regelsätze | ``` sphinx.init(sphinx.host + "/vehicleRepair/administrationPage.tmpl", "administrationPage", document.getElementById('iframeContainer'), "modelIFrame"); ``` | In der Maske Regelsätze zur Verrechnung können verschiedene Stundenverrechnungssätze für die Lohnarten Mechanik, Karosserie, Elektrik und Lack hinterlegt werden. Zu jedem erstellten Regelsatz können Auf- bzw. Abschläge für Lohn- und Teilepositionen definiert werden. Ebenso können Rabatte eingestellt werden. |
| Betriebsdaten | ``` sphinx.init(sphinx.host +  "/vehicleRepairOnline/vehicleRepairOnline/companyData.html",  "companyData",  document.getElementById('iframeContainer'),  "modelIFrame"); ``` | Hier können z.B. folgende Daten voreingestellt werden: Werkstattverrechnungssätze, Angaben zur Werkstatt selbst, Ansprechpartner |
| Einstellungen | ``` sphinx.init(sphinx.host + "/vehicleRepair/vehicleRepairOnline/companyData.html", "companyData", document.getElementById('iframeContainer'), "modelIFrame"); ``` | In der Maske Einstellungen können Voreinstellungen vorgenommen werden für die Verwendung langer Arbeitstexte, Auf- oder Abschläge im Protokoll oder in der Kalkulation, MwSt. Sätze und div. andere Einstellungen zur Beeinflussung der Kalkulation. |
| Druckvorlagen-Verwaltung | ``` sphinx.init(sphinx.host + "/vehicleRepair/layoutAdminPage.tmpl", "layoutAdminPage", document.getElementById('iframeContainer'), "modelIFrame"); ``` |  |

|  |  |
| --- | --- |
|  | Wird über firstPage eine ungültige Maske angegeben, geht der Sprung in die nächstmögliche Maske, z.B.:  - firstPage wird mit graphicSelectionPage, activityRelated, calculationResult oder printAndSend initialisiert, das Fahrzeug, ist aber noch gar nicht angelegt worden. Der Einsprung wird deshalb in die Modellmaske umgeleitet.  - firstPage wird mit printAndSend initialisiert, das Fahrzeug wurde aber noch nicht kalkuliert. Der Einsprung wird deshalb in die Ergebnismaske umgeleitet. |
| Achtung |
