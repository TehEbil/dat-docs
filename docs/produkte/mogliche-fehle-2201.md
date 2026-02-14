---
title: "Mögliche Fehlercodes getNewVehicleForecast"
topic_id: "2201"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standard Restwertprognose Neufahrzeuge > Mögliche Fehlercodes getNewVehicleForecast"
---

# Mögliche Fehlercodes getNewVehicleForecast

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:Server.CountryError | locale is missing | Der Parameter locale wurde nicht angegeben. |
| dat:validation.DatEquipmentId.missing | In der angegebenen Ausstattungsposition fehlt der Wert DATEquipmentId. | Der Parameter datEquipmentId fehlt unter equipmentPosition. Bitte geben Sie den Parameter datEquipmentId im Request an. |
| dat:validation.DatEquipmentId.invalid | Die angegebene DatEquipmentId ist ungültig. Mögliche Werte sind Zahlen zwischen 1 und 100000. | Der Parameter datEquipmentId enthält einen ungültigen Wert. Bitte korrigieren Sie den Wert und führen die Abfrage nochmals durch. |
| dat:validation.container.invalidForDatECode | Container existiert nicht für DAT €uropa-Code®. | Der Parameter Container enthält einen ungültigen Wert für den angegebenen DAT €uropa-Code®. |
| dat:validation.forecastItems.forecastItem.missing | Die Restwertprognosepositionen fehlen. | Restwertprognose-Elemente fehlen |
| dat:Server.valueNotFound | Format of return value for the unit is required. | Form der Wertrückgabe fehlt |
| dat:Server.valueNotFound | VAT is required. | Mehrwertsteuerangabe fehlt |
| dat:validation.priceType.missing | Die Art des Preises fehlt. | Preisartkennzeichen fehlt |
| dat:validation.decreaseType.missing | Die Abwertungsart fehlt. | Abwertungsartkennzeichen (für Ausstattungen) fehlt |
| dat:validation.valueType.invalid | Die Form der Wertrückgabe ist ungültig. Mögliche Werte sind 'Monetary', 'Mileage', 'Percentage'. | Für den Parameter valueType wurde ein ungültiger Wert angegeben. Bitte korrigieren Sie den Wert für den Parameter valueType. |
| dat:validation.includeVat.invalid | Die Mehrwertsteuerangabe ist ungültig. Mögliche Werte sind 'true', 'false'. | Für den Parameter includeVat wurde ein ungültiger Wert angegeben. Bitte korrigieren Sie den Wert für den Parameter includeVat. |
| dat:Server.wrongValueCode | Invalid decrease/devaluation indicator for equipment, allowed values are: 'Residual value', 'Table1', 'Table2', 'Table3', 'Table4', 'Default Table', 'RV', 'T1', 'T2', 'T3', 'T4', 'DT'. | Für den Parameter decreaseType oder devaluationType wurde ein ungültiger Wert angegeben. Bitte korrigieren Sie den Wert für den Parameter decreaseType oder devaluationType. |
| dat:validation.decreaseType.invalid | Die Abwertungsart ist ungültig. Mögliche Werte sind 'DAT', 'Maximum', 'Minimum'. | Das Abwertungsartkennzeichen curveType enthält einen ungültigen Wert. Bitte korrigieren Sie Wert für den Parameter curveType. |
| dat:validation.save.invalid | Das Speicherkennzeichen ist ungültig. Mögliche Werte sind 'true' oder 'false'. | Für den Parameter save wurde ein ungültiger Wert übergeben. Bitte korrigieren Sie den Wert für das Speicherkennzeichen. |
| dat:validation.priceType.invalid | Die Preisangabe ist ungültig. Mögliche Werte sind 'SalesPrice' oder 'PurchasePrice'. | Für den Parameter priceType wurde ein ungültiger Wert angegeben. Bitte korrigieren Sie den Wert für den Parameter priceType. |
| dat:Server.wrongValueCode | In given Value EquipmentPosition, value DATEquipmentID is missing | Der Parameter datEquipmentId unter equipmentPosition wurde nicht angegeben. |
| dat:Server.wrongValueCode | wrong value for release restriction | Ungültiger Wert für restriction. |
| dat:Server.ManufacturerNotLicensed | manufacturer not licensed | Sie sind nicht berechtigt den angegebenen Hersteller abzufragen. Bitte wenden Sie sich an den DAT Vertrieb: sales-support@dat.de. |
| dat:validation.newVehicle.RVP.notPossible | Für das angegebene Fahrzeug kann keine Neufahrzeug-Restwertprognose durchgeführt werden. | Eine Neufahrzeugprognose ist nicht mehr möglich, da es sich um kein Neufahrzeug handelt. |
| dat:validation.forecastItems.subElement.missing | ageInMonths, mileagePerYear oder mileageTotal fehlt | Es fehlen Unterelemente von forecastItem. Bitte geben Sie die Parameter ageInMonths und mileagePerYear oder mileageTotal unter forecastItem an. |
| dat:validation.mileage.invalid | Laufleistung ist ungültig. | Der Parameter mileage liegt außerhalb des gültigen Bereichs. |
