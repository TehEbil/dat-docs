---
title: "Mögliche Fehlercodes getRentalOffersbyVIN"
topic_id: "7737"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenpreise anhand der VIN und PLZ ermitteln > Mögliche Fehlercodes getRentalOffersbyVIN"
---

# Mögliche Fehlercodes getRentalOffersbyVIN

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:Server.internalError | ECode not found | Bitte melden Sie diese Fahrgestellnummer an interfaces@dat.eu. |
| dat:validation.duration.invalid | Die Mietdauer stimmt nicht mit dem Beginn und dem Ende der Vermietung überein oder ist falsch. Bitte korrigieren Sie die Mietdauer. | Die Mietdauer stimmt nicht mit dem Beginn und dem Ende der Vermietung überein oder ist falsch. Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie die Dauer der Vermietung. |
| dat:validation.duration.outOfRange | Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie die Dauer der Vermietung. | Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie die Dauer der Vermietung. |
| dat:validation.initialRegistrationToMarketIndex | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. |
| dat:validation.firstRegistration.invalid | Erstzulassung fehlt oder ist ungültig | Das Erstzulassungsdatum ist falsch oder fehlt. Bitte korrigieren Sie das Datum der Erstzulassung. |
| dat:validation.noDataFound | Keine Daten vorhanden. | In der Datenbank liegen für diese Kombination aus DAT €uropa-Code® und Mietdauer leider keine Daten vor. |
| dat:validation.postalCode.invalid | Die Postleitzahl fehlt oder ist ungültig. Bitte korrigieren Sie die Postleitzahl. | Die Postleitzahl fehlt oder ist ungültig. Bitte korrigieren Sie die Postleitzahl. |
| dat:validation.postalCode.length | Die Postleitzahl ist zu lang oder zu kurz. Bitte korrigieren Sie die Postleitzahl. | Die Postleitzahl ist zu lang oder zu kurz. Bitte korrigieren Sie die Postleitzahl. |
| dat:validation.radius.outOfRange | Der Radius ist ungültig. Bitte korrigieren Sie den Radius. | Der Radius ist ungültig. Der Radius muss zwischen 1 und 40 liegen. Bitte korrigieren Sie den Radius. |
| dat:validation.rentalDuration.invalid | Beginndatum und Enddatum der Vermietung sind ungültig.  Bitte korrigieren Sie Beginndatum und Enddatum der Vermietung. | Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie Beginndatum und Enddatum der Vermietung. |
| dat:validation.vin.invalid | VIN-Wert fehlt oder ist ungültig | Die Fahrzeug-Identifizierungsnummer ist nicht gültig (Länge, ungültige Zeichen). Bitte korrigieren Sie die Fahrzeug-Identifizierungsnummer. |
| dat:validation.vin.length | Die Länge der VIN ist zu kurz oder zu lang. Bitte korrigieren Sie die VIN. | Die Länge der Fahrzeug-Identifizierungsnummer ist zu kurz oder zu lang. Bitte korrigieren Sie die Fahrzeug-Identifizierungsnummer. |
| dat:validation.vin.noCardata | Leider können wir Ihnen für die abgefragte Fahrgestellnummer keine Fahrzeugdaten über die VIN-Abfrage anbieten. | Leider können wir Ihnen für die abgefragte Fahrgestellnummer keine Fahrzeugdaten über die VIN-Abfrage anbieten. |
| dat:validation.vin.noSpecialCharacter | VIN-Wert darf keine Sonderzeichen oder Leerzeichen beinhalten. Bitte korrigieren Sie die VIN. | Die Fahrzeug-Identifizierungsnummer darf keine Sonderzeichen oder Leerzeichen beinhalten. Bitte korrigieren Sie die Fahrzeug-Identifizierungsnummer. |
