---
title: "Fahrzeugmerkmale"
topic_id: "27920"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Fahrzeugspezifikationen > Fahrzeugmerkmale"
---

# Fahrzeugmerkmale

Fahrzeugmerkmale haben grundsätzlich eine Baumstruktur. Eine Ebene besteht aus einem
Objekt aus Feldern mit beliebigen Namen. Hinter jedem Namen findet sich ein Objekt,
das ein Feld "value" und/oder ein Feld children enthält.

- value bezeichnet den Wert des Baumknotens. Der Wert kann fehlen, wenn der Knoten nur zusammenfassende
  Funktion hat.
- children bezeichnet die nächste Ebene des Baumes. Die Struktur des Baumes wiederholt sich
  rekursiv in tieferen Ebenen, bis ein Knoten kein children-Feld mehr enthält (oder das Array dahinter leer ist)

Beispiel:

```
"specs": {
  "exterior": {
    "children": {
      "frontDoorType": {
         "value": "hinged";
       },
      "panoramicRoof": {
        "value": true,
        "children": {
          "roofType": {
            "value": "fabric";
          }
          
        }
      }
    }
  }
}
```
