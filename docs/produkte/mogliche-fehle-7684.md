---
title: "Mögliche Fehlercodes getRentalCarClassbyVIN"
topic_id: "7684"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenklasse anhand der VIN ermitteln > Mögliche Fehlercodes getRentalCarClassbyVIN"
---

# Mögliche Fehlercodes getRentalCarClassbyVIN

| Return code | Error text | Description |
| --- | --- | --- |
| dat:Server.internalError | ECode not found | Bitte schreiben Sie eine Email an interfaces@dat.eu. |
| dat:validation.firstRegistration.invalid | Erstzulassung fehlt oder ist ungültig | Die Erstzulassung ist ungültig oder fehlt. Bitte geben Sie eine korrekte Erstzulassung an. |
| dat:validation.initialRegistrationToMarketIndex | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. |
| dat:validation.vin.invalid | VIN-Wert fehlt oder ist ungültig | VIN ist ungültig. Bitte geben Sie eine korrekte VIN ein |
| dat:validation.vin.length | VIN-Wert fehlt oder ist ungültig | VIN ist ungültig. Die Länge von der VIN ist zu lang oder zu kurz. Bitte geben Sie eine korrekte VIN ein. |
| dat:validation.vin.noCardata | Leider können wir Ihnen für die abgefragte Fahrgestellnummer keine Fahrzeugdaten über die VIN-Abfrage anbieten. | Leider können wir Ihnen für die abgefragte Fahrgestellnummer keine Fahrzeugdaten über die VIN-Abfrage anbieten. |
| dat:validation.vin.noECode | VIN beinhaltet keinen ECode. Bitte korrigieren Sie die VIN. | Bitte geben Sie eine korrekte VIN ein. |
| dat:validation.vin.noSpecialCharacter | VIN beinhaltet keine Sonderzeichen und Leerzeichen. Bitte korrigieren Sie die VIN. | Die VIN darf keine Sonderzeichen und Leerzeichen enthalten. Bitte geben Sie eine korrekte VIN ein. |
| dat:validation.noDataFound | Keine Daten vorhanden. | Für das angegebene Fahrzeug liegen keine Daten vor. |
