---
title: "Merkmalskatalog"
topic_id: "28381"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Merkmalskatalog"
---

# Merkmalskatalog

Ein Merkmalskatalog beschreibt das Schema der Fahrzeugmerkmale in einem der Bäume
ident, base und dem specs-Baum von Ausstattungen. Jede Baumebene wird durch ein Objekt dargestellt, dessen Schlüssel die Felder dieser
Ebene bestimmen. Jedes Feld ist wiederum ein Objekt. Der Wertetyp des Feldes, type, bestimmt in jedem Knoten des Baumes die weiteren Felder zur Bestimmung des Wertebereiches.
Unterknoten, falls vorhanden, werden als Objekt im Feld children gespeichert. Die
Baumstruktur wiederholt sich ab hier rekursiv.

Ein Feld im Merkmalskatalog:

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| Name | Typ | Werte | Beschreibung | Pflicht |
| type | String | "None", "Boolean", "String", "Number", "Date", "Enum" | Der Wertetyp dieses Knotens ("None" bedeutet "kein Wert") | ja |
| children | Objekt | Untergeordnete Felder | Nur falls untergeordnete Felder vorhanden sind | nein |
| precision | Ganzzahl | ≥ 0 | Nur bei type = "Number": Anzahl der Nachkommastellen | nein |
| min | Zahl |  | Nur bei type = "Number": Kleinstmöglicher Wert | nein |
| max | Zahl |  | Nur bei type = "Number": Größtmöglicher Wert | nein |
| values | Array | Vorgegebene Werte beliebigen Typs | Nur bei type = "Enum": alle erlaubten Werte des Feldes (Typ beliebig) | nein |
