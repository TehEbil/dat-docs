---
title: "Mögliche Fehlercodes createDossierN"
topic_id: "15014"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Erstellen eines neuen Vorgangs > Mögliche Fehlercodes createDossierN"
---

# Mögliche Fehlercodes createDossierN

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:validation.dossierElement.missing | Dossier-Element fehlt. | Es wurde kein Dossier-Element im Request angegeben. |
| dat:validation.vehicleElement.missing | Vehicle-Element fehlt. | Es wurde kein Vehicle-Element im Request angegeben. |
| dat:validation.country.missing | Land fehlt. | Der Parameter Vehicle.Country wurde nicht angegeben. |
| dat:validation.country.invalid | Land ungültig. | Der Parameter Vehicle.Country enthält einen ungültigen Wert. |
| dat:validation.language.missing | Sprache fehlt. | Der Parameter Language wurde nicht angegeben. |
| dat:validation.language.invalid | Sprache ungültig. | Der Parameter Language enthält einen ungültigen Wert. Evtl. ist auch die Kombination mit dem gespeicherten Wert für das Datenland (Country) ungültig. |
| dat:validation.datECode.missingOrIncomplete | DatECode (15-stellig) fehlt oder unvollständig. | Mindestens einer der Parameter Marktindex oder Bauzeit wurde angegeben (Fahrzeugneuidentifikation), jedoch der Parameter DatECode fehlt oder ist nicht 15 Stellen lang oder ist nicht rein numerisch. |
| dat:validation.datECode.invalid | DatECode ist nicht valide. | Bitte melden Sie diesen DAT €uropa-Code® an interfaces@dat.eu. |
| dat:validation.vehicleType.invalid | Fahrzeugart ungültig. | Die angegebene Fahrzeugart im DAT €uropa-Code® ist ungültig. |
| dat:validation.manufacturer.invalid | Fahrzeughersteller ungültig. | Der angegebene Fahrzeughersteller im DAT €uropa-Code® ist ungültig. |
| dat:validation.mainType.invalid | Fahrzeughaupttyp ungültig. | Der angegebene Fahrzeughaupttyp im DAT €uropa-Code® ist ungültig. |
| dat:validation.subType.invalid | Fahrzeuguntertyp ungültig. | Der angegebene Fahrzeuguntertyp im DAT €uropa-Code® ist ungültig. |
| dat:validation.subTypeVariant.invalid | Fahrzeuguntertypvariante ungültig. | Die angegebene Fahrzeuguntertypvariante im DAT €uropa-Code® ist ungültig. |
| dat:validation.container.missingOrIncomplete | Container fehlt oder unvollständig. | Mindestens einer der Parameter DatECode oder ConstructionTime wurde angegeben (Fahrzeugneuidentifikation), jedoch der Parameter Marktindex fehlt oder ist nicht 5 Zeichen lang. |
| dat:validation.container.invalid | Container ungültig. | Der Parameter Marktindex besteht nicht aus zwei Buchstaben gefolgt von drei alphanumerischen Zeichen. |
| dat:validation.container.invalidForDatECode | Container existiert nicht für DatECode. | Der Parameter Marktindex enthält einen ungültigen Wert für den angegebenen DAT €uropa-Code®. |
| dat:validation.constructionTime.missing | Bauzeit fehlt. | Mindestens einer der Parameter DatECode oder Marktindex Container wurde angegeben (Fahrzeugneuidentifikation), jedoch der Parameter ConstructionTime fehlt. |
| dat:validation.constructionTime.invalid | Bauzeit ungültig. | Der Parameter ConstructionTime liegt außerhalb des gültigen Bereichs. |
| dat:validation.constructionTime.invalidForContainer | Bauzeit ungültig für Container. | Der Parameter ConstructionTime enthält einen ungültigen Wert für den angegebenen Marktindex Container. |
| dat:validation.datEquipmentId.missing | DAT-Ausstattungsnummer fehlt. | In einem EquipmentPosition-Datensatz fehlt der Parameter DatEquipmentId. |
| dat:validation.datEquipmentId.invalid | DAT-Ausstattungsnummer ungültig. | In einem EquipmentPosition-Datensatz liegt der Parameter DatEquipmentId außerhalb des gültigen Bereichs. |
| dat:validation.decreaseType.invalid | Abwertungstyp ungültig. | In einem EquipmentPosition-Datensatz enthält der Parameter DecreaseType einen ungültigen Wert. |
| dat:validation.decreaseType.invalidVV | Abwertungstyp VV ist nur für Österreich gültig. | In einem EquipmentPosition-Datensatz enthält der Parameter DecreaseType den Wert VV, welcher nur für das Datenland Österreich angegeben werden kann. |
| dat:validation.additionalEquipment.invalid | Zusatzausstattungseinbaudatum darf nicht vor dem Erstzulassungsdatum liegen. | In einem EquipmentPosition-Datensatz ist der Parameter InstallDate ungültig, da er zeitlich vor dem Erstzulassungsdatum liegt. |
| dat:validation.valuationType.invalid | Bewertungstyp ungültig | Der Parameter ValuationType enthält einen ungültigen Wert. |
| dat:validation.valuationType.impossibleForDossierType | Bewertungstyp für vorhandenen Dossiertyp nicht möglich. | Der Parameter ValuationType enthält einen Wert, der mit dem angegebenen DossierType nicht kombinierbar ist. |
| dat:validation.initialRegistration.invalid | Erstzulassungsdatum ungültig. |  |
| dat:validation.initialRegistration.missing | Erstzulassungsdatum fehlt. | Der Parameter ValuationType wurde von NEW VEHICLE auf VALUATION geändert und der Parameter InitialRegistration wurde nicht angegeben (in diesem Fall erforderlich). |
| dat:validation.initialRegistration.afterDataMonth | Erstzulassungsdatum liegt nach Datenmonat/-jahr. | Der Parameter InitialRegistration enthält ein Datum, das nach dem aktuellen Datenstand liegt. |
| dat:validation.initialRegistration.tooFarFromConstructionTime | Differenz zwischen Baujahr und Zulassungsjahr ist größer 1. | Der Parameter InitialRegistration steht in Konflikt mit dem Parameter ConstructionTime, da sie zu weit auseinander liegen. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. |
| dat:validation.initialRegistrationToMarketIndex | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. | Der Parameter InitialRegistration steht in Konflikt mit dem Parameter ConstructionTime, da sie zu weit auseinander liegen. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. |
| dat:validation.mileage.missing | Kilometerstand fehlt. | Der ValuationType wurde von NEW VEHICLE auf VALUATION geändert und der Parameter MileageEstimated wurde nicht angegeben (in diesem Fall erforderlich). |
| dat:validation.mileage.invalid | Laufleistung ist ungültig | Der Parameter MileageEstimated liegt außerhalb des gültigen Bereichs. |
| dat:validation.valuation\_mileageCorrectionUser.outOfRange | Bewertung: Benutzereingabe für Laufleistungskorrektur außerhalb des gültigen Bereichs [-999999999.99 - 999999999.99]. | Die Benutzereingabe für die Laufleistungskorrektur liegt außerhalb des gültigen Bereichs. Bitte korrigieren Sie die Benutzereingabe für die Laufleistungskorrektur. |
| dat:validation.valuation\_firstRegistrationCorrectionUser.outOfRange | Bewertung: Benutzereingabe für Erstzulassungskorrektur außerhalb des gültigen Bereichs [999999999.99 - 999999999.99]. | Die Benutzereingabe für die Erstzulassungskorrektur liegt außerhalb des gültigen Bereichs. Bitte korrigieren Sie die Benutzereingabe für die Erstzulassungskorrektur. |
| S:Server | NOT\_EVALUABLE invalid mileage/+/39000/<Wert> | Das Fahrzeug kann nicht bewertet werden, weil die Laufleistung zu hoch ist. Eine Bewertung ist nur bis zu einer Laufleistung von <Wert> km möglich |
| S:Server | NOT\_EVALUABLE invalid mileage/-/<Wert>/1428000 | Das Fahrzeug kann nicht bewertet werden, weil die Laufleistung zu gering ist. Eine Bewertung ist erst ab einer Laufleistung von <Wert> km möglich |
| dat:validation.dossierType.invalid | Dossier-Typ ungültig. | Der Parameter DossierTyp enthält einen ungültigen Wert. |
| dat:validation.vatType.invalid | Besteuerungsart ungültig. | Die Differenzbesteuerung ist für Neufahrzeuge nicht zulässig. Bitte ändern Sie die die Besteuerungsart. |
| dat:validation.determinatedDate.missing | Bewertungsdatum fehlt. | Der Parameter DeterminatedDate fehlt und es wurde für DossierType der Wert HISTORIC EVALUATION angegeben. |
| dat:validation.determinatedDate.afterDataMonth | Bewertungsdatum liegt nach Datenmonat/-jahr. | Der Parameter DeterminatedDate enthält ein Datum, das nach dem aktuellen Datenstand liegt. |
| dat:validation.determinatedDate.beforeInitialRegistration | Bewertungsdatum liegt vor Erstzulassungsdatum. | Der Parameter DeterminatedDate enthält ein Datum, das vor dem Erstzulassungsdatum liegt. |
| dat:validation.determinatedDate.beforeMinimalDate | Bewertungsdatum liegt zu weit zurück. | Der Parameter DeterminatedDate enthält ein Datum, das vor dem Minimaldatum liegt. |
| dat:validation.forecast\_priceType.invalid | Restwertprognose Preisangabe ungültig. | Der Forecast-Parameter PriceType enthält einen ungültigen Wert. |
| dat:validation.forecast\_includeVat.invalid | Restwertprognose: Steuerkennzeichen ungültig. | Der Forecast-Parameter IncludeVat enthält einen ungültigen Wert. |
| dat:validation.forecast\_curveType.invalid | Restwertprognose: Abwertungskurve ungültig. | Der Forecast-Parameter CurveType enthält einen ungültigen Wert. |
| dat:validation.forecast\_decreaseType.invalid | Restwertprognose: Ausstattungsabwertung ungültig. | Der Forecast-Parameter DecreaseType enthält einen ungültigen Wert. |
| dat:validation.forecast\_valueType.invalid | Restwertprognose: Wertangabe ungültig. | Der Forecast-Parameter ValueType enthält einen ungültigen Wert. |
| dat:validation.forecast\_startType.invalid | Restwertprognose: Kennzeichen für Fahrzeugalter ungültig. | Der Forecast-Parameter StartType enthält einen ungültigen Wert. |
| dat:validation.forecast\_mileageType.invalid | Restwertprognose Laufleistungskennzeichen ungültig. | Der Forecast-Parameter MileageType enthält einen ungültigen Wert. |
| dat:validation.forecast\_months.missing | Restwertprognose-Datensatz: Fahrzeugalter fehlt. | In einem Forecast-Datensatz fehlt der Parameter Months. |
| dat:validation.forecast\_months.outOfRange | Restwertprognose-Datensatz: Fahrzeugalter außerhalb des gültigen Bereichs [X - Y] | In einem Forecast-Datensatz liegt der Parameter Months außerhalb des gültigen Bereichs (X=Minimum, Y=Maximum). |
| dat:validation.forecast\_mileageTotal.missing | Restwertprognose-Datensatz: Gesamtkilometerstand fehlt. | Der MileageType des Forecasts ist TOTAL und in einem Forecast-Datensatz fehlt der Parameter MileageTotal. |
| dat:validation.forecast\_mileagePerYear.missing | Restwertprognose-Datensatz: Jahreskilometerleistung fehlt. | Der MileageType des Forecasts ist YEAR und in einem Forecast-Datensatz fehlt der Parameter MileagePerYear. |
| dat:validation.condition\_increaseInValue.outOfRange | Zustand: Werterhöhung außerhalb des gültigen Bereichs [X - Y]. | Der Condition-Parameter IncreaseInValue liegt außerhalb des gültigen Bereichs (X=Minimum, Y=Maximum). |
| dat:validation.condition\_decreaseInValue.outOfRange | Zustand: Wertminderung außerhalb des gültigen Bereichs [X - Y]. | Der Condition-Parameter DecreaseInValue liegt außerhalb des gültigen Bereichs (X=Minimum, Y=Maximum). |
| dat:validation.condition\_tiresMountedValue.outOfRange | Zustand: Wertanpassung der montierten Bereifung außerhalb des gültigen Bereichs [X - Y]. | Der Condition-Parameter TiresMountedValue liegt außerhalb des gültigen Bereichs (X=Minimum, Y=Maximum). |
| dat:validation.condition\_tiresUnmountedValue.outOfRange | Zustand: Wert der unmontierten Bereifung außerhalb des gültigen Bereichs [X - Y]. | Der Condition-Parameter TiresUnmountedValue liegt außerhalb des gültigen Bereichs (X=Minimum, Y=Maximum). |
| dat:validation.condition\_repairCosts.outOfRange | Zustand: Reparaturkosten außerhalb des gültigen Bereichs [X - Y] | Der Condition-Parameter RepairCosts liegt außerhalb des gültigen Bereichs (X=Minimum, Y=Maximum). |
| dat:validation.condition\_accidentDamage.invalid | Zustand: Unfallkennzeichen ungültig. | Der Condition-Parameter AccidentDamage enthält einen ungültigen Wert. |
| dat:validation.condition\_numberOfOwners.outOfRange | Zustand: Anzahl Besitzer außerhalb des gültigen Bereichs [X - Y]. | Der Condition-Parameter NumberOfOwners liegt außerhalb des gültigen Bereichs (X=Minimum, Y=Maximum). |
| dat:validation.condition\_ownerCorrectionPerc.outOfRange | Zustand: Vorbesitzer-Wertkorrektur außerhalb des gültigen Bereichs [X - Y]. | Der Condition-Parameter OwnerCorrectionPerc liegt außerhalb des gültigen Bereichs (X=Minimum, Y=Maximum). |
| dat:validation.condition\_correctionFactorPerc.outOfRange | Zustand: Zustands-Wertkorrektur außerhalb des gültigen Bereichs [X - Y]. | Der Condition-Parameter ConditionFactorPercent liegt außerhalb des gültigen Bereichs (X=Minimum, Y=Maximum). |
| dat:validation.condition\_numberOfProprietors.outOfRange | Zustand: Anzahl Besitzer außerhalb des gültigen Bereichs [0 - 15]. | Der Wert für NumberOfProprietors ist außerhalb des gültigen Bereichs (0 = minimum, 15 = maximum). |
| dat:validation.upperBody.impossible | Aufbau für diese Fahrzeugart nicht möglich. | Es wurde das UpperBodies-Element angegeben, obwohl dies für die vorliegende Fahrzeugart nicht möglich ist. |
| dat:validation.upperBodyType.missing | Aufbau: Aufbauart fehlt. | Der Parameter UpperBodyType wurde nicht angegeben. |
| dat:validation.upperBodyType.invalid | Aufbau: Aufbauart ungültig. | Der Parameter UpperBodyType enthält einen ungültigen Wert. |
| dat:validation.upperBodyManufacturer.invalid | Aufbau: Hersteller ungültig. | Der Parameter UpperBody.Manufacturer enthält einen ungültigen Wert. |
| dat:validation.upperBodyMainType.missing | Aufbau: Haupttyp fehlt. | Der Parameter UpperBody.MainModel wurde nicht angegeben. |
| dat:validation.upperBodyMainType.invalid | Aufbau: Haupttyp ungültig. | Der Parameter UpperBody.MainModel enthält einen ungültigen Wert. |
| dat:validation.upperBodySubType.missing | Aufbau: Untertyp fehlt. | Der Parameter SubModel wurde nicht angegeben. |
| dat:validation.upperBodySubType.invalid | Aufbau: Untertyp ungültig. | Der Parameter SubModel enthält einen ungültigen Wert. |
| dat:validation.upperBodyInitialRegistration.missing | Aufbau: Erstzulassung fehlt. | Der Parameter UpperBody.InitialRegistration wurde nicht angegeben. |
| dat:validation.upperBodyInitialRegistration.invalid | Aufbau: Erstzulassung ungültig. | Der Parameter UpperBody.InitialRegistration enthält einen ungültigen Wert. |
| dat:validation.upperBodyCoolingUnit.impossible | Aufbau: Kühlaggregat für diese Aufbauart nicht möglich. | Es wurde das CoolingUnit-Element angegeben, obwohl dies für die vorliegende Aufbauart nicht möglich ist. |
| dat:validation.upperBodyCoolingUnitManufacturer.missing | Aufbau: Kühlaggregat-Hersteller fehlt. | Der Parameter CoolingUnit.Manufacturer wurde nicht angegeben. |
| dat:validation.upperBodyCoolingUnitManufacturer.invalid | Aufbau: Kühlaggregat-Hersteller ungültig. | Der Parameter CoolingUnit.Manufacturer enthält einen ungültigen Wert. |
| dat:validation.upperBodyCoolingUnitMainModel.missing | Aufbau: Kühlaggregat-Modell fehlt. | Der Parameter CoolingUnit.MainModel  wurde nicht angegeben. |
| dat:validation.upperBodyCoolingUnitMainModel.invalid | Aufbau: Kühlaggregat-Modell ungültig. | Der Parameter CoolingUnit.MainModel enthält einen ungültigen Wert. |
| dat:validation.upperBodyCoolingUnitInitialRegistration.missing | Aufbau: Erstzulassung des Kühlaggregats fehlt. | Der Parameter CoolingUnit.InitialRegistration wurde nicht angegeben. |
| dat:validation.upperBodyCoolingUnitInitialRegistration.invalid | Aufbau: Erstzulassung des Kühlaggregats ungültig. | Der Parameter CoolingUnit.InitialRegistration enthält einen ungültigen Wert. |
| dat:validation.upperBody\_decreaseType.missing | Aufbau-Ausstattung: Abwertungstyp fehlt. | Der Parameter DecreaseType der Aufbau-Ausstattung wurde nicht angegeben. |
| dat:validation.upperBody\_decreaseType.invalid | Aufbau-Ausstattung: Abwertungstyp ungültig. | Der Parameter DecreaseType der Aufau-Ausstattung enthält einen ungültigen Wert. |
| validation.upperBody\_decreaseType.invalidVV | Aufbau-Ausstattung: Abwertungstyp 'VV' ist nur für Österreich gültig. | Der Parameter DecreaseType der Aufbau-Ausstattung enthält den Wert VV, welcher nur für das Datenland Österreich gültig ist. |
| dat:validation.upperBody\_datEquipmentId.missing | Aufbau-Ausstattung: DAT-Ausstattungsnummer fehlt. | Der Parameter EquipmentId der Aufbau-Sonderausstattung wurde nicht angegeben. |
| dat:validation.upperBody\_datEquipmentId.invalid | Aufbau-Ausstattung: DAT-Ausstattungsnummer ungültig. | Der Parameter EquipmentId der Aufbau- Sonderausstattung enthält einen ungültigen Wert. |
| dat:validation.upperBody\_additionalEquipment.invalid | Aufbau-Ausstattung: Zusatzausstattungseinbaudatum darf nicht vor dem Erstzulassungsdatum liegen. | Der Parameter InstallDate der Aufbau- Sonderausstattung ist ungültig, da er zeitlich vor der Erstzulassung liegt. |
| dat:validation.upperBody\_condition\_accidentDamage.invalid | Aufbau-Zustand: Unfallkennzeichen ungültig. | Die Zustandsdaten in AccidentDamage wurden falsch angegeben. Bitte überprüfen Sie den Parameter AccidentDamage . |
| dat:validation.upperBody\_condition\_increaseInValue.outOfRange | Aufbau-Zustand: Werterhöhung außerhalb des gültigen Bereichs [0.00 - 999999999.99]. | Die Werterhöhung IncreaseInvalue liegt nicht zwischen 0.00 und 999999999.99. Bitte überprüfen Sie die Werterhöhung. |
| dat:validation.upperBody\_condition\_decreaseInValue.outOfRange | Aufbau-Zustand: Wertminderung außerhalb des gültigen Bereichs [0.00 - 999999999.99]. | Die Wertminderung DecreaseInValue liegt nicht zwischen 0.00 und 999999999.99. Btte überprüfen Sie die Wertminderung. |
| dat:validation.upperBody\_OriginalPrice.outOfRange | Es sind nur Werte zwischen 0.00 und 999999999.99 zulässig. | Für den Originalpreis sind nur Wertangaben zwischen 0.00 und 999999999.99 möglich. Bitte überprüfen Sie den Neupreis des Aufbaus. |
| dat:validation.upperBodyManufacturer.invalid | Aufbau: Hersteller ungültig. | Der Hersteller Manufacturer ist ungültig. |
| dat:Server.ManufacturerNotLicensed | manufacturer not licensed | Sie sind nicht berechtigt den angegebenen Hersteller abzufragen. Bitte wenden Sie sich an den DAT Vertrieb: sales-support@dat.de. |
| dat:validation.condition.noPermission | Keine Berechtigung zum Bearbeiten von Zustandsdaten. | Sie sind nicht berechtigt Zustandsdaten zu bearbeiten. |
| dat:validation.ManualEquipmentOrignalPrice.negative | Der manuelle Ausstattungsgesamtpreis darf nicht negativ sein. | Der manuelle Ausstattungsgesamtpreis darf nicht negativ sein. Bitte korrigieren Sie diesen Wert. |
| dat:validation.EquipmentPercentage.missing | Ein prozentualler Anteil ohne einen manuellen Ausstattungsgesamtpreis ist nicht zulässig. | Der prozentualle Anteil darf nur angegeben werden, wenn auch der manuelle Ausstattungsgesamtpreis angegeben wird. Bitte löschen Sie diese Vorgabe oder setzen Sie einen manuellen Ausstattungsgesamtpreis. |
| dat:validation.EquipmentDecreaseType.invalid | Die Abwertungsart für den ersten Anteil ohne einen manuellen Ausstattungsgesamtpreis ist nicht zulässig. | Die Abwertungsart für den ersten Anteil darf nur angegeben werden, wenn auch der manuelle Ausstattungsgesamtpreis angegeben wird. Bitte löschen Sie diese Vorgabe oder setzen Sie einen manuellen Ausstattungsgesamtpreis. |
| dat:validation.EquipmentDecreaseTypeRemaining.invalid | Die Abwertungsart für den restlichen Anteil ohne einen manuellen Ausstattungsgesamtpreis ist nicht zulässig. | Die Abwertungsart für den restlichen Anteil darf nur angegeben werden, wenn auch der manuelle Ausstattungsgesamtpreis angegeben wird. Bitte löschen Sie diese Vorgabe oder setzen Sie einen manuellen Ausstattungsgesamtpreis. |
| dat:validation.EquipmentPercentage.invalid | Der prozentuale Anteil ist ungültig. | Der prozentualle Anteil muss kleiner oder gleich 100 sein. Bitte korrigieren Sie diesen Wert. |
| dat:validation.EquipmentPrice.invalid | Ein manuelle Restwertvorgabe ist bei Vorgabe eines manuellen Ausstattungsgesamtpreises nicht zulässig. | Bei Vorgabe eines eines manuellen Ausstattungsgesamtpreises ist die Vorgabe eines manuellen Restwerts nicht zulässig. Bitte löschen Sie diese Vorgabe oder löschen Sie die manuellen Vorgaben zum Ausstattungsgesamtpreis. |
| dat:validation.additionalEquipment.invalid | Zusatzausstattungseinbaudatum darf nicht vor dem Erstzulassungsdatum liegen. | Das Zusatzausstattungeinbaudatum InstallDate liegt vor dem Erstzulassungsdatum. Bitte überprüfen Sie das Zusatzausstatungseinbaudatum. |
| dat:validation.DevaluationType.invalid | Abwertungstyp ungültig. | Ändern Sie den Abwertungstyp. Gültige Werte sind Residual value,T1,T2,T3,T4, DT, Percentage. |
| dat:validation.PercentageNumber.invalid | Prozentsatznummer ist ungültig. Bitte geben Sie eine Zahl zwischen 25 und -25 ein. | Der Prozentsatz liegt zwischen 25 und -25. |
| dat:validation.mileage.invalid | A valuation is only possible from a mileage of 56000 miles. | Bitte erhöhen Sie die Laufleistung. |
| dat:validation.futurePrognosis.dateInThePast | Die Zukunftsprognose ist für die Vergangenheit nicht möglich. | PrognosisDate muss in der Zukunft liegen. |
| dat:validation.futurePrognosis.dateInTheFuture | Die Zukunftsprognose ist nur bis max. {x} Monate in die Zukunft möglich. | Der Parameter PrognosisDate enthält ein Datum zu weit in der Zukunft. |
| dat:validation.futurePrognosis.dateInTheSameMonth | Die Zukunftsprognose ist im aktuellen Monat nicht möglich. | PrognosisDate darf nicht im aktuellen Monat liegen (alle anderen Datenländer). |
| dat:validation.futurePrognosis.userMileageInvalid | Die voraussichtliche Laufleistung darf nicht kleiner sein als die aktuell vorhandene. | Die voraussichtliche Laufleistung PrognosisMileageUser darf nicht kleiner sein, als die aktuelle Laufleistung. |
| dat:validation.Version.invalid | Der Parameter Valuation.Version enthält einen ungültigen Wert, zulässige Werte sind V1.1 oder leer. | Der Parameter Version enthält einen ungültigen Wert. |
| dat:validation.approval.message | Der ausgewählte Stichtag führt zu einer kostenpflichtigen rückwirkenden Bewertung. Soll die rückwirkende Bewertung tatsächlich durchgeführt werden? Freigabe mittels Approval-Wert = <HASH> | Wiederholen Sie die Abfrage und geben Sie zusätzlich den Parameter Approval an, wenn Sie den zusätzlichen Kosten zustimmen. |
| dat:validation.Approval.invalid | Der Parameter Approval enthält einen ungültigen Wert. | Bitte geben Sie einen gültigen Wert für Approval an. Bitte beachten Sie, dass der Wert für Approval nur eine Stunde gültig ist. |
| dat:validation.LicenseNumber.length | Die maximale Zeichenlänge für Kennzeichen für das Datenland <Datenland> beträgt <Zahl> Zeichen. | Die maximale Zeichenlänge für LicenseNumber für das ausgewählte Datenlandwurde überschritten. Bitte korrigieren Sie die Angabe für den Parameter LicenseNumber . |
| dat:validation.forecast\_vehicleAge.notDeterminable | Fahrzeugalter konnte nicht ermittelt werden. | Das Fahrzeugalter kann nicht ermittelt werden. |
| dat:validation.condition\_ConditionCorrectionDescription.invalid | Bitte geben Sie für ConditionCorrectionDescription einen kürzeren Text ein. Die maximale Zeichenlänge beträgt 40 Zeichen. | Die maximale Zeichenlänge für ConditionCorrectionDescription beträgt 40 Zeichen. Bitte geben Sie einen kürzeren Text ein. |
| dat:validation.forecast\_vehicleAge.outOfRange | Eine Restwertprognose ist nicht mehr möglich, weil das Fahrzeugalter bereits 72 Monate oder mehr beträgt. | Eine Restwertprognose kann nur bis zu einem Fahrzeugalter von 72 Monaten durchgeführt werden. |
| dat:validation.futurePrognosis.disabled | Die Zukunftsprognose ist in den Benutzereinstellungen deaktiviert. | Die Zukunftsprognose ist nicht möglich, da sie in den Benutzereinstellungen deaktiviert ist. |
| dat:validation.tires\_originalPrice.mounted.invalid | Der Reifenneupreis für montierte Reifen ist ungültig: Achse <AxleNo>. | Bitte geben Sie einen gültigen Wert für TireOriginalPrice unter Axle für die entsprechende Achse an. |
| dat:validation.tires\_originalPrice.unmounted.invalid | Der Reifenneupreis für unmontierte Reifen ist ungültig: Achse <AxleNo>. | Bitte geben Sie einen gültigen Wert für TireOriginalPrice unter Axle für die entsprechende Achse an. |
| dat:validation.tires\_originalPrice.spareWheel.invalid | Der Reifenneupreis für das Ersatzrad ist ungültig. | Bitte geben Sie einen gültigen Wert für TireOriginalPrice unter Axle für die entsprechende Achse an. |
| dat:validation.tires\_originalPrice.mounted.missing | Der Reifenneupreis für montierte Reifen fehlt: Achse <AxleNo>. | Bitte geben Sie einen gültigen Wert für TireOriginalPrice unter Axle für die entsprechende Achse an. |
| dat:validation.tires\_originalPrice.unmounted.missing | Der Reifenneupreis für unmontierte Reifen fehlt: Achse <AxleNo>. | Bitte geben Sie einen gültigen Wert für TireOriginalPrice unter Axle für die entsprechende Achse an. |
| dat:validation.tires\_originalPrice.spareWheel.missing | Der Reifenneupreis für das Ersatzrad fehlt. | Bitte geben Sie einen gültigen Wert für TireOriginalPrice unter Axle für die entsprechende Achse an. |
| dat:validation.upperBody\_PaintLabelDescription.invalid | Bitte geben Sie für PaintLabelDescription einen kürzeren Text ein. Die maximale Zeichenlänge beträgt 200 Zeichen. | Die angegebene Beschreibung des Aufbaus ist länger als 200 Zeichen. Bitte geben Sie einen kürzeren Text für PaintLabelDescription unter UpperBody an. |
| dat:validation.condition\_commentDecreaseInValue.invalid | Bitte geben Sie für CommentDecreaseInValue einen kürzeren Text ein. Die maximale Zeichenlänge beträgt 200 Zeichen. | Der angegebene Kommentar zur Wertminderung ist länger als 200 Zeichen. Bitte geben Sie einen kürzeren Text für CommentDecreaseInValue unter Condition an. |
| dat:validation.condition\_commentIncreaseInValue.invalid | Bitte geben Sie für CommentIncreaseInValue einen kürzeren Text ein. Die maximale Zeichenlänge beträgt 200 Zeichen. | Der angegebene Kommentar zur Werterhöhung ist länger als 200 Zeichen. Bitte geben Sie einen kürzeren Text für CommentIncreaseInValue unter Condition an. |
| dat:validation.condition\_commentRepairCosts.invalid | Bitte geben Sie für CommentRepairCosts einen kürzeren Text ein. Die maximale Zeichenlänge beträgt 200 Zeichen. | Der angegebene Kommentar zu den Reperaturkosten ist länger als 200 Zeichen. Bitte geben Sie einen kürzeren Text für CommentRepairCosts unter Condition an. |

Mögliche Warnmeldungen createDossierN

Unter Umständen kann es beim Anlegen einer Bewertung für einen Lastkraftwagen dazu
kommen, dass die Bewertung des Fahrzeugs und bzw. oder von Ausstattungen nicht möglich
ist. In solchen Fällen wird in der Response zukünftig im Element <Valuation> unter <Warning> eine der folgenden Warnmeldungen ausgegeben:

| Problem | Warnmeldung |
| --- | --- |
| Fahrzeug und Ausstattungen können nicht bewertet werden | Das gewählte Fahrzeug kann nicht mit den Daten der DAT Marktbeobachtung bewertet werden, es ist nur eine manuelle Fahrzeugbewertung über Wertvorgaben durch den Anwender möglich. Zur Bewertung des Fahrzeugs ist die Angabe des Parameters BasePrice2 unter Valuation zwingend notwendig. Dies betrifft aufgrund von fehlenden Herstellerangaben auch die Bewertung von Sonderausstattungen. Die Ausstattungswertermittlung kann nur über manuelle Wertvorgaben durch den Benutzer erfolgen. |
| Ausstattungen können nicht bewertet werden | Aufgrund von fehlenden Neupreisinformationen des Herstellers kann keine Ausstattungswertermittlung nach DAT erfolgen. Die Ausstattungswertermittlung kann nur über manuelle Wertvorgaben durch den Benutzer erfolgen. |
