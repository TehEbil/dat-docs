---
title: "Auswahlmöglichkeiten"
topic_id: "27939"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Logik > Beispiele für die Validierung > Auswahlmöglichkeiten"
---

# Auswahlmöglichkeiten

Gegeben seien E11 bis E17, mit den folgenden logischen Begriffen:

```
E11 INCLUDES AND(OR(E12, E13))
E12 INCLUDES OR(AND(E14, E15), AND(E16, E17))
E13 REQUIRES AND(OR(E14, E15, E16, E17))
```

Die folgende Tabelle listet Kombinationen von Aufrufen von validateConfiguration und
die entsprechenden Ergebnisse auf:

| Im Aufruf angegebene Ausstattung (jede Zeile in einer Reihe bedeutet einen Aufruf) | Fehlercode | Fehlerdetails | Begründung |
| --- | --- | --- | --- |
| [] | 0 |  |  |
| E11 | ERR\_ILLEGAL\_SELECTION | [E11] | Keine von E12 oder E13 angegeben |
| E11, E12 | ERR\_ILLEGAL\_SELECTION | [E12] | Keine von (E14 und E15) oder (E16 und E17) angegeben |
| E11, E13 | ERR\_ILLEGAL\_SELECTION | [E13] | Keine von (E14 oder E15 oder E16 oder E17) angegeben |
| E11, E12, E14 | ERR\_ILLEGAL\_SELECTION | [E12] | E15 nicht zusammen mit E14 angegeben |
| E11, E12, E14, E15 E11, E12, E14, E15, E16 | 0 |  |  |
| E11, E12, E14, E15, E16, E17 | ERR\_ILLEGAL\_SELECTION | [E12] | Sowohl (E14 und E15) als auch (E16 und E17) angegeben |
| E11, E13, E14 E11, E13, E15 E11, E13, E16 E11, E13, E17 | 0 |  |  |
| E11, E13, E14, E15 ... | ERR\_ILLEGAL\_SELECTION | [E13] | Mehr als eine von (E14 oder E15 oder E16 oder E17) angegeben |
