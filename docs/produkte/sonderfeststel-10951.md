---
title: "Sonderfeststellungen anlegen"
topic_id: "10951"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Sonderfeststellungen anlegen"
---

# Sonderfeststellungen anlegen

Mit der Funktion setBasecheckSpecialAssesmentsDetails/setLeasingReturnSpecialAssesmentsDetails /setValuationExpertiseSpecialAssesmentsDetails/setEstimationCertificateSpecialAssesmentsDetails
legen Sie die Sonderfeststellung zu einem Produkt (Grundüberprüfung, Leasingrückgabe,
Bewertungsgutachten oder Schätzurkunde) zu dem bestehenden Vorgang an.

Parameter   
setBasecheckSpecialAssesmentsDetails  
setLeasingReturnSpecialAssesmentsDetails  
setValuationExpertiseSpecialAssesmentsDetails  
setEstimationCertificateSpecialAssesmentsDetails

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Einstiegselement, enthält sämtliche Eingabedaten zum Vorgang | numerisch | x |
| Comments | String | Kommentar |  |  |
| HydraulicRamp | String | Hebebühne | AVL = vorhanden, UNAVL = nicht vorhanden |  |
| NumberOfVehicleKeys | Long | Anzahl der Fahrzeugschlüssel |  |  |
| PerformedPaintCoatingThicknessMeasurement | Boolean | Lackschichtdickenmessung durchgeführt | true, false |  |
| Shunting | String | Rangierfahrt | DONE = durchgeführt, NDONE = nicht durchgeführt, NPSBL = nicht möglich |  |
| TestDrive | String | Probefahrt | DONE = durchgeführt, NDONE = nicht durchgeführt, NPSBL = nicht möglich |  |
| VehicleDirty | Boolean | Fahrzeug verschmutzt | true,false |  |
