---
title: "Modelle"
topic_id: "15761"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Funktionsreferenz > Modelle"
---

# Modelle

|  |  |  |  |
| --- | --- | --- | --- |
| getModels | POST | Liefert die verfügbaren Modelle für eine Fahrzeugmarke. | Array von Objekten, die die Modelle enthalten |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| country | String | Ländercodes nach ISO-3166-1 | Land, für das die Information angefordert wird | ja |
| vehicleTypes | Array (Zahl) | unterstützte Fahrzeugarten | Kennung der Fahrzeugart, für die die Information angefordert wird | ja |
| brand | Zahl | gültige Markenkennungen | Einer der id-Werte, die von getBrands geliefert werden | ja |
| untilReleaseDate | String | Datum in ISO-8601-Format (YYYY-MM-DD) | Ende des begrenzten Zeitraums in dem ein freigegebenes Workbook mit mindestens einem Derivat existieren muss. | nein |

Jedes Objekt im ausgegebenen Array hat folgende Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung |
| --- | --- | --- | --- |
| modelId | String |  | Modellkennung (besteht aus Länderkennzeichen, Fahrzeugart, Hersteller und Modellkürzel) |
| modelName | String |  | Lokale Modellbezeichnung |

Die Funktion liefert nur Modelle zurück, für die es mindestens ein aktuell verfügbares
Derivat gibt. Falls untilReleaseDate angegeben wurde, werden nur diejenigen Modelle zurückgeliefert, für die es bis zum
angegeben Datum mindestens ein Derivat gab.
