---
title: "Aufrufziele"
topic_id: "2325"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Integration der Oberfläche > Aufruf der Methoden von SilverDAT 3 valuateExpert Oberflächeintegration > Aufrufziele"
---

# Aufrufziele

Bitte beachten Sie die umfangreichen Abhängigkeiten der Aufrufziele.

Übersicht der Abhängigkeiten der Aufrufziele

| Abhängigkeit | Beschreibung |
| --- | --- |
| Lizenz | Bitte beachten Sie, dass aus lizenztechnischen Gründen bestimmte Funktionalitäten nicht freigeschaltet sein können. |
| Verwaltung | Bitte beachten Sie, dass die Vorgaben bei den Systemeinstellungen, insbesondere die Einstellungen in der Prozessverwaltung die möglichen Aufrufziele einschränken können. |
| Benutzer | Bitte beachten Sie, dass die Benutzerberechtigungen die möglichen Aufrufziele einschränken können. Die jeweiligen Berechtigungen werden über die Gruppenzuordnung bestimmt. |
| Aufrufparameter | Bitte beachten Sie, dass die Vorgaben in den Aufrufparametern die möglichen Aufrufziele einschränken können. |
| Dossier | Bitte beachten Sie, dass es Aufrufziele gibt, die mit einem leeren oder unvollständigen Dossier nicht zulässig sind. |
| Fahrzeugart | Bitte beachten Sie, dass es Aufrufziele gibt, die nur für bestimmte Fahrzeugarten zulässig sind. |

Übersicht der möglichen Aufrufziele

| Prozess | Aufrufziel | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| Übersicht | Vorgangsübersicht | Die Vorgangsübersicht listet die angelegten Vorgänge auf. | overview.eventlist |
| Wertermittlung | Neuanlage | Prozess zur Anlage eines neuen Vorgangs. | valuation.create |
| Wertermittlung | Auftragseröffnung | In der Auftragseröffnung erfassen Sie die Auftrags- und Kundendaten. | valuation.contractOpening |
| Wertermittlung | Modell | In der Modellmaske erfassen Sie die Fahrzeugdaten für die Fahrzeugauswahl. | valuation.model |
| Wertermittlung | Ausstattung | Die Ausstattungsmaske dient zur Anzeige und Auswahl der Serien-, Sonder- und Zusatzausstattungen. | valuation.equipment |
| Wertermittlung | Aufbauten | Maske für die Auswahl der Aufbauten für Transporter und Lastwagen. | valuation.truckbody |
| Wertermittlung | Zustand | Die Fahrzeugzustandsmaske dient zur Erfassung des Fahrzeugzustands. | valuation.condition |
| Wertermittlung | Aufbauten Wertermittlung | Die Maske für die Wertermittlung der Aufbauten beinhaltet die Bewertungsangaben für die Aufbauten und deren Ausstattungen. | valuation.truckbodyValuation |
| Wertermittlung | Wertermittlung | In der Wertermittlungsmaske finden Sie die Bewertungsangaben zum Fahrzeug, sowie die Eingabefelder zum Überschreiben der DAT-Werte. | valuation.historyValuation |
| Wertermittlung | webScan | Börsenscanner zur vereinfachten Vergleichsabfrage der Gebrauchtfahrzeugbörsen | valuation.webscan |
| Wertermittlung | Wertdefinition | Die Maske für die Wertdefinition dient zur Eingabe der Festlegungen des Sachverständigen | valuation.valueDefinition |
| Produzieren | Produzieren | Diese Maske dient zur Steuerung der Ausdrucke | compile.compile |
| Administration | Stammdaten | Konfiguration der Anwendung wie zum Beispiel: Texte, Reparaturkostenparameter, Steuersatzeinstellungen usw. | masterData.entryPage |
| Administration | Systemoptionen | Einstellung der Firmendaten | systemOptions.entryPage |
| Administration | Benutzereinstellungen | Defaults für die Fahrzeugauswahl, Maskenverhalten und Landeseinstellung | userSettings.userSettingsPage |

Übersicht der Aufrufziele, die nur für bestimmte Fahrzeugarten VehicleType möglich sind.

| Aufrufziel | Transporter und LKW |
| --- | --- |
| valuation.truckbody | X |
| valuation.truckbodyValuation | X |
