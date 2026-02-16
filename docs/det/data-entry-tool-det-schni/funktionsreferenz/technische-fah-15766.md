---
title: "Technische Fahrzeugdaten"
topic_id: "15766"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Funktionsreferenz > Technische Fahrzeugdaten"
---

# Technische Fahrzeugdaten

| Funktionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| getTechnicalData | POST | Liefert die als technische Fahrzeugdaten bezeichneten Datenelemente. | Objekt mit technischen Daten |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| derivativeId | String | Derivat-ID | Eine der Derivat-Kennungen, die von getDerivatives geliefert werden | ja |
| version | Number | Gültige Workbook-Version | Version des Workbooks, aus dem die Daten des Derivats zurückgeliefert werden sollen | nein |

Das ausgegebene Objekt hat die folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung |
| --- | --- | --- | --- |
| version | Zahl |  | Workbook-Version, für die die Derivatdaten ausgegeben werden |
| specs | Objekt | (Datengruppen und Elemente) | Struktur der Datenelemente, Elementgruppen und Untergruppen, die die technischen Daten des Derivats beschreiben. Elemente sind Objekte mit der einzigen Eigenschaft value, die den Wert des Elements angibt |

Die specs-Datenelemente sind Teil des Fahrzeug-Eigenschaftenkatalogs, der von DAT bereitgestellt
wird.
