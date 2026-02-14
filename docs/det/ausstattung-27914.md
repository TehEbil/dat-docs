---
title: "Ausstattung"
topic_id: "27914"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Funktionsreferenz > Ausstattung"
---

# Ausstattung

| Funktionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| getEquipment | POST | Liefert die für ein Fahrzeugderivat verfügbare Serien- und Sonderausstattung (Optionen). | Objekt mit Ausstattungsdaten |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| derivativeId | String | Derivat-ID | Eine der Derivat-Kennungen, die von getDerivatives geliefert werden | ja |
| version | Dezimalzahl | Gültige Workbook-Version | Version des Workbooks, aus dem die Daten des Derivats zurückgeliefert werden sollen. Falls der Paramter nicht gesetzt ist, wird die jüngste Workbook-Version verwendet | nein |

Das ausgegebene Objekt hat die folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung |
| --- | --- | --- | --- |
| version | Dezimalzahl | Gültige Workbook-Version | Workbook-Version, für die die Derivatdaten ausgegeben werden. |
| unavailableSpecs | Objekt | (nicht verfügbare Datenelemente) | Baum von Merkmalen, die in keiner Ausstattung für dieses Derivat vorkommen können. Elemente sind Objekte mit einem einzigen Feld value |
| equipment | Array | (Datengruppen und Elemente) | Positionen, die die für das Derivat verfügbare Ausstattung beschreiben, einschließlich der Merkmale der Ausstattungen. Beinhaltet Serienausstattung, Optionen, Außenfarben und Innenfarben. |
