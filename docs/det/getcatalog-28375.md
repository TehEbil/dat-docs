---
title: "getCatalog"
topic_id: "28375"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Funktionsreferenz > Fahrzeugmerkmale > getCatalog"
---

# getCatalog

| Funktionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| getCatalog | GET | Liefert den aktuell gültigen DAT-Merkmalskatalog für ein bestimmtes Land und Fahrzeugtyp zurück. | Objekt mit dem angeforderten Merkmalskatalog |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| vehicleType | Ganzzahl | Fahrzeugtyp-Kennung | Eindeutige Kennung des Fahrzeugtyps; fehlt dieser Parameter, wird von allen Fahrzeugtypen der jeweils aktuelle Merkmalskatalog zurückgeliefert | nein |
| country | String | Länderkennung nach ISO-3166-1 | Kennung des Landes; fehlt dieser Parameter, so wird von allen Ländern der jeweils aktuelle Merkmalskatalog zurückgeliefert | nein |

Jedes Element des ausgegebenen Arrays ist ein Objekt mit den folgenden Eigenschaften:

|  |  |  |  |
| --- | --- | --- | --- |
| Name der Eigenschaft | Typ | Werte | Beschreibung |
| effectiveFrom | String | ISO-Zeitstempel: yyyy-MM-ddTHH:mm:ssZ | Zeitpunkt (UTC), seit dem der der Katalog wirksam ist |
| vehicleType | Ganzzahl | ≥1 | Kennung des Fahrzeugtyps |
| country | String | Zwei Großbuchstaben | Länderkennung |
| ident | Objekt | (identifizierende Datenelemente) | Namen, Wertetypen und Wertebereiche der identifizierenden Merkmale von Derivaten |
| base | Objekt | (grundlegende Datenelemente) | Namen, Wertetypen und Wertebereiche der Grunddaten von Derivaten |
| specs | Objekt | (allgemeine Datenelemente) | Namen, Wertetypen und Wertebereiche der Ausstattungsmerkmale von Derivaten |
