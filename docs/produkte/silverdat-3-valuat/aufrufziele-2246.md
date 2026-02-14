---
title: "Aufrufziele"
topic_id: "2246"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Integration der Oberfläche > Aufruf der Oberfläche > Aufrufziele"
---

# Aufrufziele

Bitte beachten Sie die umfangreichen Abhängigkeiten der Aufrufziele.   
Die Aufrufziele sind vom Aktionstyp action, dem Typ des anzulegenden Vorgangs DossierType, der Fahrzeugart VehicleType und der Bewertungsart ValuationType abhängig

Übersicht der möglichen Aufrufziele

| Aufrufziel | Beschreibung | Schreibweise |
| --- | --- | --- |
| Vorgangsübersicht | Die Vorgangsübersicht listet alle angelegten Vorgänge auf. | showEventList |
| Auftragseröffnung | Die Auftragseröffnung enthält die Basisdaten für die historische Bewertung. | contract opening |
| Fahrzeugauswahl | Die Modellmaske beinhaltet die Fahrzeugdaten für die Fahrzeugauswahl. | model selection |
| Aufbauten | Maske mit den Aufbauten für Transporter und Lastwagen. | hgv platforms selection |
| Ausstattungsauswahl | Die Ausstattungsmaske listet die Serien-, Sonder- und Zusatzausstattungen auf. | equipment selection;  equipment selection (hgv platform) |
| Zustand | Die Fahrzeugzustandsmaske beinhaltet die Angaben zur Erfassung des Fahrzeugzustands. | vehicle condition |
| montierte Reifen | Maske zur Erfassung der montierten Reifen. | mounted tires evaluation |
| nicht montierte Reifen | Maske zur Erfassung der nicht montierten Reifen. | not mounted tires evaluation |
| Aufbauten Wertermittlung | Die Maske für die Wertermittlung der Aufbauten beinhaltet die Bewertungsangaben für die Aufbauten und deren Ausstattungen. | hgv platforms evaluation |
| Wertermittlung | Die Wertermittlungsmaske beinhaltet die Bewertungsangaben zum Fahrzeug. | evaluation |
| Stichtagsbewertung | Bewertungsangaben bezüglich eines Stichtags. | historical evaluation |
| Fahrzeugpreis | Grunddaten und Neupreise für Basisfahrzeug und Ausstattungen | new vehicle price |
| Restwertprognose | Die Restwertprognose beinhaltet die Angaben zur Fahrzeugrestwertprognose. | residual value forecast |
| Fahrzeugdaten | Übersicht der technischen Fahrzeugdaten. | vehicle data (from evaluation);  vehicle data (from historical evaluation);  vehicle data (from new vehicle price);  vehicle data (from residual value forecast) |
| Vergleichseröffnung | Die Vergleichseinstellungen beinhalten die Einstellungen und Vorgaben für den Vergleich. | compare preferences |
| Vergleichsmodelle | Übersicht der gewählten Modelle für den Vergleich. | compare models track |
| Vergleichsmodelle wählen | Maske zur Auswahl der Vergleichsmodelle Inland/Ausland | compare models national;  compare models international |
| Vergleichsergebnis | Modellvergleich in tabellarischer Form. | compare result |
| Grafischer Vergleich | Modellvergleich als Grafik. | charts |
| webScan | Börsenübersicht des Fahrzeugs im Vorgang | WebScanPage |

| Aufrufziel für  DossierType = evaluation | Gebrauchtfahrzeug | Neufahrzeug | Nur Transporter und LKW |
| --- | --- | --- | --- |
| model selection | X | X |  |
| equipment selection | X | X |  |
| hgv platforms selection | X | X | X |
| equipment selection (hgv platform) | X | X | X |
| vehicle condition | X |  |  |
| mounted tires evaluation | X |  |  |
| not mounted tires evaluation | X |  |  |
| hgv platforms evaluation | X |  | X |
| new vehicle price |  | X |  |
| vehicle data (from new vehicle price) |  | X |  |
| evaluation | X |  |  |
| vehicle data (from evaluation) | X |  |  |
| residual value forecast | X | X |  |
| vehicle data (from residual value forecast) | X | X |  |
| WebScanPage | X |  |  |

| Aufrufziel für  DossierType = historical evaluation | Gebrauchtfahrzeug | Neufahrzeug | Nur Transporter und LKW |
| --- | --- | --- | --- |
| contract opening | X |  |  |
| model selection | X |  |  |
| equipment selection | X |  |  |
| historical evaluation | X |  |  |
| vehicle data (from historical evaluation) | X |  |  |

| Aufrufziel für  DossierType = compare | Gebrauchtfahrzeug | Neufahrzeug | Nur Transporter und LKW |
| --- | --- | --- | --- |
| compare preferences | X |  |  |
| compare models track | X |  |  |
| compare models national | X |  |  |
| compare models international | X |  |  |
| equipment selection | X |  |  |
| compare result | X |  |  |
| charts | X |  |  |
