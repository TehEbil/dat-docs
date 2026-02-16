---
title: "Optionen"
topic_id: "15773"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Ausstattungspositionen > Optionen"
---

# Optionen

Ein Optionselement hat einige der folgenden oder alle folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| optionId | String | gültige Optionskennungen | Optionskennung | ja |
| sortNum | Ganzzahl | 1-n | Position der Option in der Preisliste des Herstellers | ja |
| code | String | gültige Optionscodes | Optionscode wie vom Hersteller angegeben (mehrere Codes werden durch ein '+'-Zeichen getrennt, Alternativen werden durch ein '|'-Zeichen getrennt) | nein |
| name | String | Freitext | Kurzbeschreibung der Option, wie sie vom Hersteller bereitgestellt wird | ja |
| fleet | Boolean |  | true, wenn die Option eine Flottenoption ist | nein |
| desc | String | Freitext | Ausführliche Beschreibung der Option, wie sie vom Hersteller bereitgestellt wird | nein |
| comment | String |  |  | nein |
| priceNet | Dezimalzahl | 0-n | Nettopreis der Option (darf 0 sein) | ja |
| priceAfterTax | Dezimalzahl | 0-n | Deutschland: Preis der Option inklusive MwSt. (darf 0 sein) | ja |
| specs | Objekt | (Datengruppen und Elemente) | Struktur der Datenelemente, Elementgruppen und Untergruppen, die die Ausstattung der Option beschreiben. | ja |
| includes | Objekt | (logische Hierarchie) | Logik, die festlegt, welche Optionen, Außenfarben und Polsterungen bei Auswahl dieser Option automatisch mit ausgewählt werden (siehe Beschreibung der Logiksyntax) | nein |
| excludes | Objekt | (logische Hierarchie) | Logik, die definiert, welche Optionen, Außenfarben und Polsterungen nicht ausgewählt werden dürfen, wenn diese Option ausgewählt ist (siehe Beschreibung der Logiksyntax) | nein |
| requires | Objekt | (logische Hierarchie) | Logik, die festlegt, welche Optionen, Außenfarben und Polsterungen bei Auswahl dieser Option ebenfalls ausgewählt werden müssen (siehe Beschreibung der Logiksyntax) | nein |

Das Datenmodell für die Fahrzeugspezifikationen von Optionen ist identisch mit dem
Datenmodell für Fahrzeugspezifikationen von Derivaten.
