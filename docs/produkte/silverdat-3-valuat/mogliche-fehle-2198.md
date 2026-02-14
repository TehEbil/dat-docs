---
title: "Mögliche Fehlercodes getVehicleEvaluation"
topic_id: "2198"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standardbewertung > Mögliche Fehlercodes getVehicleEvaluation"
---

# Mögliche Fehlercodes getVehicleEvaluation

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:validation.container.invalidForDatECode | Container existiert nicht für DAT €uropa-Code®. | Der Parameter Container enthält einen ungültigen Wert für den angegebenen DAT €uropa-Code®. |
| dat:validation.DatEquipmentId.missing | In der angegebenen Ausstattungsposition fehlt der Wert DATEquipmentId. | Der Parameter datEquipmentId fehlt unter equipmentPosition. Bitte geben Sie den Parameter datEquipmentId im Request an. |
| dat:validation.DatEquipmentId.invalid | Die angegebene DatEquipmentId ist ungültig. Mögliche Werte sind Zahlen zwischen 1 und 100000. | Der Parameter datEquipmentId enthält einen ungültigen Wert. Bitte korrigieren Sie den Wert und führen die Abfrage nochmals durch. |
| dat:validation.save.invalid | Das Speicherkennzeichen ist ungültig. Mögliche Werte sind 'true' oder 'false'. | Für den Parameter save wurde ein ungültiger Wert übergeben. Bitte korrigieren Sie den Wert für das Speicherkennzeichen. |
| dat:Server.valueNotFound | Missing memory indicator. | Speicherkennzeichen fehlt |
| dat:validation.initialRegistration.missing | Erstzulassungsdatum fehlt. | Das Erstzulassungsdatum registrationDate fehlt oder enthält einen ungültigen Wert. Bitte prüfen Sie Ihre Angabe für den Parameter registrationDate. |
| dat:validation.initialRegistration.afterDataMonth | Erstzulassungsdatum liegt nach Datenmonat/-jahr. | Die Erstzulassung registrationDate liegt in der Zukunft. Bitte korrigieren Sie die Erstzulasung. |
| dat:validation.registrationDate.inFuture | Das Erstzulassungsdatum liegt in der Zukunft | Die Erstzulassung registrationDate liegt in der Zukunft. Bitte korrigieren Sie die Erstzulasung. |
| dat:Server.wrongValueCode | Invalid decrease/devaluation indicator for equipment, allowed values are: 'Residual value', 'Table1', 'Table2', 'Table3', 'Table4', 'Default Table', 'RV', 'T1', 'T2', 'T3', 'T4', 'DT'. | Sie haben eine nicht erlaubte Abwertungsart benutzt. Bitte korrigieren Sie den Wert und führen die Abfrage nochmals durch. |
| dat:Server.wrongValueCode | wrong value for release restriction | Der Parameter restriction wurde nicht oder mit einem falschen Wert angegeben. |
| dat:validation.constructionTime.missing | Bauzeit fehlt. | Der Parameter constructionTime wurde nicht oder mit einem falschen Wert angegeben. |
| dat:validation.mileage.missing | Kilometerstand fehlt. | Der Parameter mileage wurde nicht oder mit einem falschen Wert angegeben. |
| dat:Server.ManufacturerNotLicensed | manufacturer not licensed | Sie sind nicht berechtigt den angegebenen Hersteller abzufragen. Bitte wenden Sie sich an den DAT Vertrieb: sales-support@dat.de. |
| dat:validation.condition.noPermission | No rights for processing state data. | Sie sind nicht berechtigt Zustandsdaten zu bearbeiten. |
| dat:validation.condition\_tiresUnmountedValue.outOfRange | Zustand: Wert der unmontierten Bereifung außerhalb des gültigen Bereichs [0.00 - 999999999.99]. | Der Wert der unmontierten Bereifung liegt außerhalb des gültigen Bereichs. Bitte korrigieren Sie den Wert der unmontierten Bereifung. |
| dat:validation.condition\_tiresMountedValue.outOfRange | Zustand: Wertanpassung der montierten Bereifung außerhalb des gültigen Bereichs [-999999999.99 - 999999999.99]. | Der Wert der montierten Bereifung liegt außerhalb des gültigen Bereichs. Bitte korrigieren Sie den Wert der montierten Bereifung. |
| dat:validation.condition\_correctionFactorPercent.outOfRange | Zustand: Zustands-Wertkorrektur außerhalb des gültigen Bereichs [70.00 - 130.00]. | Die Zustands-Wertkorrektur liegt außerhalb des gültigen Bereichs. Bitte korrigieren Sie die Zustands-Wertkorrektur. |
| dat:Server.CountryError | locale is missing | Der Parameter locale wurde nicht angegeben. |
| dat:validation.condition\_decreaseInValue.outOfRange | Zustand: Wertminderung außerhalb des gültigen Bereichs [0.00 - 999999999.99]. | Der Wert für die Wertminderung liegt außerhalb des gültigen Bereichs. Bitte geben Sie einen gültigen Wert für die Wertminderung an. |
| dat:validation.condition\_increaseInValue.outOfRange | Zustand: Werterhöhung außerhalb des gültigen Bereichs [0.00 - 999999999.99]. | Der Wert für die Werterhöhung liegt außerhalb des gültigen Bereichs. Bitte geben Sie einen gültigen Wert für die Werterhöhung an. |
| dat:validation.condition\_accidentDamage.invalid | Zustand: Unfallkennzeichen ungültig. | Der Wert für den Parameter accidentDamage ist ungültig. Bitte geben Sie einen gültigen Wert für accidentDamage an. |
| dat:validation.condition\_numberOfOwners.outOfRange | Zustand: Anzahl Besitzer außerhalb des gültigen Bereichs [0 - 15]. | Die Anzahl der Halter liegt außerhalb des gültigen Bereichs. Bitte geben Sie einen gültigen Wert für numberOfOwners an. |
| dat:validation.condition\_ownerCorrectionPercent.outOfRange | Zustand: Vorbesitzer-Wertkorrektur außerhalb des gültigen Bereichs [0.00 - 15.00]. | Die Wertkorrektur für die Anzahl der Vorbesitzer ist außerhalb des gültigen Bereichs. Bitte geben Sie einen gültigen Wert für ownerCorrectionPercent an. |
| dat:validation.LicenseNumber.length | Die maximale Zeichenlänge für Kennzeichen für das Datenland <Datenland> beträgt <Zahl> Zeichen. | Die maximale Zeichenlänge für das Kennzeichen LicenseNumber für das gewählte Datenland wurde überschritten. Bitte passen Sie den Parameter LicenseNumber an. |
| dat:validation.mileage.invalid | Laufleistung ist ungültig. | Der Parameter mileage liegt außerhalb des gültigen Bereichs. |
