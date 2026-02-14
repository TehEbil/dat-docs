---
title: "getDerivatives"
topic_id: "27912"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Funktionsreferenz > Derivate > getDerivatives"
---

# getDerivatives

| Funktionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| getDerivatives | POST | Liefert grundlegende Informationen zu den Derivaten, die dem angegebenen Modell entsprechen, sowie zusätzliche Informationen. | Array mit Derivat-Objekten |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| modelId | String | gültige Modellkennungen | Eine der Kennungen, die von getModels geliefert werden | ja |
| (identifizierende Fahrzeug-merkmale) |  |  | Null oder mehr Datenelemente, die zur Identifizierung eines Derivats verwendet werden | nein |
| manufacturerCode | String | gültige Bestellcodes | Hersteller-Bestellcode eines Derivats | nein |
| minUsability | String | events.usability Wert (Voreinstellung: "complete") | Kennung, die die Datennutzbarkeit angibt, die das Derivat erreicht oder übertroffen haben muss | nein |
| untilReleaseDate | String | Datum in ISO-8601-Format (YYYY-MM-DD) | Ende des begrenzten Zeitraums in dem das Derivat mindestens einmal freigegeben worden sein muss. | nein |

Die identifizierenden Datenelemente sind Teil des Fahrzeug-Eigenschaftenkatalogs,
der von DAT bereitgestellt wird. Die Parameternamen müssen mit den Elementschlüsseln
übereinstimmen. Die Übereinstimmung basiert immer auf Gleichheit.

Jedes Element im ausgegebenen Arrays ist ein Objekt mit den folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung |
| --- | --- | --- | --- |
| version | Zahl |  | Workbook-Version, zu der das Derivat gehört |
| derivativeId | String |  | Derivatkennung |
| name | String | Freitext | Derivatname |
| ident | Objekt | (identifizierende Datenelemente) | Identifizierende Eigenschaften des Derivats, die für jedes Derivat im Workbook eindeutig sind. |
| base | Objekt | (grundlegende Datenelemente) | Grunddaten des Derivats. Elemente sind Objekte mit der einzigen Eigenschaft value, die den Wert des Elements angibt. |
| events | Objekt | (Ereignisdatenelemente) | Datenelemente, die den aktuellen Status der Daten des Derivats und Marktereignisse in Bezug auf das Derivat beschreiben (ohne Benutzerdaten) |
| codes | Objekt | ecode-Eigenschaft (String) | DAT €uropa-Code®, der zum Derivat gehört |
| images | Objekt | externalImageId-Eigenschaft (String) | Kennung, die verwendet werden kann, um das Fahrzeugbild für das Derivat zu erhalten |

Die Datenelemente sind Teil des Fahrzeug-Eigenschaftenkatalogs, der von der DAT bereitgestellt
wird.
