---
title: "Mögliche Fehlercodes createContract"
topic_id: "2120"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Methodenüberblick > Methoden > automatische Erzeugung eines Vorgangs mit createContract > Mögliche Fehlercodes createContract"
---

# Mögliche Fehlercodes createContract

Die folgende Liste enthält eine Beschreibung der Fehlermeldungen, die beim Aufruf
der dokumentierten Funktionen auftreten können. Die hier erläuterten Fehler-Codes
beziehen sich auf die in diesem Dokument beschriebenen Funktionen. Bitte beachten
Sie daher auch das Kapitel [Notwendige Login-Informationen](../../../allgemein/dat-developers-guide/authentifizierung-de/notwendige-inf-1578.md), das sich unter anderem auch mit Fehlern der Authentifizierung beschäftigt.

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| internalError | Cannot create Contract. required: [datCustomerId] | Bitte prüfen Sie Ihre Session. Entweder ist sie abgelaufen oder Ihre Anmeldedaten sind nicht gültig. |
| requireCode | Input does not contain all required fields. [field] missing | Bitte prüfen Sie, ob alle notwendigen Felder übergeben wurden. |
| authorizationFailed | authorizationFailed | Bitte prüfen Sie Ihre Anmeldedaten und Ihre Signatur. |
| requireCode | Input does not contain order number. Unable to import | Die Order-Nr. muß zwingend mit übergeben werden. |
| wrongValueCode | Order number contained in input is already in use. | Die übergebene OrderID wird schon verwendet. |
| requireCode | No valid input found to import. | Bitte prüfen Sie die übergebenen Daten. |
| wrongValueCode | No vxd given for createContract. | Es fehlt die Anlage. |
| wrongValueCode | Input contains invalid insurance data. | Bitte prüfen Sie die Versicherungs-Nr. |
| wrongValueCode | User has no permissions for type <parameter> | Bitte prüfen Sie das Attribut 'type' in Element 'Dossiers'. Es enthält eine ungültige Variante. |
