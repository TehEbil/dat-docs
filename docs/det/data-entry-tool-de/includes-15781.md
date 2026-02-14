---
title: "Includes"
topic_id: "15781"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Logik > Logische Begriffe > Includes"
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
| AND | AND | Ja | O1 INCLUDES: AND(AND(O4, O5), AND(C2)) |
| AND | AND/OR | Ja | O1 INCLUDES: AND(AND(O2), OR(U1, U2, U3)) |
| AND | OR | Ja | O1 INCLUDES: AND(OR(O7, O8, O9), OR(U1, U2)) |
| OR | AND | Ja | O1 INCLUDES: OR(AND(O4), AND(O7, O8, O9)) |
| OR | AND/OR | Nein | O1 INCLUDES: OR(AND(O4), OR(C1, C2)) |
| OR | OR | Nein | O1 INCLUDES: OR(OR(O4), OR(C1, C2)) |
| OR (einzeln) | | Nein | O1 INCLUDES: OR(AND(O2, O3)) O1 INCLUDES: AND(OR(O2)) |
