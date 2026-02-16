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

- [anmeldung-27906](anmeldung-27906.md)
- [ausstattung-27914](ausstattung-27914.md)
- [derivate-27911](derivate-27911.md)
- [fahrzeugmerkma-28364](fahrzeugmerkma-28364.md)
- [findderivative-27913](findderivative-27913.md)
- [getcatalog-28375](getcatalog-28375.md)
- [getcatalogdate-28808](getcatalogdate-28808.md)
- [getderivatives-27912](getderivatives-27912.md)
- [hersteller-mar-27909](hersteller-mar-27909.md)
- [login-27907](login-27907.md)
- [modelle-27910](modelle-27910.md)
- [refresh-token-27908](refresh-token-27908.md)
- [technical-data-27915](technical-data-27915.md)
- [validierung-vo-27916](validierung-vo-27916.md)
