---
title: "Laufende Kosten (RunningExpenses)"
topic_id: "2939"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Laufende Kosten (RunningExpenses)"
---

# Laufende Kosten (RunningExpenses)

<RunningExpenses> ist ein Unter-Element von <Vehicle> und enthält Informationen zu den laufenden Kosten (Versicherung und Steuern).

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| (Dat)LiabilityInsuranceTypeClass | string | Versicherungsklasse Haftpflicht |
| (Dat)PartialCascoTypeClass | string | Versicherungsklasse Teilkasko |
| (Dat)ComprCascoTypeClass | string | Versicherungsklasse Vollkasko |
| TaxationDescription | string | KFZ-Steuereinteilung |
| (Dat)TaxPerYear | decimal | KFZ-Steuer pro Jahr |
| (Dat)TaxPer100ccm | decimal | KFZ-Steuer pro 100cm³ |
