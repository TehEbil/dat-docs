---
title: "Mögliche Fehlercodes getRentalOffersbyDATECode"
topic_id: "7738"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenpreise anhand des DAT €uropa-Code® und PLZ ermitteln > Mögliche Fehlercodes getRentalOffersbyDATECode"
---

# Mögliche Fehlercodes getRentalOffersbyDATECode

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:Server.internalError | wrong ECode | Der DAT €uropa-Code® ist falsch oder unvollständig. Bitte überprüfen Sie 20stellige Kombination aus DAT €uropa-Code® und Marktindex. |
| dat:validation.beginningofRental.tooFarInFuture | Nach der Erstzulassung dürfen maximal 50 Jahre vergehen, in diesem Zeitraum kann die Vermietung stattfinden.  Bitte korrigieren Sie Beginndatum und Enddatum der Vermietung. | Nach der Erstzulassung dürfen maximal 50 Jahre vergehen, in diesem Zeitraum kann die Vermietung stattfinden.  Bitte korrigieren Sie Beginn-Datum und End-Datum der Vermietung. |
| dat:validation.duration.invalid | Die Mietdauer stimmt nicht mit dem Beginn und dem Ende der Vermietung überein oder ist falsch. Bitte korrigieren Sie die Mietdauer. | Die Mietdauer stimmt nicht mit dem Beginn und dem Ende der Vermietung überein oder ist falsch. Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie die Dauer der Vermietung. |
| dat:validation.duration.outOfRange | Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie die Dauer der Vermietung. | Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie die Dauer der Vermietung. |
| dat:validation.eCode.invalid | ECode fehlt oder ist ungültig | Das Format des DAT €uropa-Code® ist falsch. Bitte überprüfen Sie 20stellige Kombination aus DAT €uropa-Code® und Marktindex. |
| dat:validation.eCode.invalidFormat | ECode hat ein schlechtes Format | Das Format des DAT €uropa-Code® ist falsch. Bitte überprüfen Sie 20stellige Kombination aus DAT €uropa-Code® und Marktindex. |
| dat:validation.eCode.length | Die Länge des DateCodes ist zu kurz oder zu lang. Bitte korrigieren Sie den DateCode. | Das Format des DAT €uropa-Code® ist falsch. Bitte überprüfen Sie 20stellige Kombination aus DAT €uropa-Code® und Marktindex |
| dat:validation.initialRegistrationToMarketIndex | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. |
| dat:validation.firstRegistration.invalid | Erstzulassung fehlt oder ist ungültig | Das Datum der Erstzulassung ist falsch oder fehlt. Bitte korrigieren Sie das Datum der Erstzulassung. |
| dat:validation.noDataFound | Keine Daten vorhanden. | In der Datenbank liegen für diese Kombination aus DAT €uropa-Code® und Mietdauer keine Daten vor. |
| dat:validation.postalCode.invalid | Die Postleitzahl fehlt oder ist ungültig. Bitte korrigieren Sie die Postleitzahl. | Die Postleitzahl fehlt oder ist ungültig. Bitte korrigieren Sie die Postleitzahl. |
| dat:validation.postalCode.length | Die Postleitzahl ist zu lang oder zu kurz. Bitte korrigieren Sie die Postleitzahl. | Die Postleitzahl ist zu lang oder zu kurz. Bitte korrigieren Sie die Postleitzahl. |
| dat:validation.radius.outOfRange | Der Radius ist ungültig. Bitte korrigieren Sie den Radius. | Der Radius ist ungültig. Der Radius muss zwischen 1 und 40 liegen. Bitte korrigieren Sie den Radius. |
| dat:validation.rentalDuration.invalid | Beginndatum und Enddatum der Vermietung sind ungültig.  Bitte korrigieren Sie Beginndatum und Enddatum der Vermietung. | Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie Beginn-Datum und End-Datum der Vermietung. |
