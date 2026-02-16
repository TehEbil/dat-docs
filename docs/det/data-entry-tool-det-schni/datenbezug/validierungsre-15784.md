---
title: "Validierungsregeln"
topic_id: "15784"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Logik > Validierungsregeln"
---

# Validierungsregeln

Um den Erfolg der DET-Schnittstellenfunktion validateConfiguration sicherzustellen, müssen beim Aufruf der Funktion folgende Regeln beachtet werden:

- Jede Ausstattungsposition, die im Aufruf angegeben ist, muss für das Derivat freigegeben
  sein.
- Wenn einige der angegebenen Ausstattungspositionen andere Positionen durch AND-Definitionen einschließen, dürfen die eingeschlossenen Positionen nicht im Aufruf
  angegeben werden.
- Wenn einige der angegebenen Ausstattungspositionen andere Ausstattungspositionen durch
  AND-Definitionen erfordern, müssen alle erforderlichen Ausstattungspositionen im Aufruf
  angegeben werden, sofern sie nicht durch andere Ausstattungspositionen durch AND-Definitionen eingeschlossen sind.
- Wenn einige der angegebenen Ausstattungspositionen über OR-Einschlüsse andere Positionen einschließen oder erfordern, muss genau eine der eingeschlossenen
  / erforderlichen Positionen im Aufruf angegeben werden, es sei denn, eine oder mehrere
  von ihnen sind über AND-Definitionen von anderen Ausstattungspositionen eingeschlossen.
- Die "Includes"-, "Excludes"- und "Requires"-Definitionen der Ausstattungspositionen, die im Aufruf angegeben oder implizit enthalten
  sind, dürfen von keiner der anderen angegebenen oder implizit enthaltenen Ausstattungspositionen
  verletzt werden.

Das bedeutet, dass die logischen Definitionen von Positionen, die implizit über eine
AND-Einbindung eingeschlossen sind, rekursiv geprüft werden müssen. Andererseits müssen
die logischen Definitionen von ausgeschlossenen, erforderlichen und über eine Auswahl
eingeschlossenen Positionen nicht rekursiv geprüft werden:

- Wenn Position A Position B voraussetzt, werden die Definitionen von B trotzdem ausgewertet,
  wenn es explizit angegeben ist, und es tritt ein Fehler auf, wenn es nicht explizit
  angegeben ist.
- Wenn Position A Position B ausschließt, können die Definitionen von B ignoriert werden,
  da B ohnehin nicht Teil der Konfiguration sein darf, und es tritt ein Fehler auf,
  wenn es dennoch angegeben wird.

Widersprüchliche Logik wird vom Data Entry Tool während des Editiervorgangs geprüft; daher sollte eine solche Logik in den Daten
nicht vorkommen. Um sicherzugehen, führt die Funktion validateConfiguration dieselben Prüfungen jedoch selbst durch. Wenn ein Logikfehler erkannt wird, gibt die
Funktion den Fehlercode ERR\_LOGIC zurück.
