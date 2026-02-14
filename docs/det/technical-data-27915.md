---
title: "Technical Data for API Partners"
topic_id: "27915"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Funktionsreferenz > Technical Data for API Partners"
---

# Technical Data for API Partners

| Funktionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| getApiPartnerTechnicalData | POST | Liefert die Fahrzeugmerkmale zurück, die als technische Daten für Schnittstellenpartner markiert sind. | Objekt mit Fahrzeugmerkmalen |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| derivativeId | String | Derivat-ID | Eine der Derivat-Kennungen, die von getDerivatives geliefert werden | ja |
| version | Dezimalzahl | Gültige Workbook-Version | Version des Workbooks, aus dem die Daten des Derivats zurückgeliefert werden sollen | nein |

Das ausgegebene Objekt hat die folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung |
| --- | --- | --- | --- |
| version | Dezimalzahl | Gültige Workbook-Version | Workbook-Version, für die die Derivatdaten ausgegeben werden |
| ident | Objekt | (Datengruppen und Elemente) | Struktur der Datenelemente, Elementgruppen und Untergruppen, die die identifizierenden Merkmale des Derivats beschreiben, die als technische Merkmale für Schnittstellenpartner markiert sind |
| base | Objekt | (Datengruppen und Elemente) | Struktur der Datenelemente, Elementgruppen und Untergruppen, die die Grunddaten des Derivats beschreiben, die als technische Merkmale für Schnittstellenpartner markiert sind |
| specs | Objekt | (Datengruppen und Elemente) | Struktur der Datenelemente, Elementgruppen und Untergruppen, die die Ausstattungsmerkmale des Derivats beschreiben, die als technische Merkmale für Schnittstellenpartner markiert sind |
