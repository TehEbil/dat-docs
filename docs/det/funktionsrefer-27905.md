---
title: "Funktionsreferenz"
topic_id: "27905"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Funktionsreferenz"
---

# Funktionsreferenz

Alle Funktionen verwenden als Basis-Datenformat die "JavaScript Object Notation" (JSON).
Dieses Format wird sowohl für HTTP-Antworten ("Response Body") als auch für HTTP-POST-Anfragen
("Request Body") verwendet. Die Parameter bei HTTP-GET-Aufrufen sind dagegen grundsätzlich
einfache Zeichenketten, falls nicht anders angegeben.

Standardmäßig verwenden alle Funktionen nur die neueste Version des Workbooks eines
jeden Fahrzeug-Modells. Ausgelaufene Modelle werden ignoriert.

Jedoch haben einige Funktionen einen optionalen Parameter untilReleaseDate. Dieser Parameter bestimmt das Ende einer vordefinierten Zeitspanne von 24 Monaten,
im Folgenden als "beschränkte Zeitspanne" bezeichnet. Wenn dieser Parameter gegeben
ist, dann wird die jeweilige Funktion die Workbooks behandeln, die innerhalb dieser
Zeitspanne freigegeben wurden.
