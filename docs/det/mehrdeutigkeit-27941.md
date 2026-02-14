---
title: "Mehrdeutigkeiten bei äußerer Auswahl"
topic_id: "27941"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Logik > Beispiele für die Validierung > Mehrdeutigkeiten bei äußerer Auswahl"
---

# Mehrdeutigkeiten bei äußerer Auswahl

Gegeben sind E31 bis E37, mit den folgenden logischen Verknüpfungen:

```
E31 INCLUDES OR(AND(E36, E37), AND(E38, E39))
E32 INCLUDES AND(AND(E36))
E33 INCLUDES AND(AND(E37))
E34 INCLUDES AND(AND(E38))
E35 INCLUDES AND(AND(E39))
```

Die folgende Tabelle listet Kombinationen von Aufrufen von validateConfiguration und
die entsprechenden Ergebnisse auf:

| Im Aufruf angegebene Optionen (jede Zeile in einer Reihe bedeutet einen Aufruf) | Fehlercode | Fehlerdetails | Begründung |
| --- | --- | --- | --- |
| E31, E32, E33 E31, E33, E36 E31, E32, E33, E38 E31, E32, E33, E38, E39 E31, E32, E37, E38 | 0 |  |  |
| E31, E32, E37, E38, E39 E31, E36, E37, E38, E39 | ERR\_SELECTION | [E31] | Die Elemente der beiden Positionsgruppen innerhalb der äußeren Auswahl wurden im Aufruf angegeben |
