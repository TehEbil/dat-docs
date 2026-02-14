---
title: "Variante"
topic_id: "28357"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Ausstattungspositionen > Variante"
---

# Variante

| Name der Eigenschaft | Typ | Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| id | Zahl | 1-n | Eindeutige Kennung der Ausstattungsvariante. Cxxxxxxxx für Außenfarben, Uxxxxxxxx für Innenfarben und Exxxxxxxx für andere Ausstattung. | ja |
| priceNet | Dezimalzahl | 0-n | Nettopreis der Option (darf 0 sein) | ja |
| priceAfterTax | Dezimalzahl | 0-n | Deutschland: Preis der Option inklusive MwSt. (darf 0 sein) | ja |
| includes | Objekt | (logische Hierarchie) | Logik, die festlegt, welche Optionen, Außenfarben und Polsterungen bei Auswahl dieser Option automatisch mit ausgewählt werden (siehe Beschreibung der Logiksyntax) | nein |
| excludes | Objekt | (logische Hierarchie) | Logik, die definiert, welche Optionen, Außenfarben und Polsterungen nicht ausgewählt werden dürfen, wenn diese Option ausgewählt ist (siehe Beschreibung der Logiksyntax) | nein |
| requires | Objekt | (logische Hierarchie) | Logik, die festlegt, welche Optionen, Außenfarben und Polsterungen bei Auswahl dieser Option ebenfalls ausgewählt werden müssen (siehe Beschreibung der Logiksyntax) | nein |
| standard | Boolean |  | true bedeutet Serienausstattung  false bedeutet Option | nein |
| discontinued | Boolean |  | true bedeutet, dass diese Ausstattung ausgelaufen ist und entfernt wird | nein |
| fleetOption | Boolean |  | true bedeutet, dass die Option für Flottenmodelle vorgesehen ist (nur für Optionen) | nein |
| visible | Boolean |  | true bedeutet, dass diese Ausstattung in der Auswahl sichtbar ist (nur für Serienausstattung) | nein |
| selectable | Boolean |  | true bedeutet, dass diese Ausstattung direkt auswählbar ist (nur für optionale Ausstattung)  false bedeutet, dass diese Ausstattung nicht in Auswahllisten auftauchen sollte und nur indirekt über Pakete ausgewählt werden kann | nein |
| preselected | Boolean |  | true bedeutet, dass die Ausstattung anfangs ausgewählt ist (nur für optionale Ausstattung) | nein |
| priceList | Boolean |  | true bedeutet, dass diese Ausstattung von der Preisliste stammt.  false bedeutet manuelle Recherche | nein |
