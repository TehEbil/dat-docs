---
title: "getCatalogDate"
topic_id: "28808"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Funktionsreferenz > Fahrzeugmerkmale > getCatalogDate"
---

# getCatalogDate

| Functionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| getCatalogDate | GET | Liefert das Datum der jüngsten Änderung des Fahrzeugmerkmalskatalogs zurück. Die Suche kann optional auf ein Land oder einen Fahrzeugtypen beschränkt werden. | Datum der letzten Änderung des Merkmalskatalogs. |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| vehicleType | Number | Kennung des Fahrzeugtyps | Eindeutige Kennung des Fahrzeugtyps; fehlt dieser Parameter, so wird das Datum der jüngsten Änderung der Kataloge aller Fahrzeugtypen zurückgeliefert | nein |
| country | String | Ländercode nach ISO-3166-1 Alpha2 | Eindeutiger Ländercode; fehlt dieser, so wird das Datum der jüngsten Änderung der Kataloge aller Länder zurückgeliefert. | nein |

Each element of the returned array is an object having the following fields:

|  |  |  |  |
| --- | --- | --- | --- |
| Property name | Type | Values | Description |
| effectiveFrom | String | Zeitstempel nach ISO-8601 (yyyy-MM-ddTHH:mm:ssZ) | Zeitpunkt (UTC) seitdem der geänderte Katalog gültig ist |
