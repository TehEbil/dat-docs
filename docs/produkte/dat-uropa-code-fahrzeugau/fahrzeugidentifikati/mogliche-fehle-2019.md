---
title: "Mögliche Fehlercodes getVehicleTranslation"
topic_id: "2019"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation in mehreren Sprachen > Mögliche Fehlercodes getVehicleTranslation"
---

# Mögliche Fehlercodes getVehicleTranslation

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| valueNotFound | ECode not found | Bitte überprüfen Sie den DAT €uropa-Code. Er ist nicht gültig. |
| valueNotFound | ECode not found for this construction time | Bitte prüfen Sie die Bauzeit zum übergebenen DAT €uropa-Code; diese Kombination liefert kein gültiges Ergebnis. |
| wrongValueCode | LocaleError | Bitte prüfen Sie den Parameter "locale", er enthält ungültige Attributwerte. |
| Server | country-language-combination [it-de] not supported. | Bitte prüfen Sie die Sprachkombination im Parameter locale. Sie haben eine ungültige Sprachkombination übergeben. |
| valueNotFound | invalid language: ..... (format xx\_YY expected, e.g. en\_US) | Bitte prüfen Sie die Sprachkombination im Parameter language. Sie haben eine ungültige Sprachkombination übergeben. |
