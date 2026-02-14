---
title: "Excludes"
topic_id: "27932"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Logik > Logische Verknüpfungen > Excludes"
---

# Excludes

Die Bedeutung einer "Excludes"-Definition ist, dass wenn der Kunde die aktuelle Ausstattungsposition
kauft, die Ausstattungspositionen, die dadurch ausgeschlossen werden, nicht gleichzeitig
gekauft werden dürfen.

ODER-Kombinationen von Positionen sind nicht erlaubt: Eine Ausstattungsposition kann
andere nur bedingungslos ausschließen.

| Äußere Ebene | Innere Ebene | Erlaubt | Beispiel |
| --- | --- | --- | --- |
| AND | AND | Ja | E1 EXCLUDES: AND(AND(E4, E5), AND(C2)) |
| AND | AND/OR | Nein | E1 EXCLUDES: AND(AND(E2), OR(U1, U2, U3)) |
| AND | OR | Nein | E1 EXCLUDES: AND(OR(E7, E8, E9), OR(U1, U2)) |
| OR | AND | Nein | E1 EXCLUDES: OR(AND(E4), AND(E7, E8, E9)) |
| OR | AND/OR | Nein | E1 EXCLUDES: OR(AND(E4), OR(C1, C2)) |
| OR | OR | Nein | E1 EXCLUDES: OR(OR(E4), OR(C1, C2)) |
| OR (einzeln) | | Nein | E1 EXCLUDES: OR(AND(E2, E3)) E1 EXCLUDES: AND(OR(E2)) |
