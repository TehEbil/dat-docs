---
title: "Spezifische Fahrzeugdaten anlegen"
topic_id: "10940"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Spezifische Fahrzeugdaten anlegen"
---

# Spezifische Fahrzeugdaten anlegen

Mit der Funktion setCommonCheckListforBaseCheck/setCommonCheckListforLeasingReturn/setCommonCheckListValuationExpertise/setCommonCheckListEstimationCertificate
legen Sie die spezifischen Fahrzeugdaten zu einem Produkt (Grundüberprüfung, Leasingrückgabe,
Zustandsbericht, Bewertungsgutachten oder Schätzurkunde) zu den bestehenden Vorgang
an.

Parameter  
setCommonCheckListforBaseCheck  
setCommonCheckListforLeasingReturn  
setCommonCheckListforConditionReport  
setCommonCheckListValuationExpertise  
setCommonCheckListEstimationCertificate

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Einstiegselement, enthält sämtliche Eingabedaten zum Vorgang | numerisch | x |
| AirConditionChecked | Boolean | Klimaanlage geprüft | true,false |  |
| BoardWalletAvailable | Boolean | Bordmappe geprüft | true,false |  |
| DateOfExpiry | Date | Gültig bis | JJJJ-MM-DD |  |
| ExpertDefinedMileage | Long | Laufleistung (Sachverständiger) |  |  |
| HeatedSeatsChecked | Boolean | Sitzheizung geprüft | true,false |  |
| LastServiceDate | Date | Letzter Kundendienst | JJJJ-MM-DD |  |
| LastServiceKilometer | Long | Letzte Kilometerstand |  |  |
| NavigationChecked | Boolean | Navigation geprüft | true,false |  |
| NextMOT | Date | Nächste Hauptuntersuchung | JJJJ-MM |  |
| NextMOTStatus | String | Hauptuntersuchungsstatus | DUE = Fällig ,UNKN = Unbekannt |  |
| OdoMeterMileage | Long | Laufleistung (Tacho) |  |  |
| RegistrationInServiceBook | String | Eintragungen im Serviceheft | CMLT = vollständig, NCMLT = lückenhaft, NONE = keine |  |
| ServiceBookChecked | String | Serviceheft geprüft | INPR = in Papierform, DTL = digital, UNAVL = nicht vorhanden |  |
| TireRapairkitAvailable | Boolean | Reifenreparaturset vorhanden | true,false |  |
| ToolKitAvailable | Boolean | Bordfahrzeug vorhanden | true,false |  |
| VehicleMileage | Long | Laufleistung (Fahrzeugdaten) |  |  |
| VehiclePapersPart1 | String | Fahrzeugdokumente 1 | PRST = lag vor ,NPRST = lag nicht vor |  |
| VehiclePapersPart2 | String | Fahrzeugdokumente 2 | PRST = lag vor ,NPRST = lag nicht vor |  |
| WindBreakAvailable | Boolean | Windschott vorhanden | true,false |  |
