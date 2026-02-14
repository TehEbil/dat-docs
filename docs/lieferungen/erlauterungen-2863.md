---
title: "Erläuterungen zur SVG Schema Definition"
topic_id: "2863"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 4 > Erläuterungen zur SVG Schema Definition"
---

# Erläuterungen zur SVG Schema Definition

Regeln der svg.xsd

- Jedes grafische Teil erhält folgende Informationen (s. auch [Beispiel Metadaten SVG](#showid/2865 "Beispiel Metadaten SVG")):

  - DVN-Nummern
  - Reparaturcodes
  - Benennung
- Knoten <metadata>:

  Der Knoten <dat:objectInfo> kann unter <metadata> mehrfach vorkommen. Bisher gab es pro <metadata> nur ein <dat:objectInfo>.
- Knoten <dat:objectInfo>:

  Neben der Struktur <dat:title> gibt es die Struktur <dat:tooltip>, jedoch nicht in allen <dat:objectInfo>. Der Knoten <dat:tooltip> könnte also komplett fehlen. Der Aufbau von <dat:tooltip> ist identisch zu <dat:title>.

DVNs können auch Fußnoten (Tooltip) haben.

- Knoten <dat:lang>:

  Das Attribut "lkz" heißt nun "languageCode".

  Das Attribut "stnr" ist neu. Es enthält den Übersetzungscode der jeweiligen Sprache.
- Knoten <dat:objectInfo>:

  Neben den Strukturen <dat:title> und <dat:tooltip> gibt es auch die Struktur <dat:text>, jedoch nicht in allen <dat:objectInfo>. Der Knoten <dat:text> könnte also komplett fehlen. Der Aufbau von <dat:text> ist identisch zu <dat:title> und <dat:tooltip>.

  Das Kennzeichen <kzSeite> ist in der Struktur aufgenommen, da Ersatzteile mit bestimmten Lackkennzeichen (Eurolack
  oder Herstellerlack) an der Flash-Oberfläche anders behandelt werden müssen.
- Knoten <dat:title>, <dat:tooltip> und <dat:text>:

  Das Attribut "stnr" wurde ausgetauscht mit dem Attribut "uebId" <ÜbersetzungsID).
- Knoten <dat:dvnLeft> und <dat:dvnRight>:

  Hier befindet sich das Kennzeichen <dat:etBauart>, denn Ersatzteile mit bestimmter "EBA" (Ersatzteil Bauart) müssen an der Flash-Oberfläche
  anders behandelt werden.

  Hier befindet sich auch das Kennzeichen <dat:etBauartOptKz>, da Ersatzteile mit bestimmten Merkmalen und Kennzeichen an der Flash-Oberfläche
  anders behandelt werden müssen.
