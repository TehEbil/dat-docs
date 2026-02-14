---
title: "Mehrdeutigkeiten bei innerer Auswahl"
topic_id: "15791"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Logik > Beispiele für die Validierung > Mehrdeutigkeiten bei innerer Auswahl"
---

# Mehrdeutigkeiten bei innerer Auswahl

Gegeben sind O21 bis O27, mit den folgenden logischen Begriffen:

```
O21 INCLUDES AND(AND(O26, O27))
O22 INCLUDES AND(AND(O26))
O23 INCLUDES AND(OR(O26, O27))
O24 REQUIRES AND(OR(O26, O27))
O25 REQUIRES AND(AND(O26, O27))
```

Die folgende Tabelle listet Kombinationen von Aufrufen von validateConfiguration und
die entsprechenden Ergebnisse auf:

| Im Aufruf angegebene Optionen (jede Zeile in einer Reihe bedeutet einen Aufruf) | Fehlercode | Fehlerdetails | Begründung |
| --- | --- | --- | --- |
| O21, O22 O21, O23 O21, O24 O21, O25 O22, O23 O22, O24 O21, O22, O23, O24, O25 | 0 |  |  |
| O22, O25 | ERR\_REQUIRED\_MISSING | [O27] | O27 erforderlich durch O25, aber nicht spezifiziert |
| O23, O24  O23, O25 | ERR\_SELECTION | [O23] |  |
| O24, O25 | ERR\_ REQUIRED\_MISSING | [O26, O27] | kein includes, nur requires |
| O24, O25, O26 | ERR\_ REQUIRED\_MISSING | [O27] |  |
| O24, O25, O26, O27 | ERR\_SELECTION | [O24] |  |
