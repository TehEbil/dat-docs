---
title: "Requires"
topic_id: "27935"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Logik > Validierungsregeln > Requires"
---

# Requires

| Äußere Ebene | Innere Ebene | Beispiel | Obligatorische Parameter im Aufruf, wenn auch E1 angegeben ist |
| --- | --- | --- | --- |
| AND | AND | E1 REQUIRES: AND(AND(E4, E5), AND(C2)) | E4, E5, C2 |
| AND | AND/OR | E1 REQUIRES: AND(AND(E2), OR(U1, U2, U3)) | 1. E2  2. genau einer von U1, U2 oder U3 |
| AND | OR | E1 REQUIRES: AND(OR(E7, E8, E9), OR(U1, U2)) | 1. genau einer von E7, E8 oder E9  2. genau einer von U1, U2 |
| OR | AND | E1 REQUIRES: OR(AND(E4), AND(E7, E8, E9)) | entweder E4 oder alle von E7, E8 und E9 |
