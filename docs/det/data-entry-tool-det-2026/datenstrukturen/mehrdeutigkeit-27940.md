---
title: "Mehrdeutigkeiten bei innerer Auswahl"
topic_id: "27940"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Logik > Beispiele für die Validierung > Mehrdeutigkeiten bei innerer Auswahl"
---

# Mehrdeutigkeiten bei innerer Auswahl

Gegeben sind E21 bis E27, mit den folgenden logischen Verknüpfungen:

```
E21 INCLUDES AND(AND(E26, E27))
E22 INCLUDES AND(AND(E26))
E23 INCLUDES AND(OR(E26, E27))
E24 REQUIRES AND(OR(E26, E27))
E25 REQUIRES AND(AND(E26, E27))
```

Die folgende Tabelle listet Kombinationen von Aufrufen von validateConfiguration und die entsprechenden Ergebnisse auf:

| Im Aufruf angegebene Ausstattung (jede Zeile in einer Reihe bedeutet einen Aufruf) | Fehlercode | Fehlerdetails | Begründung |
| --- | --- | --- | --- |
| E21, E22 E21, E23 E21, E24 E21, E25 E22, E23 E22, E24 E21, E22, E23, E24, E25 | 0 |  |  |
| E22, E25 | ERR\_REQUIRED\_MISSING | [E27] | E27 erforderlich durch E25, aber nicht spezifiziert |
| E23, E24  E23, E25 | ERR\_SELECTION | [E23] |  |
| E24, E25 | ERR\_ REQUIRED\_MISSING | [E26, E27] | kein includes, nur requires |
| E24, E25, E26 | ERR\_ REQUIRED\_MISSING | [E27] |  |
| E24, E25, E26, E27 | ERR\_SELECTION | [E24] |  |
