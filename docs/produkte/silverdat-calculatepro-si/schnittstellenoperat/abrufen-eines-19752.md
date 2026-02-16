---
title: "Abrufen eines Kalkulationsergebnisses"
topic_id: "19752"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen eines Kalkulationsergebnisses"
---

# Abrufen eines Kalkulationsergebnisses

Die Funktion getCalculationResultN() dient dem Abrufen der Kalkulationsergebnisse eines in SilverDAT calculatePro vorhandenen Vorgangs. Üblicherweise wird ein solcher Vorgang wie unter Anlage eines neuen Vorgangs beschrieben erzeugt und dann von einem Benutzer bearbeitet und kalkuliert. Nach erfolgter
Kalkulation können mit getCalculationResultN() bspw. die Ersatzteilinformationen durch ein Fremdsystem ausgelesen werden.

Im Vergleich zur alten Funktion getCalculationResults(), werden die Eingabeparameter zusätzlich mit dem Element <request> umrandet. Die neue Funktion dient weiterhin dem Abruf der Kalkulationsergebnisse.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| contractID | Long, Pflicht |  | Vorgangsnummer |
| locale | Locale, optional |  | [Element locale](../../../allgemein/dat-developers-guide/arbeiten-mit-den-web/element-locale-1352.md) |
| includeAttachments | Boolean, optional | true | false  Defaultwert: false | Kennzeichen, ob Anhänge exportiert werden sollen |
| includeProtocol | Boolean, optional | true | false  Defaultwert: false | Kennzeichen, ob Protokoll exportiert werden soll |

Als Eingabe dient dabei die Vorgangsnummer (contractID), die wie unter Anlage eines neuen Vorgangs beschrieben erlangt werden kann. Optional kann auch der Parameter "[locale](../../../allgemein/dat-developers-guide/arbeiten-mit-den-web/element-locale-1352.md)" mit übergeben werden. Dadurch lässt sich das Kalkulationsergebnis in der gewünschten
Sprache abrufen.

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [Dossiers](../../../vxs/aktenzeichenvorgange-doss/index.md) | [Dossiers](../../../vxs/aktenzeichenvorgange-doss/index.md) | Fahrzeugdossier inkl. Kalkulationsergebnis |

Als Rückgabe wird ein so genanntes „Fahrzeugdossier" zurückgeliefert. Dieses Dossier
ist im so genannten VXS-Format gehalten. Folgende Informationsblöcke werden zurückgegeben:

```
Dossier
    DatCustomerAddress
    Vehicle
        RegistrationData
        TechInfo
            FillingQuantities
        Equipment
    VAT
    TradingData
        Owner
        Opponent
    RepairCalculation
        Vehicle
        RepairWages
        RepairParameters
        ProcedureRelatedParameters
        RepairPositions
        CalcResultCommon
            MaterialPositions
            LabourPositions
            LacquerPositions
            RepairCalculationSummary
    RepairOrder
```

Bitte beachten Sie im getCalculationResultNResponse, dass im Falle der Lackiermethode AZT die Arbeitszeiten bei den Positionen der Lackierung (Tag „LacquerPosition") immer in Stunden angegeben werden, trotz Vorgabe eines anderen Zeitmaßes.

Die detaillierte Beschreibung dieses Formats und seiner Felder finden Sie im Kapitel
"VXS".

|  |  |
| --- | --- |
| Name | getCalculationResultN |
| Use | literal |
| Style | document |
| One-Way | false |
| SOAP Action | getCalculationResultN |
| Message Name | getCalculationResultN |
| Part Name | parameters |
| Part Type | Element (tns:getCalculationResultN mit tns= http://sphinx.dat.de/services/VehicleRepairService) |
