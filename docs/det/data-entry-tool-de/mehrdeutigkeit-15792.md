---
title: "Mehrdeutigkeiten bei äußerer Auswahl"
topic_id: "15792"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Logik > Beispiele für die Validierung > Mehrdeutigkeiten bei äußerer Auswahl"
---

# Mehrdeutigkeiten bei äußerer Auswahl

Gegeben sind O31 bis O37, mit den folgenden logischen Begriffen:

```
O31 INCLUDES OR(AND(O36, O37), AND(O38, O39))
O32 INCLUDES AND(AND(O36))
O33 INCLUDES AND(AND(O37))
O34 INCLUDES AND(AND(O38))
O35 INCLUDES AND(AND(O39))
```

Die folgende Tabelle listet Kombinationen von Aufrufen von validateConfiguration und
die entsprechenden Ergebnisse auf:

| Im Aufruf angegebene Optionen (jede Zeile in einer Reihe bedeutet einen Aufruf) | Fehlercode | Fehlerdetails | Begründung |
| --- | --- | --- | --- |
| O31, O32, O33 O31, O33, O36 O31, O32, O33, O38 O31, O32, O33, O38, O39 O31, O32, O37, O38 | 0 |  |  |
| O31, O32, O37, O38, O39 O31, O36, O37, O38, O39 | ERR\_SELECTION | [O31] | Die Elemente der beiden Positionsgruppen innerhalb der äußeren Auswahl wurden im Aufruf angegeben |
