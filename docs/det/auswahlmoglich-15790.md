---
title: "Auswahlmöglichkeiten"
topic_id: "15790"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Logik > Beispiele für die Validierung > Auswahlmöglichkeiten"
---

# Auswahlmöglichkeiten

Gegeben sind O11 bis O17, mit den folgenden logischen Begriffen:

```
O11 INCLUDES AND(OR(O12, O13))
O12 INCLUDES OR(AND(O14, O15), AND(O16, O17))
O13 REQUIRES AND(OR(O14, O15, O16, O17))
```

Die folgende Tabelle listet Kombinationen von Aufrufen von validateConfiguration und
die entsprechenden Ergebnisse auf:

| Im Aufruf angegebene Optionen (jede Zeile in einer Reihe bedeutet einen Aufruf) | Fehlercode | Fehlerdetails | Begründung |
| --- | --- | --- | --- |
| [] | 0 |  |  |
| O11 | ERR\_ILLEGAL\_SELECTION | [O11] | Keine von O12 oder O13 angegeben |
| O11, O12 | ERR\_ILLEGAL\_SELECTION | [O12] | Keine von (O14 und O15) oder (O16 und O17) angegeben |
| O11, O13 | ERR\_ILLEGAL\_SELECTION | [O13] | Keine von (O14 oder O15 oder O16 oder O17) angegeben |
| O11, O12, O14 | ERR\_ILLEGAL\_SELECTION | [O12] | O15 nicht zusammen mit O14 angegeben |
| O11, O12, O14, O15 O11, O12, O14, O15, O16 | 0 |  |  |
| O11, O12, O14, O15, O16, O17 | ERR\_ILLEGAL\_SELECTION | [O12] | Sowohl (O14 und O15) als auch (O16 und O17) angegeben |
| O11, O13, O14 O11, O13, O15 O11, O13, O16 O11, O13, O17 | 0 |  |  |
| O11, O13, O14, O15 ... | ERR\_ILLEGAL\_SELECTION | [O13] | Mehr als eine von (O14 oder O15 oder O16 oder O17) angegeben |
