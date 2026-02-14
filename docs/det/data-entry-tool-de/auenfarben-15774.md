---
title: "Außenfarben"
topic_id: "15774"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Ausstattungspositionen > Außenfarben"
---

# Außenfarben

Eine Außenfarben-Position hat einige der folgenden oder alle folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| colourId | String | gültige Farbkennungen | Kennung der Außenfarbe | ja |
| sortNum | Ganzzahl | 1-n | Position der Außenfarbe in der Preisliste des Herstellers | ja |
| paintType | String | vordefinierte Typschlüssel | Farbtyp der Außenfarbe - vordefinierter Typschlüssel, siehe Liste der Farbtypschlüssel | nein |
| code | String | gültige Farbcodes | Code der Außenfarbe wie vom Hersteller angegeben (mehrere Codes werden durch ein '+'-Zeichen getrennt, Alternativen werden durch ein '|'-Zeichen getrennt) | nein |
| colour | String | Freitext | Name der Primärfarbe | ja |
| colourAlias | String | vordefinierte Alias-Keys | Primärfarben-Alias - vordefinierte Alias-Keys, siehe Liste der Farb-Alias-Keys | nein |
| colour2 | String | Freitext | Name der Sekundärfarbe | nein |
| colour2Alias | String | vordefinierte Alias-Keys | Sekundärfarben-Alias - vordefinierter Alias-Key, siehe Liste der Farb-Alias-Keys | nein |
| priceNet | Dezimalzahl | 0-n | Nettopreis der Außenfarbe (darf 0 sein) | ja |
| priceAfterTax | Dezimalzahl | 0-n | Deutschland: Preis der Außenfarbe inklusive MwSt. (darf 0 sein) | ja |
| includes | Objekt | (logische Hierarchie) | Logik, die festlegt, welche Optionen, Außenfarben und Polster bei Auswahl dieser Außenfarbe automatisch mit ausgewählt werden (siehe Beschreibung der Logiksyntax) | nein |
| excludes | Objekt | (logische Hierarchie) | Logik, die definiert, welche Optionen, Außenfarben und Polster nicht ausgewählt werden dürfen, wenn diese Außenfarbe ausgewählt ist (siehe Beschreibung der Logiksyntax) | nein |
| requires | Objekt | (logische Hierarchie) | Logik, die festlegt, welche Optionen, Außenfarben und Polster bei Auswahl dieser Außenfarbe ebenfalls ausgewählt werden müssen (siehe Beschreibung der Logiksyntax) | nein |
