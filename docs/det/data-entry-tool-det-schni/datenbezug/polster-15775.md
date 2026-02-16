---
title: "Polster"
topic_id: "15775"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Ausstattungspositionen > Polster"
---

# Polster

Eine Polsterposition hat einige der folgenden oder alle folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| upholsteryId | String | gültige Polsterkennungen | Polsterkennung | ja |
| sortNum | Ganzzahl | 1-n | Position der Polsterung in der Preisliste des Herstellers | ja |
| materialName | String | Freitext | Name des Hauptmaterials | ja |
| materialType | String | vordefinierte Typschlüssel | Hauptmaterialtyp – vordefinierter Typschlüssel, siehe Liste der Materialtypschlüssel | nein |
| material2Type | String | vordefinierte Typenschlüssel | Zusätzlicher Materialtyp - vordefinierter Typenschlüssel, siehe Liste der Materialtypenschlüssel | nein |
| materialCode | String | gültige Farbcodes | Polstercode wie vom Hersteller angegeben (mehrere Codes werden durch ein '+'-Zeichen getrennt, Alternativen werden durch ein '|'-Zeichen getrennt) | nein |
| colour | String | Freitext | Name der Farbe | nein |
| colourAlias | String | vordefinierte Alias-Keys | Farben-Alias - vordefinierter Alias-Key, siehe Liste der Farb-Alias-Keys | nein |
| colourCode | String | Freitext | Farbcode (mehrere Codes werden durch ein '+'-Zeichen getrennt, Alternativen werden durch ein '|'-Zeichen getrennt) | nein |
| priceNet | Dezimalzahl | 0-n | Nettopreis des Polsters (darf 0 sein) | ja |
| priceAfterTax | Dezimalzahl | 0-n | Deutschland: Preis des Polsters inklusive MwSt. (darf 0 sein) | ja |
| includes | Objekt | (logische Hierarchie) | Logik, die festlegt, welche Optionen, Außenfarben und Polster bei Auswahl dieses Polsters automatisch mit ausgewählt werden (siehe Beschreibung der Logiksyntax) | nein |
| excludes | Objekt | (logische Hierarchie) | Logik, die definiert, welche Optionen, Außenfarben und Polsterungen nicht ausgewählt werden dürfen, wenn dieses Polster ausgewählt ist (siehe Beschreibung der Logiksyntax) | nein |
| requires | Objekt | (logische Hierarchie) | Logik, die festlegt, welche Optionen, Außenfarben und Polsterungen bei Auswahl dieses Polsters ebenfalls ausgewählt werden müssen (siehe Beschreibung der Logiksyntax) | nein |
