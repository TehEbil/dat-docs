---
title: "Mögliche Fehlercodes getUsedVehicleForecast"
topic_id: "2204"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standard Restwertprognose Gebrauchtfahrzeuge > Mögliche Fehlercodes getUsedVehicleForecast"
---

# Mögliche Fehlercodes getUsedVehicleForecast

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:Server.CountryError | locale is missing | Der Parameter locale wurde nicht angegeben. |
| dat:validation.DatEquipmentId.missing | In der angegebenen Ausstattungsposition fehlt der Wert DATEquipmentId. | Der Parameter datEquipmentId fehlt unter equipmentPosition. Bitte geben Sie den Parameter datEquipmentId im Request an. |
| dat:validation.DatEquipmentId.invalid | Die angegebene DatEquipmentId ist ungültig. Mögliche Werte sind Zahlen zwischen 1 und 100000. | Der Parameter datEquipmentId enthält einen ungültigen Wert. Bitte korrigieren Sie den Wert und führen die Abfrage nochmals durch. |
| dat:validation.container.invalidForDatECode | Container existiert nicht für DAT €uropa-Code®. | Der Parameter Container enthält einen ungültigen Wert für den angegebenen DAT €uropa-Code®. |
| dat:validation.initialRegistration.missing | Erstzulassungsdatum fehlt. | Das Erstzulassungsdatum registrationDate fehlt oder enthält einen ungültigen Wert. Bitte prüfen Sie Ihre Angabe für den Parameter registrationDate. |
| dat:validation.initialRegistration.afterDataMonth | Erstzulassungsdatum liegt nach Datenmonat/-jahr. | Die Erstzulassung liegt in der Zukunft. Bitte korrigieren Sie die Erstzulasung. |
| dat:validation.mileage.missing | Kilometerstand fehlt. | Der Parameter mileage wurde nicht oder mit einem falschen Wert angegeben. |
| dat:validation.forecastItems.forecastItem.missing | Die Restwertprognosepositionen fehlen. | Restwertprognose-Elemente fehlen |
| dat:Server.valueNotFound | Format of return value for the unit is required. | Form der Wertrückgabe fehlt |
| dat:Server.valueNotFound | VAT is required. | Mehrwertsteuerangabe fehlt |
| dat:validation.priceType.missing | Die Art des Preises fehlt. | Preisartkennzeichen fehlt |
| dat:validation.decreaseType.missing | Die Abwertungsart fehlt. | Abwertungsartkennzeichen (für Ausstattungen) fehlt |
| dat:validation.constructionTime.missing | Bauzeit fehlt. | Der Parameter constructionTime wurde nicht oder mit einem falschen Wert angegeben. |
| dat:validation.valueType.invalid | Die Form der Wertrückgabe ist ungültig. Mögliche Werte sind 'Monetary', 'Mileage', 'Percentage'. | Für den Parameter valueType wurde ein ungültiger Wert angegeben. Bitte korrigieren Sie den Wert für den Parameter valueType. |
| dat:validation.includeVat.invalid | Die Mehrwertsteuerangabe ist ungültig. Mögliche Werte sind 'true', 'false'. | Für den Parameter includeVat wurde ein ungültiger Wert angegeben. Bitte korrigieren Sie den Wert für den Parameter includeVat. |
| dat:Server.wrongValueCode | Invalid decrease/devaluation indicator for equipment, allowed values are: 'Residual value', 'Table1', 'Table2', 'Table3', 'Table4', 'Default Table', 'RV', 'T1', 'T2', 'T3', 'T4', 'DT'. | Für den Parameter decreaseType oder devaluationType wurde ein ungültiger Wert angegeben. Bitte korrigieren Sie den Wert für den Parameter decreaseType oder devaluationType. |
| dat:validation.decreaseType.invalid | Die Abwertungsart ist ungültig. Mögliche Werte sind 'DAT', 'Maximum', 'Minimum'. | Das Abwertungsartkennzeichen curveType enthält einen ungültigen Wert. Bitte korrigieren Sie Wert für den Parameter curveType. |
| dat:validation.save.invalid | Das Speicherkennzeichen ist ungültig. Mögliche Werte sind 'true' oder 'false'. | Für den Parameter save wurde ein ungültiger Wert übergeben. Bitte korrigieren Sie den Wert für das Speicherkennzeichen. |
| dat:validation.priceType.invalid | Die Preisangabe ist ungültig. Mögliche Werte sind 'SalesPrice' oder 'PurchasePrice'. | Für den Parameter priceType wurde ein ungültiger Wert angegeben. Bitte korrigieren Sie den Wert für den Parameter priceType. |
| dat:Server.wrongValueCode | wrong value for release restriction | Ungültiger Wert für restriction. |
| dat:validation.forecastItems.subElement.missing | ageInMonths, mileagePerYear oder mileageTotal fehlt | Es fehlen Unterelemente von forecastItem. Bitte geben Sie die Parameter ageInMonths und mileagePerYear oder mileageTotal unter forecastItem an. |
| dat:validation.forecast\_vehicleAge.outOfRange | Eine Restwertprognose ist nicht mehr möglich, weil das Fahrzeugalter bereits 72 Monate oder mehr beträgt. | Eine Restwertprognose ist nur bis zu einem Fahrzeugalter von 72 Monate möglich. |
| dat:validation.mileage.invalid | Laufleistung ist ungültig. | Der Parameter mileage liegt außerhalb des gültigen Bereichs. |
