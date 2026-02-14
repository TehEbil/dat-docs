---
title: "Requires"
topic_id: "15786"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Datenbezug > Logik > Validierungsregeln > Requires"
---

# Requires

| Äußere Ebene | Innere Ebene | Beispiel | Obligatorische Parameter im Aufruf, wenn auch O1 angegeben ist |
| --- | --- | --- | --- |
| AND | AND | O1 REQUIRES: AND(AND(O4, O5), AND(C2)) | O4, O5, C2 |
| AND | AND/OR | O1 REQUIRES: AND(AND(O2), OR(U1, U2, U3)) | O2  genau einer von U1, U2 oder U3 |
| AND | OR | O1 REQUIRES: AND(OR(O7, O8, O9), OR(U1, U2)) | 1. genau einer von O7, O8 oder O9  2. genau einer von U1, U2 |
| OR | AND | O1 REQUIRES: OR(AND(O4), AND(O7, O8, O9)) | entweder O4 oder alle von O7, O8 und O9 |
