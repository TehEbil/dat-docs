---
title: "SparePartFactor"
topic_id: "14062"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > ProcedureRelatedParameter > SparePartFactor"
---

# SparePartFactor

Ersatzteilfaktoren

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| factor | attribute | Beschreibung | type | mode | Mögliche Werte |
| SparePartFactor | priceDate | Preisdatum | Date |  |  |
| SparePartFactor | increaseDecrease | Auf-/Abschlag (%) | Double |  | % [-999,00 bis 999,99] |
| SparePartFactor | surchargeInProtocolOly | ET-Zuschlag nur im Protokoll anzeigen | Boolean |  | true/false |
| SparePartFactor | surchargeSeparated | Ersatzteilzuschlag separat | Boolean |  | true/false |
| SparePartFactor | bracketSetRentCost | Miete Richtwinkelsatz (EUR) | Price | ABSOLUTE |  |
| SparePartFactor | bracketSetProcurementCost | Beschaffungskosten - Richtwinkelsatz (EUR) | Price | ABSOLUTE |  |
| SparePartFactor | procurementCost | Beschaffungskosten - Ersatzteile (EUR) | Price | ABSOLUTE |  |
| SparePartFactor | smallSparePartCalculationModel | K. bzw Verbrauchsmaterial Kalkulationsmodus | smallSparePartCalculationModel |  | FLAT / PERCENT\_OF\_PARTS |
| SparePartFactor | smallSparePartFlatRatePrice | K. bzw Verbrauchsmaterial - Pauschalbetrag | Price | ABSOLUTE |  |
| SparePartFactor | smallSparePartPercentOfPart | K. bzw Verbrauchsmaterial (%) | Double |  | % [0 bis 9,99] |
| SparePartFactor | bodyInWhiteProcurementCost | Beschaffungskosten - Rohbaukarosserie (EUR) | Price | ABSOLUTE |  |
| SparePartFactor | smallSparePartPercentOfPartBiw | K. bzw Verbrauchsmaterial (%) für Optimierung auf RBK | Double |  | % [0 bis 9,99] |
| SparePartFactor | smallSparePartPercentOfWageMax | Maximalwert Kleinmengenzuschlag in CHF, berechnet als Prozentsatz der Teile | Double |  |  |
| SparePartFactor | smallSparePartPercentOfWage | Kleinmengenzuschlag in Prozent des Lohns | Double |  |  |
| SparePartFactor | discount | Rabatt | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| SparePartFactor | discountBiw | Rabatt Optimierung auf RBK | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| SparePartFactor | sparePartLumpSum | Ersatzteile pauschal (EUR) | Price | ABSOLUTE |  |
| SparePartFactor | newForOld | Pauschaler Neu für Alt Abzug auf Ersatzteile | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
