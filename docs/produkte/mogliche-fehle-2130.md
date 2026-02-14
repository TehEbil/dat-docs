---
title: "Mögliche Fehlercodes getContract"
topic_id: "2130"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Methodenüberblick > Methoden > Abrufen eines einzelnen Vorgangs mit getContract > Mögliche Fehlercodes getContract"
---

# Mögliche Fehlercodes getContract

Die folgende Liste enthält eine Beschreibung der Fehlermeldungen, die beim Aufruf
der dokumentierten Funktionen auftreten können. Die hier erläuterten Fehler-Codes
beziehen sich auf die in diesem Dokument beschriebenen Funktionen. Bitte beachten
Sie daher auch das Kapitel [Notwendige Login-Informationen](#showid/1578 "Notwendige Informationen"), das sich unter anderem auch mit Fehlern der Authentifizierung beschäftigt.

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| internalError | Cannot create Contract. required: [datCustomerId ] | Bitte prüfen Sie Ihre Session. Entweder ist sie abgelaufen oder Ihre Anmeldedaten sind nicht gültig. |
| requireCode | Input does not contain all required fields. [field] missing | Bitte prüfen Sie, ob die Auftragsnr. übergeben wurde. |
| authorizationFailed | authorizationFailed | Bitte prüfen Sie Ihre Session-Cookies. Sie wurden nicht ordnungsgemäß übergeben. |
| requireCode | Input does not contain order number. Unable to import | Die Order-Nr. muß zwingend übergeben werden. |
| wrongValueCode | Order number contained in input is already in use. | Die übergebene OrderID wird schon verwendet oder es fehlt die OrderID. |
| contractNotFound | Contract not found. | Diese Auftragsnummer existiert nicht. |
| contractHasNoCalculation | w.v. | Diese Auftragsnummer hat keine gültige Kalkulation. |
