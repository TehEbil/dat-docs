---
title: "findDerivatives"
topic_id: "15764"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Funktionsreferenz > Derivate > findDerivatives"
---

# findDerivatives

| Funktionsname | Methode | Beschreibung | Ausgabe |
| --- | --- | --- | --- |
| findDerivatives | POST | Liefert grundlegende Informationen zu den Derivaten, die den angegebenen Fahrzeugspezifikationskriterien entsprechen. | Derivate-Array |

Die Funktion hat die folgenden Parameter:

| Parametername | Typ | Erlaubte Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| country | String | Ländercodes nach ISO-3166-1 | Land, für das die Information angefordert wird | ja |
| vehicleTypes | Array (Zahl) | unterstützte Fahrzeugarten | Kennungen der Fahrzeugarten, für die die Information angefordert wird | ja |
| brands | Array | gültige Markenschlüssel | Einer oder mehrere der von getBrands zurückgegebenen Schlüsselnamen | nein |
| criteria | Array | Objekte:   ``` {   "path": "<property_path>"   "op": "<operator_key>"   ("value": <operand>   | "values": [<operands>]) } ``` | Ein oder mehrere Filterkriterien, die sich auf die Identifizierung von Fahrzeugeigenschaften beziehen | ja |
| untilReleaseDate | String | Datum in ISO-8601-Format (YYYY-MM-DD) | Ende des begrenzten Zeitraums in dem das Derivat mindestens einmal freigegeben worden sein muss. | nein |

Als Datenelementkriterien können beliebige Elemente oder Untergruppen im Fahrzeugeigenschaften-Unterbaum
base, events oder specs angegeben werden. Die Eigenschaft path muss den Pfad zum Datenelement oder zu den Untergruppen angeben, wobei die Ebenen
durch '.' getrennt sind.Beispiel: "base.ident.doors", "base.priceNet", oder "specs.exterior.panoramicRoof". In der folgenden Tabelle sind die zulässigen Operatoren und die Element-/Untergruppenwerttypen
aufgeführt, für die jeder Operator zulässig ist:

| Operator | Relation | Strings | Zahlen | Booleans |
| --- | --- | --- | --- | --- |
| eq | Elementwert ist identisch mit value | ja | ja | ja |
| in | Elementwert ist einer der in values definierten Werte | ja | ja | nein |
| ne | Elementwert ist nicht identisch mit value | ja | ja | ja |
| lt | Elementwert ist geringer als value | nein | ja | nein |
| le | Elementwert ist geringer oder gleich value | nein | ja | nein |
| gt | Elementwert ist größer als value | nein | ja | nein |
| ge | Elementwert ist größer oder gleich value | nein | ja | nein |

Das gleiche Element/die gleiche Untergruppe kann in mehreren Kriterien angegeben werden.
Zum Beispiel können "ge" und "le" in zwei Kriterien mit demselben Datenelement angegeben
werden, um ein "zwischen"-Kriterium zu definieren. Es wird nicht geprüft, ob mehrere
Angaben zum gleichen Datenelement/zur gleichen Untergruppe zu widersprüchlichen Kriterien
führen. Ein Derivat erfüllt ein Kriterium, wenn die Fahrzeugspezifikationen des Derivats
es direkt erfüllen oder wenn eine für das Derivat verfügbare Option es erfüllt. Zum
Beispiel ist das Kriterium "specs.exterior.panoramicRoof == Yes" erfüllt, wenn

- das Panoramadach in den Spezifikationsdaten specs des Derivats definiert ist
- ODER wenn es eine Option für das Derivat gibt, die ein Panoramadach definiert

Die Kriterien werden auch mit allen Optionen abgeglichen, die für das Derivat verfügbar
sind. Die Logikdefinitionen der Optionen werden ignoriert. Es wird nicht geprüft, ob es mehrere Kriterien gibt, die zu widersprüchlichen Ergebnissen führen,
z.B. wenn sich Kriterium A auf die Option O1 stützt, während sich Kriterium B auf
die Option O2 stützt, aber O1 O2 ausschließt. Die path-Eigenschaft eines jeden Kriteriums wird auf Gültigkeit geprüft. Alle Pfade, die nicht
mit einem der folgenden Muster übereinstimmen, führen zu einem Fehler:

- "base." <basic\_characteristic\_name> (nur die erlaubten Eigenschaftsnamen)
- "base.ident." <identifying\_property\_name> (nur die erlaubten Eigenschaftsnamen)
- "specs." <top\_level\_item\_group> "." <...> (alles unterhalb einer Top-Level-Gruppe)

Die Suche erfolgt von der niedrigsten zur höchsten Markenkennung. Innerhalb einer
Marke erfolgt die Suche in alphabetischer Reihenfolge der Modellkürzel Innerhalb eines
Modells erfolgt die Suche in der Preislistenreihenfolge der Derivate (Attribut sortNum).

Die Funktion liefert nur die ersten 200 übereinstimmenden Derivate.

Jedes Element des zurückgegebenen Arrays ist ein Objekt, das die gleichen Datenelemente
des Derivats enthält, die auch von der Funktion getDerivatives zurückgegeben werden:

| Name der Eigenschaft | Typ | Werte | Beschreibung |
| --- | --- | --- | --- |
| brand | Objekt | ``` {   "id": <manufacturer_id>,   "name": "<local_name>" } ``` | Marke, zu der das Derivat gehört |
| model | Objekt | ``` {   "modelId": <model_acronym>,   "modelName": "<model_name>" } ``` | Modell, zu der das Derivat gehört |
| derivativeId | String |  | Derivatkennung |
| version | Zahl |  | Workbook-Version, zu der das Derivat gehört |
| name | String | Freitext | Derivatname |
| base | Objekt | (grundlegende Datenelemente) | Grundlegende Eigenschaften des Derivats. Elemente sind Objekte mit der einzigen Eigenschaft value, die den Wert des Elements angibt. |
| events | Objekt | (Ereignisdatenelemente) | Datenelemente, die den aktuellen Status der Daten des Derivats und Marktereignisse in Bezug auf das Derivat beschreiben (ohne Benutzerdaten) |
| codes | Objekt | ecode-Eigenschaft (String) | DAT €uropa-Code®, der zum Derivat gehört |
| images | Objekt | externalImageId-Eigenschaft (String) | Kennung, die verwendet werden kann, um das Fahrzeugbild für das Derivat zu erhalten |
