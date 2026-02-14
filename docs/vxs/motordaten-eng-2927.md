---
title: "Motordaten (Engine)"
topic_id: "2927"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Motordaten (Engine)"
---

# Motordaten (Engine)

<Engine> ist ein Unter-Element von <Vehicle> und enthält Informationen zum Motor.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| Description | string40 | Beschreibung / Motorname |
| EngineType | string30 | Motor-Art |
| CatalyticConverterType | string30 | Katalysator |
| GearType | string2 | Antriebsart |
| (Dat)FuelMethod | string | veraltet, bitte TechInfo.FuelMethod verwenden; Entfall seit 12/2017 geplant |
| (Dat)EnginePowerKw | integer | veraltet, bitte TechInfo.PowerKw verwenden |
| (Dat)EnginePowerHp | integer | veraltet, bitte TechInfo.PowerHp verwenden |
| (Dat)Cylinders | integer | veraltet, bitte TechInfo.Cylinder verwenden |
| (Dat)Capacity | integer | veraltet, bitte TechInfo.Capacity verwenden |
| PollutionClass | string | veraltet, bitte TechInfo.EmissionClassN verwenden |
| Consumption | decimal | veraltet, bitte TechInfo.Consumption verwenden |
| ConsumptionInTown | decimal | veraltet, bitte TechInfo.ConsumptionInTown verwenden |
| ConsumptionOutOfTown | decimal | veraltet, bitte TechInfo.ConsumptionOutOfTown verwenden |
| Co2Emission | decimal | veraltet, bitte TechInfo.Co2Emission verwenden |
