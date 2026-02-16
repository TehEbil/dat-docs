---
title: "Requires"
topic_id: "27931"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Logik > Logische Verknüpfungen > Requires"
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
| AND | AND | Ja | E1 REQUIRES: AND(AND(E4, E5), AND(C2)) |
| AND | AND/OR | Ja | E1 REQUIRES: AND(AND(E2), OR(U1, U2, U3)) |
| AND | OR | Ja | E1 REQUIRES: AND(OR(E7, E8, E9), OR(U1, U2)) |
| OR | AND | Ja | E1 REQUIRES: OR(AND(E4), AND(E7, E8, E9)) |
| OR | AND/OR | Nein | E1 REQUIRES: OR(AND(E4), OR(C1, C2)) |
| OR | OR | Nein | E1 REQUIRES: OR(OR(E4), OR(C1, C2)) |
| OR (einzeln) | | Nein | E1 REQUIRES: OR(AND(E2, E3)) E1 REQUIRES: AND(OR(E2)) |
