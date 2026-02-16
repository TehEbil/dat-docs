---
title: "(Nach-) Kalkulieren eines bestehenden Vorgangs"
topic_id: "18905"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > (Nach-) Kalkulieren eines bestehenden Vorgangs"
---

# (Nach-) Kalkulieren eines bestehenden Vorgangs

Mit der Funktion calculateContract() kann ein Vorgang in SilverDAT 3 PRO kalkuliert werden. calculateContract() kann nur im Nachgang zu [importDossier()](../../silverdat-calculatepro-si/schnittstellenoperat/erstellen-aktu-1367.md) durchgeführt werden, weil die contractId, die von [importDossier](../../silverdat-calculatepro-si/schnittstellenoperat/erstellen-aktu-1367.md)() zurückgegeben wird, ein Pflichtparameter von calculateContract() ist.

Diese Funktion dient der Vereinheitlichung der Schnittstelle und wird zukünftig die
calculateContractN() ersetzen.

Parameter

| Name / Elternelement | Datentyp | Beschreibung |
| --- | --- | --- |
| contractID | Long, Pflicht | Vorgangsnummer |
| includeAttachments | Boolean (default: false),  Optional | Kennzeichen, ob Anhänge exportiert werden sollen |
| locale | locale, optional | Datenland, Land- und Spracheinstellung |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [Dossier](../../../vxs/aktenzeichenvorgange-doss/aktenzeichenvorgang/index.md) | [Dossier](../../../vxs/aktenzeichenvorgange-doss/aktenzeichenvorgang/index.md) | Enthält das Fahrzeugobjekt, die Arbeitslöhne, Kalkulationsfaktoren, Schadenspositionen und das Kalkulationssergebnis |

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
        RepairWages
        RepairParameters
```

```
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
