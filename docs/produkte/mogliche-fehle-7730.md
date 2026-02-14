---
title: "Mögliche Fehlercodes getLossOfUseDatabyDATECode"
topic_id: "7730"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Nutzungsausfalldaten anhand DAT €uropa-Code® ermitteln > Mögliche Fehlercodes getLossOfUseDatabyDATECode"
---

# Mögliche Fehlercodes getLossOfUseDatabyDATECode

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:Server.internalError | wrong ECode | Der DAT €uropa-Code® ist falsch oder unvollständig. Bitte überprüfen Sie 20stellige Kombination aus DAT €uropa-Code® und Marktindex. |
| dat:validation.eCode.container.invalid | DateCode beinhaltet einen falschen Container. Bitte korrigieren Sie den DateCode. | Der DAT €uropa-Code® beinhaltet einen Container-Wert zum Beispiel „DE002". Dieser Wert ist falsch. Bitte korrigieren Sie den DAT €uropa-Code®. |
| dat:validation.eCode.invalid | ECode fehlt oder ist ungültig | Der DAT €uropa-Code® fehlt oder ist ungültig. Bitte korrigieren Sie den DAT €uropa-Code®. |
| dat:validation.eCode.invalidFormat | ECode hat ein schlechtes Format | Das Format des DAT €uropa-Code® ist falsch. Bitte überprüfen Sie 20stellige Kombination aus DAT €uropa-Code® und Marktindex. |
| dat:validation.eCode.length | Die Länge der DateCode ist zu kurz oder zu lang. Bitte korrigieren Sie den DateCode. | Die Länge des DAT €uropa-Code® ist zu kurz oder zu lang. Bitte korrigieren Sie den DAT €uropa-Code®. |
| dat:validation.eCode.noSpecialCharacter | DateCode beinhaltet keine Sonderzeichen und Leerzeichen. Bitte korrigieren Sie den DateCode. | DAT €uropa-Code® beinhaltet keine Sonderzeichen und Leerzeichen. Bitte korrigieren Sie den DAT €uropa-Code®. |
| dat:validation.initialRegistrationToMarketIndex | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. | Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex ist größer als 1 Jahr. In der Fahrzeugbewertung kann in diesem Fall kein Wert ermittelt werden. Bitte nehmen Sie eine Korrektur an der Erstzulassung oder am Marktindex vor. |
| dat:validation.firstRegistration.invalid | Erstzulassung fehlt oder ist ungültig | Das Datum der Erstzulassung ist falsch oder fehlt. Bitte korrigieren Sie das Datum der Erstzulassung. |
| dat:validation.noDataFound | Keine Daten vorhanden. | In der Datenbank liegen für diese Kombination aus DAT €uropa-Code® und Mietdauer keine Daten vor. |
| dat:validation.rentalDuration.invalid | Beginndatum und Enddatum der Vermietung sind ungültig.  Bitte korrigieren Sie Beginndatum und Enddatum der Vermietung. | Die Dauer der Vermietung darf nicht länger als 30 Tage und nicht negativ sein. Bitte korrigieren Sie Beginn-Datum und End-Datum der Vermietung. |
