---
title: "Zugriff von einem anderen (Micro-)Service aus"
topic_id: "22639"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Anmeldung > Zugriff von einem anderen (Micro-)Service aus"
---

# Zugriff von einem anderen (Micro-)Service aus

Vor dem Zugriff auf jedwede Funktion zur Datenabfrage muss der Benutzer sich mittels
eines Aufrufs der Login-Funktion berechtigen. Diese Funktion liefert einen JSON Web Token (JWT) zurück, der als Kennung an alle anderen Funktionen übergeben werden muss, im HTTP-Header DAT-AuthorizationToken.

Der Zugriffstoken ist mind. 10 Minuten lang gültig. Dies sollte für alle einmaligen
Anfragen ausreichen. Alle Funktionen liefern einen HTTP-Fehler 401 ("Unangemeldet")
zurück, wenn der Zugriffstoken ungültig oder abgelaufen ist. Wir empfehlen, für jede
Folge von Anfragen, die nicht durch menschliche Benutzer unterbrochen wird (und somit
den Ablauf des Tokens zur Folge haben könnte), einen neuen Token anzufragen.
