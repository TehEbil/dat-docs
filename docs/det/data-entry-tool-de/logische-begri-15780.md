---
title: "Logische Begriffe"
topic_id: "15780"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Logik > Logische Begriffe"
---

# Logische Begriffe

Die im Data Entry Tool verwendeten logischen Begriffe werden immer in einer 2-stufigen
Hierarchie definiert. Ihre Syntax ist bei Optionen, Außenfarben und Polstern identisch:

```
("includes" | "excludes" | "requires"): {
   ("AND" | "OR"): [
      {
         ("AND" | "OR"): [
            <optionId_or_colourId_or_upholsteryId>,
            ...
         ]
      },
      {
         ("AND" | "OR"): [
            <optionId_or_colourId_or_upholsteryId>,
            ...
         ]
      },
      {
         ("AND" | "OR"): [
            <optionId_or_colourId_or_upholsteryId>,
            ...
         ]
      }
   ]
}
```

Jedes der Objekte "includes", "excludes" und "requires" enthält genau eine Array-Eigenschaft. Der Schlüssel der Eigenschaft kann entweder
"AND" oder "OR" sein. In dieser Produktversion enthält das Array zwischen einem und fünf Objekten,
die wiederum genau eine Array-Eigenschaft mit dem Namen "AND" oder "OR" enthalten. Diese Array-Eigenschaften enthalten einen oder mehrere Kennungen von
Ausstattungspositionen.

Alle Ein-Operanden-Klauseln sind AND-Klauseln. OR-Klauseln haben immer mehr als einen Operanden.
