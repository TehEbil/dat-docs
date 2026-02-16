---
title: "Excludes"
topic_id: "15783"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Logik > Logische Begriffe > Excludes"
---

# Excludes

Die Bedeutung einer "Excludes"-Definition ist, dass wenn der Kunde die aktuelle Ausstattungsposition
kauft, die Ausstattungspositionen, die dadurch ausgeschlossen werden, nicht gleichzeitig
gekauft werden dürfen.

ODER-Kombinationen von Positionen sind nicht erlaubt: Eine Ausstattungsposition kann
andere nur bedingungslos ausschließen.

| Äußere Ebene | Innere Ebene | Erlaubt | Beispiel |
| --- | --- | --- | --- |
| AND | AND | Ja | O1 EXCLUDES: AND(AND(O4, O5), AND(C2)) |
| AND | AND/OR | Nein | O1 EXCLUDES: AND(AND(O2), OR(U1, U2, U3)) |
| AND | OR | Nein | O1 EXCLUDES: AND(OR(O7, O8, O9), OR(U1, U2)) |
| OR | AND | Nein | O1 EXCLUDES: OR(AND(O4), AND(O7, O8, O9)) |
| OR | AND/OR | Nein | O1 EXCLUDES: OR(AND(O4), OR(C1, C2)) |
| OR | OR | Nein | O1 EXCLUDES: OR(OR(O4), OR(C1, C2)) |
| OR (einzeln) | | Nein | O1 EXCLUDES: OR(AND(O2, O3)) O1 EXCLUDES: AND(OR(O2)) |
