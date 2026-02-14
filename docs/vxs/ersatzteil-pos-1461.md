---
title: "Ersatzteil-Positionen (SparePartPositions) ... (SparePartPosition)"
topic_id: "1461"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Ersatzteil-Positionen (SparePartPositions) ... (SparePartPosition)"
---

# Ersatzteil-Positionen (SparePartPositions) ... (SparePartPosition)

<SparePartPositions> ist ein Unterelement von <Dossier> und enthält die Informationen zu Ersatzteilen. <SparePartPosition> ist das Einzelelement.

Felder

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DATProcessId | Integer | DAT - Vorgangsnummer für einen Reparaturvorgang. |
| DATProcessName | String | DAT - Vorgangsnummer-Benennung |
| PartNumber | String | Ersatzteilnummer |
| Description | String | Ersatzteilbenennung |
| LastUPE | Decimal | Letzte unverbindliche Preisempfehlung lt. Hersteller |
| LastUPEDate | Decimal | Zeitpunkt der letzten unverbindlichen Preisempfehlung lt. Hersteller |
| SecondtoLastUPE | Decimal | Vorletzte unverbindliche Preisempfehlung lt. Hersteller |
| SecondtoLastUPEDate | Decimal | Zeitpunkt der vorletzten unverbindlichen Preisempfehlung lt. Hersteller |
| ThirdtoLastUPE | Decimal | Drittletzte unverbindliche Preisempfehlung lt. Hersteller |
| ThirdtoLastUPEDate | Decimal | Zeitpunkt der drittletzten unverbindlichen Preisempfehlung lt. Hersteller |
| FourthtoLastUPE | Decimal | Vierletzte unverbindliche Preisempfehlung lt. Hersteller |
| FourthtoLastUPEDate | Decimal | Zeitpunkt der viertletzten unverbindlichen Preisempfehlung lt. Hersteller |
| EquipmentPositions |  | [Ausstattungen zum Ersatzteil (EquipmentPositions)](#showid/1379 "Ausstattungen zum Ersatzteil (EquipmentPositions)") |
| WorkTimeMin | Decimal | Minimaler Kernaufwand in Stunden (Minuten im 100er-System); die Kernaufwände können aufgrund von Verbundarbeiten variieren, daher wird hier eine Spanne geliefert. Kommt nur zurück, wenn der COVERAGE-Parameter "COMPLETE" gesetzt ist (außer getModelInfoByMfrAndExtPartNo) |
| WorkTimeMax | Decimal | Maximaler Kernaufwand in Stunden (Minuten im 100er-System); die Kernaufwände können aufgrund von Verbundarbeiten variieren, daher wird hier eine Spanne geliefert. Kommt nur zurück, wenn der COVERAGE-Parameter "COMPLETE" gesetzt ist (außer getModelInfoByMfrAndExtPartNo) |
