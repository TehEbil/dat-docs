---
title: "Änderungsnachweis"
topic_id: "2157"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Änderungsnachweis"
---

# Änderungsnachweis

Mit der jeweils aktuellsten Fassung verlieren alle früheren Versionen ihre Gültigkeit.

| Version | Datum | Änderung |
| --- | --- | --- |
| 3.7 | 08.02.2024 | Neuer Request-Parameter considerCurrentCondition für getUsedvehicleForecast, createDossierN und changeDossierN |
| 3.6 | 05.02.2020 | Neue Benutzerwerte für createDossierN; Responsebeschreibung für getVehicleApprixomateValue |
| 3.5 | 27.11.2020 | Neuer Service verfügbar: DossierN |
| 3.4 | 10.07.2020 | [Integration der Oberfläche](#showid/2160 "Integration der Oberfläche"), Erweiterung um die Parameter: pageList, vehicleIdentNumber, vehicleIdentNumberRequest, initialRegistration, mileageEstimated, kbaNumber, nationalCodeAustria, datECode, container und constructionTime |
| 3.3 | 20.05.2020 | Neue Option nationalCode für Funktion getVehicleApproximateValue |
| 3.2 | 19.09.2019 | Neuer Service verfügbar: BatchValuation und Erweiterung der Fehlermeldungen für die Methoden createDossier und changeDossier |
| 3.1 | 26.04.2019 | Entfall der Pflicht zur Angabe der Bauzeit bei der Restwertprognose von Neufahrzeugen mit getNewVehicleForecast und createDossier. |
| 3.0 | 13.07.2018 | Die Funktion [getVehicleApproximateValue](#showid/1818 "Parameter getVehicleApproximateValue ") wurde um den Mode AVERAGE erweitert. |
| 2.9 | 13.04.2017 | Bei [Integration der Oberfläche](#showid/2160 "Integration der Oberfläche") Verweise auf jQuery entfernt |
| 2.8 | 08.06.2016 | Integration des Services [Fahrzeugbilder Funktionen](#showid/2026 "Fahrzeugbilder Funktionen"); Änderung der Servicepfade von services nach soap |
| 2.7 | 28.05.2015 | Neues Kapitel: [Integration der Oberfläche](#showid/2160 "Integration der Oberfläche") |
| 2.6 | 14.04.2015 | Die überarbeitete Funktion searchDossierList ersetzt die veraltete Funktion searchDossier. |
| 2.5 | 14.05.2014 | Freigabe der Vorgangsverwaltung mit den Funktionen createDossier, getDossier, changeDossier, updateDossier, resetDossier2Default, deleteDossier, exportDossier, searchDossier. |
| 2.4 | 01.12.2013 | Ergänzung um Funktionen für DAT-interne Zwecke. |
| 2.3 | 01.08.2013 | Erweiterung um eine Vorgangsverwaltung, voraussichtlich zu 12/2013. |
| 2.2 | 03.07.2013 | Erweiterung der möglichen Werte des Elements coverage von [getNewVehicleForecast](#showid/2163 "Parameter getNewVehicleForecast "), [getUsedVehicleForecast](#showid/2165 "Parameter getUsedVehicleForecast "), [getVehicleApproximateValue](#showid/1818 "Parameter getVehicleApproximateValue "), [getVehicleEvaluation](#showid/2169 "Parameter getVehicleEvaluation ") und [getVehicleTargetDateEvaluationHistory](#showid/1832 "Parameter getVehicleTargetDateEvaluationHistory "). |
| 2.1 | 26.06.2013 | Erweiterung der möglichen Werte des Elements coverage von [getVehicleApproximateValue](#showid/1818 "Parameter getVehicleApproximateValue ").  Änderung der möglichen Werte des Elements accidentDamage, Korrektur des Trennzeichens und entsprechende Anpassung der Beispiele für die Requests von [getVehicleEvaluation](#showid/2169 "Parameter getVehicleEvaluation ") und [getVehicleTargetDateEvaluationHistory](#showid/1832 "Parameter getVehicleTargetDateEvaluationHistory ").  Umbennenung von "DescreaseType" in "DecreaseType" in den Responses von [getNewVehicleForecast](#showid/2163 "Parameter getNewVehicleForecast "), [getUsedVehicleForecast](#showid/2165 "Parameter getUsedVehicleForecast ") und [getVehicleTargetDateEvaluationHistory](#showid/1832 "Parameter getVehicleTargetDateEvaluationHistory "). |
| 2.0 | 16.01.2013 | Parameter coverage und save für alle Funktionen jetzt aktiv |
| 1.9 | 22.10.2012 | Erweiterung [Minimale Bewertung](#showid/2172 "Standardbewertung") und [stichtagsbezogene Bewertung durchfuhren](#showid/2177 "Stichtagsbezogene Bewertung durchführen (Historische Bewertung)"), um eine genauere Wertkorrektur durchführen zu können; neuer Fehlercode in [Moegliche Fehlercodes getVehicleApproximateValue](#showid/2179 "Mögliche Fehlercodes getVehicleApproximateValue") |
| 1.8 | 04.09.2012 | Einschrankung Bewertung |
| 1.7 | 20.08.2012 | Erweiterung aller Bewertungsschnittstellen um Mehrwertsteuer. Siehe Handbuch VXS; Erweiterung aller Bewertungsschnittstellen um Besteuerungsart vatType, optional; neue Funktion zur [Historischen Bewertung](#showid/2177 "Stichtagsbezogene Bewertung durchführen (Historische Bewertung)") |
| 1.6 | 12.01.2012 | Erweiterung [Annäherungsbewertung](#showid/2174 "Annäherungsbewertung") um Parameter Model |
| 1.5 | 04.11.2011 | neuer Wert für devaluationType (nur AT) in [Annäherungsbewertung](#showid/2174 "Annäherungsbewertung") und [Minimale Bewertung](#showid/2172 "Standardbewertung") |
| 1.4 | 26.07.2011 | Änderungen in [Minimale Restwertprognose Neufahrzeuge](#showid/2185 "Standard Restwertprognose Neufahrzeuge") und [Minimale Restwertprognose Gebrauchtfahrzeuge](#showid/2187 "Standard Restwertprognose Gebrauchtfahrzeuge") |
| 1.3 | 07.07.2011 | neues Rückgabefeld IdentificationSource in [Annäherungsbewertung](#showid/2174 "Annäherungsbewertung") |
| 1.2 | 08.11.2010 | Überarbeitung/Ergänzung aller Funktions-Parameter; Überarbeitung Authentifizierung und Dokument-Struktur |
| 1.1 | 02.09.2010 | Ergänzung Requests/Responses |
| 1.0 | 21.08.2010 | Erst-Erstellung |
