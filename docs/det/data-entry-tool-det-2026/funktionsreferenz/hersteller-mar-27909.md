---
title: "Hersteller / Marken"
topic_id: "27909"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Funktionsreferenz > Hersteller / Marken"
---

# Hersteller / Marken

| Funktionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| getBrands | POST | Liefert die Fahrzeughersteller im DAT-Kontext - faktisch Fahrzeugmarken. | Array von Objekten, die Markennamen-Kennungen und Namen in der Sprache des angegebenen Landes enthalten. Jedes Objekt im Array hat die Werte id (Bezeichner) und name (lokaler Name). |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| country | String | Länderkennzeichen nach ISO-3166-1 | Land, für das die Information angefordert wird | ja |
| vehicleTypes | Array (Zahl) | unterstützte Fahrzeugarten | Kennungen der Fahrzeugarten, für die die Information angefordert wird | ja |
| untilReleaseDate | String | Datum in ISO-8601-Format (YYYY-MM-DD) | Ende des begrenzten Zeitraums in dem ein freigegebenes Workbook mit mindestens einem Derivat existieren muss. | nein |

Die Funktion liefert nur Marken zurück, für die es mindestens ein Modell mit momentan
verfügbaren Derivaten gibt. Falls untilReleaseDate angegeben wurde, werden nur diejenigen Marken zurückgeliefert, für die mindestens
ein Modell mit mindestens einem Derivat in dem beschränkten Zeitraum bis zum angegebenen
Datum existierte.
