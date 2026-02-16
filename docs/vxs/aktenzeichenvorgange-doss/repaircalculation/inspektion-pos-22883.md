---
title: "Inspektion-Positionen (InspectionPosition(s))"
topic_id: "22883"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Inspektion-Positionen (InspectionPosition(s))"
---

# Inspektion-Positionen (InspectionPosition(s))

Unter den in "[Kalkulationsergebnisse](kalkulationser-1409.md)" aufgeführten Elementen gibt es das Element <InspectionPositions>, das mehrere <InspectionPosition>-Elemente enthält. Diese enthalten Informationen die kalkulierten HU/AU-Positionen.

Felder

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DATProcessId | Integer, optional | DAT-Verarbeitungsnummer (DVN) |
| PartNumber | String, optional | Ersatzteilnummer |
| Description | String, optional | Beschreibung der HU/AU-Position |
| Amount | Decimal, optional | Menge |
| ValuePerUnit | Decimal, optional | Preis pro Einheit |
| QuantityUnit | String, optional | Einheit Material |
| TaxNeutral | Boolean, optional | Information ob die HU/AU-Position steuerneutral kalkuliert wurde |
| Location | String, optional | Ortsangabe vom Schaden am Fahrzeug |
| WorkNumber | String, optional | Arbeitspositionsnummer |
| RepairType | String, optional | Reparatur-Art |
| WageType | String, optional | Arbeitsart |
| WageLevel | Integer, optional | Arbeitsstufe |
| Duration | Decimal, optional | Dauer (in Stunde oder Herstellerzeitmaß) |
| ValueTotal | Decimal, optional | Preis gesamt |
