---
title: "Requires"
topic_id: "15782"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Logik > Logische Begriffe > Requires"
---

# Requires

Die "Requires"-Definition besagt, dass der Kunde, um die aktuelle Ausstattungsposition
zu kaufen, auch bestimmte andere Ausstattungspositionen kaufen muss. Die Preise dieser
zusätzlichen Positionen gelten weiterhin, so dass sich der Gesamtpreis aus dem der
aktuellen Position zuzüglich der Preise der zusätzlich erforderlichen Positionen zusammensetzt.

Die Kombination von Positionen mit ODER ist erlaubt: Wenn eine Ausstattungsposition
eine innere ODER-Kombination anderer Ausstattungspositionen erforderlich macht, muss
genau eine der Positionen aus dieser Auswahl vom Kunden ausgewählt werden. Wenn eine
Ausstattungsposition eine äußere ODER-Kombination von Gruppen von Ausstattungspositionen
erforderlich macht, muss der Kunde alle Ausstattungspositionen von genau einer dieser
Gruppen auswählen.

| Äußere Ebene | Innere Ebene | Erlaubt | Beispiel |
| --- | --- | --- | --- |
| AND | AND | Ja | O1 REQUIRES: AND(AND(O4, O5), AND(C2)) |
| AND | AND/OR | Ja | O1 REQUIRES: AND(AND(O2), OR(U1, U2, U3)) |
| AND | OR | Ja | O1 REQUIRES: AND(OR(O7, O8, O9), OR(U1, U2)) |
| OR | AND | Ja | O1 REQUIRES: OR(AND(O4), AND(O7, O8, O9)) |
| OR | AND/OR | Nein | O1 REQUIRES: OR(AND(O4), OR(C1, C2)) |
| OR | OR | Nein | O1 REQUIRES: OR(OR(O4), OR(C1, C2)) |
| OR (einzeln) | | Nein | O1 REQUIRES: OR(AND(O2, O3)) O1 REQUIRES: AND(OR(O2)) |
