---
title: "Aktenzeichen/Vorgänge (Dossiers)"
topic_id: "1369"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers)"
---

# Aktenzeichen/Vorgänge (Dossiers)

Das Hauptelement des XML-Schemas ist <Dossiers>. Es darf nur einmal enthalten sein.

Attribute:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| source | string | Das System, das den Inhalt generiert hat, Für Importe in eine der Glas-Anwendungen: SD3. Für Importe aus Fremdanwendungen wird hier der Name der Anwendung vermerkt. |
| type | string | Die Art bzw. den Zweck der Generierung, etwa spezielle abgespeckte Börsenexporte, z.B. SparePartRequest, GlassRep.  Bei Übergabe an eine Glas-Anwendung muß - zusätzlich zum source=SD3 - einer der folgenden Werte in type gesetzt werden:  - glassrep.mbg für Mercedes-Benz Glas  - glassrep.vwg für Volkswagen Glas  - glassrep.sdg für SilverDAT calculateGlass  - glassrep.agp für autoglas Plus  - glassrep.aug für Audi Glas  - glassrep.nsg für Nissan Glas |
| [Dossier[]](aktenzeichenvorgang/index.md) | [Dossier[]](aktenzeichenvorgang/index.md) | Eine Liste von Einzelvorgängen bzw. [Dossier](aktenzeichenvorgang/index.md)s. |

## Bereiche

- [Aktenzeichen/Vorgang (Dossier)](aktenzeichenvorgang/index.md) (1 Topics)
- [Attachments](attachments/index.md) (1 Topics)
- [Bewertungsdaten (Valuation)](bewertungsdaten-valu/index.md) (7 Topics)
- [Bilder (ImageList)](bilder-imagelist/index.md) (1 Topics)
- [Fahrzeug (Vehicle)](fahrzeug-vehicle/index.md) (23 Topics)
- [Handelsdaten (TradingData)](handelsdaten-trading/index.md) (3 Topics)
- [Handelstätigkeit (TradingActivity)](handelstatigkeit-tra/index.md) (8 Topics)
- [Manuelle Positionen manualPositions](manuelle-positionen/index.md) (2 Topics)
- [RepairCalculation](repaircalculation/index.md) (66 Topics)
- [Reparaturauftrag (RepairOrder)](reparaturauftrag-rep/index.md) (2 Topics)
- [Weitere Handelsdaten (TradingAdditional)](weitere-handelsdaten/index.md) (32 Topics)

## Topics

- [ersatzteil-pos-1461](ersatzteil-pos-1461.md)
- [haufig-verwend-2925](haufig-verwend-2925.md)
- [images-images-1398](images-images-1398.md)
- [maintenanceint-1463](maintenanceint-1463.md)
- [umsatzsteuer-v-1400](umsatzsteuer-v-1400.md)
- [vertragsdaten-22797](vertragsdaten-22797.md)
