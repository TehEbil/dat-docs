---
title: "Ausstattung"
topic_id: "28356"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Ausstattungspositionen > Ausstattung"
---

# Ausstattung

Eine Ausstattung hat die folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| id | String | gültige Ausstattungsskennungen | Ausstattungskennung (Cxxxxxx für Außenfarben, Uxxxxxx für Innenfarben und Exxxxxx für andere Ausstattungen oder Mischungen | ja |
| code | String | gültige Optionscodes | Optionscode wie vom Hersteller angegeben (mehrere Codes werden durch ein '+'-Zeichen getrennt, Alternativen werden durch ein '|'-Zeichen getrennt) | nein |
| name | String | Freitext | Kurzbezeichnung der Ausstattung, wie sie vom Hersteller bereitgestellt wird | ja |
| description | String | Freitext | Ausführliche Beschreibung der Ausstattung, wie sie vom Hersteller bereitgestellt wird | nein |
| specs | Objekt | (Datengruppen und Elemente) | Struktur der Datenelemente, Elementgruppen und Untergruppen, die die Ausstattung beschreiben. | ja |
| variants | Array | Objekte mit Werten | Unterschiedliche Preise und Verwendungsarten dieser Ausstattung | ja |
