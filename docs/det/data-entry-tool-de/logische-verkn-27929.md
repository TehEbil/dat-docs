---
title: "Logische Verknüpfungen"
topic_id: "27929"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Logik > Logische Verknüpfungen"
---

# Logische Verknüpfungen

Die im Data Entry Tool verwendeten logischen Verknüpfungen werden immer in einer 2-stufigen
Hierarchie definiert. Ihre Syntax ist immer gleich:

```
("includes" | "excludes" | "requires"): {
   ("AND" | "OR"): [
      {
         ("AND" | "OR"): [
            <equipmentId>,
            ...
         ]
      },
      {
         ("AND" | "OR"): [
            <equipmentId>,
            ...
         ]
      },
      {
         ("AND" | "OR"): [
            <equipmentId>,
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

Alle Ein-Operanden-Klauseln sind AND-Verknüpfungen. OR-Klauseln haben immer mehr als einen Operanden.
