---
title: "Mögliche Fehlercodes exportRentalOffers"
topic_id: "16471"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenprotokoll erstellen > Mögliche Fehlercodes exportRentalOffers"
---

# Mögliche Fehlercodes exportRentalOffers

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:validation.ExportProduct.missingOrInvalid | ExportProduct fehlt oder ist ungültig. | Bitte geben Sie die Bezeichnung des Reports an. |
| dat:validation.eCode.container.invalid | DateCode beinhaltet einen falschen Container.Bitte korrigieren Sie den Container des DateCodes. | Der DAT €uropa-Code® beinhaltet einen falschen Container. Bitte korrigieren Sie den Container des DAT €uropa-Code®. |
| dat:validation.rentalCarClass.outOfRange | Der Mietwagenklasse ist ungültig. Bitte korrigieren Sie die Mietwagenklasse. | Der Mietwagenklasse ist ungültig. Bitte korrigieren Sie die Mietwagenklasse. |
| dat:validation.vin.noCardata | Leider können wir Ihnen für die abgefragte Fahrgestellnummer keine Fahrzeugdaten über die VIN-Abfrage anbieten. | Leider können wir Ihnen für die abgefragte Fahrgestellnummer keine Fahrzeugdaten über die VIN-Abfrage anbieten. |
| dat:validation.firstRegistration.invalid | Erstzulassung fehlt oder ist ungültig | Die Erstzulassung ist ungültig oder fehlt. Bitte geben Sie eine korrekte Erstzulassung an. |
| dat:validation.firstRegistration.inthefuture | Die Erstzulassung liegt zu weit in der Zukunft. Bitte korrigieren Sie die Erstzulassung. | Erstzulassung darf maximal ein Jahr nach der Bauzeit liegen und darf nicht über das heutige Datum gesetzt werden. Bitte korrigieren Sie die Erstzulassung. |
| dat:validation.rentalDuration.invalid | Beginndatum und Enddatum der Vermietung sind ungültig.  Bitte korrigieren Sie Beginndatum und Enddatum der Vermietung. | Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie Beginn-Datum und End-Datum der Vermietung. |
| dat:validation.postalCode.length | Die Postleitzahl ist zu lang oder zu kurz. Bitte korrigieren Sie die Postleitzahl. | Die Postleitzahl ist zu lang oder zu kurz. Bitte korrigieren Sie die Postleitzahl. |
| dat:validation.duration.invalid | Die Mietdauer stimmt nicht mit dem Beginn und dem Ende der Vermietung überein. Bitte korrigieren Sie die Mietdauer. | Die Mietdauer stimmt nicht mit dem Beginn und dem Ende der Vermietung überein. Bitte korrigieren Sie die Mietdauer. |
| dat:validation.radius.outOfRange | Der Radius ist ungültig. Bitte korrigieren Sie den Radius. | Der Radius ist ungültig. Der Radius muss zwischen 1 und 40 liegen. Bitte korrigieren Sie den Radius. |
| dat:validation.SpecificConditionAndRentalOptionsCombination.invalid | Rental options sind nur zulässig, wenn specificConditions aktiviert ist. | Mietoptionen können nur angegeben werden, wenn der Wert für specificConditions true ist. |
