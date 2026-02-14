---
title: "Mögliche Fehlercodes MarketDataFromVXS"
topic_id: "16902"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Börsendaten via webScan REST-API abrufen > Funktionsumfang webScan > Mögliche Fehlercodes MarketDataFromVXS"
---

# Mögliche Fehlercodes MarketDataFromVXS

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
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
| dat:validation.initialRegistration.invalid | Erstzulassungsdatum ungültig. | Der Parameter InitialRegistration ist ungültig. Geben Sie das Datum im folgendem Format an: JJJJ-MM-TT. |
| dat:validation.initialRegistration.missing | Erstzulassungsdatum fehlt. | InitialRegistration wurde nicht angegeben. |
| dat:validation.initialRegistration.afterDataMonth | Erstzulassungsdatum liegt nach Datenmonat/-jahr. | Der Parameter InitialRegistration enthält ein Datum, das nach dem aktuellen Datenstand liegt. |
| dat:validation.initialRegistration.InFuture | Erstzulassungsdatum liegt in der Zukunft | Der Parameter InitialRegistration enthält ein Datum, das in der Zukunft liegt. |
| dat:validation.initialRegistrationToMarketIndex | Erstzulassungsdatum liegt nicht + oder - ein Jahr zur Bauzeit | Die Differenz der Erstzulassung zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. |
| dat:validation.mileage.missing | Kilometerstand fehlt. | MileageEstimated wurde nicht angegeben. |
| dat:validation.mileage.invalid | Laufleistung ist ungültig | Der Parameter MileageEstimated liegt außerhalb des gültigen Bereichs. |
| dat:validation.webscan2.notLicensed | Für diese Funktion liegt keine Lizenzierung vor. | Die webScan Funktionalität ist für die Kundennummer nicht lizenziert. |
