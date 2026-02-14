---
title: "Includes"
topic_id: "27930"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Logik > Logische Verknüpfungen > Includes"
---

# Includes

Die Bedeutung einer "Includes"-Definition ist, dass beim Kauf der aktuellen Ausstattungsposition
durch den Kunden andere Positionen, die für sich genommen einen Preis ungleich 0 haben
können, automatisch und kostenlos enthalten sind.

Die Kombination von Positionen mit ODER ist erlaubt: Wenn eine Ausstattungsposition
eine innere ODER-Kombination anderer Ausstattungspositionen enthält, muss genau eine
der Positionen aus dieser Auswahl vom Kunden ausgewählt werden. Wenn eine Ausstattungsposition
eine äußere ODER-Kombination von Gruppen von Ausstattungspositionen umfasst, muss
der Kunde alle Ausstattungspositionen von genau einer dieser Gruppen auswählen.

| Äußere Ebene | Innere Ebene | Erlaubt | Beispiel |
| --- | --- | --- | --- |
| AND | AND | Ja | E1 INCLUDES: AND(AND(E4, E5), AND(C2)) |
| AND | AND/OR | Ja | E1 INCLUDES: AND(AND(E2), OR(U1, U2, U3)) |
| AND | OR | Ja | E1 INCLUDES: AND(OR(E7, E8, E9), OR(U1, U2)) |
| OR | AND | Ja | E1 INCLUDES: OR(AND(E4), AND(E7, E8, E9)) |
| OR | AND/OR | Nein | E1 INCLUDES: OR(AND(E4), OR(C1, C2)) |
| OR | OR | Nein | E1 INCLUDES: OR(OR(E4), OR(C1, C2)) |
| OR (einzeln) | | Nein | E1 INCLUDES: OR(AND(E2, E3)) E1 INCLUDES: AND(OR(E2)) |
