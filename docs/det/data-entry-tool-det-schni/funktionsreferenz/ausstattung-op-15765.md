---
title: "Ausstattung / Optionen"
topic_id: "15765"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Funktionsreferenz > Ausstattung / Optionen"
---

# Ausstattung / Optionen

| Funktionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| getOptions | POST | Liefert die für ein Fahrzeugderivat verfügbare Serien- und Sonderausstattung, konventionell "Optionen" genannt. | Objekt mit Ausstattungsdaten |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| derivativeId | String | Derivat-ID | Eine der Derivat-Kennungen, die von getDerivatives geliefert werden | ja |
| version | Number | Gültige Workbook-Version | Version des Workbooks, aus dem die Daten des Derivats zurückgeliefert werden sollen | nein |

Das ausgegebene Objekt hat die folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung |
| --- | --- | --- | --- |
| version | Zahl |  | Workbook-Version, für die die Derivatdaten ausgegeben werden |
| specs | Objekt | (Datengruppen und Elemente) | Struktur der Datenelemente, Elementgruppen und Untergruppen, die die Serienausstattung des Derivats beschreiben. Elemente sind Objekte mit der einzigen Eigenschaft value, die den Wert des Elements angibt |
| options | Array | (Datengruppen und Elemente) | Positionen, die die für das Derivat verfügbare Sonderausstattung beschreiben, einschließlich der Fahrzeugspezifikationen der Optionen |
| colours | Array | (Farbpositionen) | Positionen, die die für das Derivat verfügbaren Außenfarben beschreiben |
| upholstery | Array | (Polsterpositionen) | Positionen, die die für das Derivat verfügbaren Polster beschreiben |

Die specs-Datenelemente sind Teil des Fahrzeug-Eigenschaftenkatalogs, der von DAT bereitgestellt
wird.

Die Elemente options, colours und upholstery werden im Anhang beschrieben.
