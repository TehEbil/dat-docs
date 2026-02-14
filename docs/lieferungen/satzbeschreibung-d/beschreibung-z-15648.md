---
title: "Beschreibung Zusatzelement 4a"
topic_id: "15648"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 4a"
---

# Beschreibung Zusatzelement 4a

Eine ausführlichere Beschreibung der SVG-Dateien inklusive Beispielen zur Verarbeitung
der Baugruppengrafiken finden Sie im DAT Developers Guide, [SVG in den DAT Anwendungen](../../allgemein/dat-developers-gui/svg-in-den-dat-1551.md).

Zusatzelement 4a erweitert Zusatzelement 4 um folgende Möglichkeiten:

- Zuordnung zwischen Hauttypen und Zonengrafiken
- Zuordnung der Baugruppengrafiken zu Fahrzeugzonen
- Filterung der Baugruppengrafiken für einzelne Untertypen
- Filterung der Baugruppengrafiken anhand Ausstattungen

Eine ausführliche Beischreibung zu Zusatzelement 4 inklusive Beispielen finden Sie
hier.

Die Dateninformationen werden in zwei xml-Dateien sowie einem Zip-Archiv ausgeliefert.
Die Namen der Dateien lauten zusatz4a.xml, zusatz4a\_ht\_zg.xml sowie zusatz4azonengrafik.zip. Im Zip Archiv sind die SVGs der Zonengrafiken enthalten. Beispiel: zusatz4a\_zg\_1.svg. Die Nummer vor der Dateiendung, in diesem Fall "1", steht für die ID der jeweiligen Zonengrafik.

Legende:

FZA = Fahrzeugart

HST = Hersteller

HT = Haupttyp

constructionGroupId= Baugruppen-ID

constructionGroupNames = Baugruppenbenennungen

zones = Liste der zugehörigen Fahrzeugzonen

subModels = Liste der Untertypen, für die die jeweilige Baugruppengrafik Gültigkeit hat

options = Liste der Ausstattungen, für die die jeweilige Baugruppengrafik Gültigkeit hat

constructionTimeFrom = Bauzeit in DAT Notation ab der die jeweilige Baugruppengrafik Gültigkeit besitzt.

metadata = Liste von gültigen DVNs und deren zulässige Reparaturcodes.

Für weitere Informationen zu den Baugruppengrafiken klicken Sie hier.
