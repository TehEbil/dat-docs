---
title: "Mögliche Fehlercodes getLossOfUseDatabyVIN"
topic_id: "7726"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Nutzungsausfalldaten anhand der VIN ermitteln > Mögliche Fehlercodes getLossOfUseDatabyVIN"
---

# Mögliche Fehlercodes getLossOfUseDatabyVIN

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:Server.internalError | ECode not found | Bitte melden Sie diese Fahrgestellnummer an interfaces@dat.eu. |
| dat:validation.endOfRental.ErrorInthefuture | Zwischen dem Enddatum der Vermietung und der der Erstzulassung dürfen maximal 40 Jahre liegen. Das Enddatum der Vermietung liegt in der Zukunft. Bitte korrigieren Sie das Enddatum der Vermietung. | Zwischen dem Enddatum der Vermietung und der der Erstzulassung dürfen maximal 40 Jahre liegen. Das Enddatum der Vermietung liegt in der Zukunft. Bitte korrigieren Sie das Enddatum der Vermietung. |
| dat:validation.initialRegistrationToMarketIndex | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. |
| dat:validation.firstRegistration.invalid | Erstzulassung fehlt oder ist ungültig | Das Erstzulassungsdatum ist falsch oder fehlt. Bitte korrigieren Sie das Datum der Erstzulassung. |
| dat:validation.noDataFound | Keine Daten vorhanden. | In der Datenbank liegen für diese Kombination aus DAT €uropa-Code® und Mietdauer leider keine Daten vor. |
| dat:validation.rentalDuration.invalid | Beginndatum und Enddatum der Vermietung sind ungültig.  Bitte korrigieren Sie Beginndatum und Enddatum der Vermietung. | Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie Beginndatum und Enddatum der Vermietung. |
| dat:validation.vin.invalid | VIN-Wert fehlt oder ist ungültig | Die Fahrzeug-Identifizierungsnummer ist nicht gültig (Länge, ungültige Zeichen). Bitte korrigieren Sie die Fahrzeug-Identifizierungsnummer. |
| dat:validation.vin.length | Die Länge der VIN ist zu kurz oder zu lang. Bitte korrigieren Sie die VIN. | Die Länge der Fahrzeug-Identifizierungsnummer ist zu kurz oder zu lang. Bitte korrigieren Sie die Fahrzeug-Identifizierungsnummer. |
| dat:validation.vin.noCardata | Leider können wir Ihnen für die abgefragte Fahrgestellnummer keine Fahrzeugdaten über die VIN-Abfrage anbieten. | Leider können wir Ihnen für die abgefragte Fahrgestellnummer keine Fahrzeugdaten über die VIN-Abfrage anbieten. |
| dat:validation.vin.noECode | VIN beinhaltet keinen ECode. Bitte korrigieren Sie die VIN. | Die Fahrzeug-Identifizierungsnummer beinhaltet keinen gültigen DAT €uropa-Code®. Bitte korrigieren Sie die Fahrzeug-Identifizierungsnummer. |
| dat:validation.vin.noSpecialCharacter | VIN-Wert darf keine Sonderzeichen oder Leerzeichen beinhalten. Bitte korrigieren Sie die VIN. | Die Fahrzeug-Identifizierungsnummer darf keine Sonderzeichen oder Leerzeichen beinhalten. Bitte korrigieren Sie die Fahrzeug-Identifizierungsnummer. |
| dat:validation.noDataFound | Keine Daten vorhanden. | Für das angegebene Fahrzeug liegen keine Daten vor. |
