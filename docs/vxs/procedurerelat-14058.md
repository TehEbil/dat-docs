---
title: "ProcedureRelatedParameters"
topic_id: "14058"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters"
---

# ProcedureRelatedParameters

Das Element <ProcedureRelatedParameters > dient zum Import/-Abrufen der Kalkulationsparameter der "Vorgangsbezogenen Daten".

ProcedureRelatedParameters ist eine Liste an Wertemengen, die folgende kalkulationsrelevante Faktoren modelliert:

1. [Allgemeine Faktoren](#showid/14061 "CalculationFactor")
2. [Ersatzteilfaktoren](#showid/14062 "SparePartFactor")
3. [Arbeitslohnfaktoren](#showid/14063 "LabourCostFactor")
4. Lackfaktoren

   - [Lackfaktoren Eurolack](#showid/14064 "EuroLacquerFactor")
   - [Lackfaktoren Herstellersystem](#showid/14060 "ManufacturerLacquerFactor")
   - [Lackfaktoren AZT](#showid/14065 "AztLacquerFactor")
   - [Lackfaktoren Centro Zaragoza](#showid/14066 "CzLacquerFactor")
   - [Lackfaktoren Cesvimap](#showid/14067 "CesvimapLacquerFactor")
   - [Lackfaktoren Manuell](#showid/14068 "FullyManualLacquerFactor")
5. [Schadensteilungfaktoren](#showid/22902 "DamageSegmentationFactor")

ProcedureRelatedParameters fungiert als parentNode und kann mit beliebig vielen [ProcedureRelatedParameter](#showid/14059 "ProcedureRelatedParameter") bestückt werden. Die Struktur des [ProcedureRelatedParameter](#showid/14059 "ProcedureRelatedParameter") Objektes ist immer gleich und hat eine Vielzahl an Attributen.
