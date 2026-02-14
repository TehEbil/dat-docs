---
title: "Mögliche Fehlercodes getNewContracts"
topic_id: "2149"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Methodenüberblick > Methoden > Mengen-Abruf von Kalkulationen mit getNewContracts > Mögliche Fehlercodes getNewContracts"
---

# Mögliche Fehlercodes getNewContracts

Die folgende Liste enthält eine Beschreibung der Fehlermeldungen, die beim Aufruf
der dokumentierten Funktionen auftreten können. Die hier erläuterten Fehler-Codes
beziehen sich auf die in diesem Dokument beschriebenen Funktionen. Bitte beachten
Sie daher auch das Kapitel [Notwendige Login-Informationen](#showid/1578 "Notwendige Informationen"), das sich unter anderem auch mit Fehlern der Authentifizierung beschäftigt.

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| internalError | Cannot create Contract. required: [datCustomerId ] | Bitte prüfen Sie Ihre Session. Entweder ist sie abgelaufen oder Ihre Anmeldedaten sind nicht gültig. |
| requireCode | Input does not contain all required fields. [field] missing | Bitte prüfen Sie, ob alle notwendigen Felder übergeben wurden. |
| authorizationFailed | authorizationFailed | Bitte prüfen Sie Ihre Anmeldedaten und Ihre Signatur. |
| requireCode | Input does not contain order number. Unable to import | Die Order-Nr. muß zwingend mit übergeben werden. |
| wrongValueCode | Order number contained in input is already in use. | Die übergebene OrderID wird schon verwendet. |
| requireCode | No valid input found to import. | Bitte prüfen Sie die übergebenen Daten. |
| wrongValueCode | No vxd given for createContract. | Es fehlt die Anlage. |
| wrongValueCode | Input contains invalid insurance data. | Bitte prüfen Sie die Versicherungs-Nr. |
