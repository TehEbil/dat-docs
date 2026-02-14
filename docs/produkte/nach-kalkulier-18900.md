---
title: "(Nach-) Kalkulieren eines bestehenden Vorgangs"
topic_id: "18900"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > (Nach-) Kalkulieren eines bestehenden Vorgangs"
---

# (Nach-) Kalkulieren eines bestehenden Vorgangs

Mit der Funktion calculateContract() kann ein Vorgang in SilverDAT calculatePro oder SilverDAT calculateEypert kalkuliert werden. calculateContract() kann nur im Nachgang zu [importDossier()](#showid/1367 "Erstellen, Aktualisiern und Überschreiben eines Vorgangs") durchgeführt werden, weil die contractId, die von [importDossier](#showid/1367 "Erstellen, Aktualisiern und Überschreiben eines Vorgangs")() zurückgegeben wird, ein Pflichtparameter von calculateContract() ist.

Diese Funktion dient der Vereinheitlichung der Schnittstelle und wird zukünftig die
calculateContractN() ersetzen.

Parameter

| Name / Elternelement | Datentyp | Beschreibung |
| --- | --- | --- |
| contractID | Long, Pflicht | Vorgangsnummer |
| includeAttachments | Boolean (default: false), optional | Kennzeichen, ob Anhänge exportiert werden sollen |
| locale | Locale, optional | Datenland, Land- und Spracheinstellung |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [Dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") | [Dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") | Enthält das Fahrzeugobjekt, die Kalkulationsfaktoren, die Schadenspositionen und das Kalkulationssergebnis |

Als Antwort wird eine komplette Kalkulation, inklusive Ölfüllstandsmengen, wie folgt
zurückgeliefert:

```
Dossier
    DatCustomerAddress
    Vehicle
        RegistrationData
        Engine
        TechInfo
            FillingQuantities
        Equipment
```

```
        Tires
```

```
        VINResult
    VAT
    TradingData
        Owner
        Opponent
        ClientContactAddresses
    RepairCalculation
        Vehicle
            RegistrationData
            Engine
            TechInfo
                FillingQuantities
            Equipment
```

```
            Tires
```

```
            VINResult
        ProcedureRelatedParameters
        RepairPositions
        CalcResultCommon
            MaterialPositions
            LabourPositions
            LacquerPositions
            RepairCalculationSummary
        CalculationSummary
    RepairOrder
```

|  |  |
| --- | --- |
| Name | calculateContract |
| Use | literal |
| Style | document |
| One-Way | false |
| SOAP Action | calculateContract |
| Message Name | calculateContract |
| Part Name | parameters |
| Part Type | Element (tns:calculateContract mit tns= http://sphinx.dat.de/services/VehicleRepairService) |
