---
title: "Zugriff von einem anderen (Micro-)Service aus"
topic_id: "27902"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Anmeldung > Zugriff von einem anderen (Micro-)Service aus"
---

# Zugriff von einem anderen (Micro-)Service aus

Vor dem Zugriff auf jedwede Funktion zur Datenabfrage muss der Benutzer sich mittels
eines Aufrufs der Login-Funktion berechtigen. Diese Funktion liefert einen JSON Web Token (JWT) zurück, der als Kennung an alle anderen Funktionen im HTTP-Header DAT-AuthorizationToken übergeben werden muss.

Der Zugriffstoken ist mind. 10 Minuten lang gültig. Alle Funktionen liefern einen
HTTP-Fehler 401 ("Unangemeldet") zurück, wenn der Zugriffstoken ungültig oder abgelaufen
ist. Wir empfehlen, für jede ununterbrochene Folge von Anfragen einen neuen Token
anzufragen.

Anfragen mit gültigem Token aber mangelnder Berechtigung werden mit einem HTTP-Fehler
403 ("Zugriff verweigert") quittiert.
