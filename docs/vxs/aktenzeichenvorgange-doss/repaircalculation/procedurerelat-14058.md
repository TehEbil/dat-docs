---
title: "ProcedureRelatedParameters"
topic_id: "14058"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters"
---

# ProcedureRelatedParameters

Das Element <ProcedureRelatedParameters > dient zum Import/-Abrufen der Kalkulationsparameter der "Vorgangsbezogenen Daten".

ProcedureRelatedParameters ist eine Liste an Wertemengen, die folgende kalkulationsrelevante Faktoren modelliert:

1. [Allgemeine Faktoren](calculationfac-14061.md)
2. [Ersatzteilfaktoren](sparepartfacto-14062.md)
3. [Arbeitslohnfaktoren](labourcostfact-14063.md)
4. Lackfaktoren

   - [Lackfaktoren Eurolack](eurolacquerfac-14064.md)
   - [Lackfaktoren Herstellersystem](manufacturerla-14060.md)
   - [Lackfaktoren AZT](aztlacquerfact-14065.md)
   - [Lackfaktoren Centro Zaragoza](czlacquerfacto-14066.md)
   - [Lackfaktoren Cesvimap](cesvimaplacque-14067.md)
   - [Lackfaktoren Manuell](fullymanuallac-14068.md)
5. [Schadensteilungfaktoren](damagesegmenta-22902.md)

ProcedureRelatedParameters fungiert als parentNode und kann mit beliebig vielen [ProcedureRelatedParameter](procedurerelat-14059.md) bestückt werden. Die Struktur des [ProcedureRelatedParameter](procedurerelat-14059.md) Objektes ist immer gleich und hat eine Vielzahl an Attributen.
