---
title: "DAT €uropa-Code Ausstattungen (DATECodeEquipment)"
topic_id: "2940"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > DAT €uropa-Code Ausstattungen (DATECodeEquipment)"
---

# DAT €uropa-Code Ausstattungen (DATECodeEquipment)

Sind die zu der UTV gehörenden Ausstattungen und bilden mit den folgenden Feldern
die Beschreibung des DAT €uropa-Code® inkl. Markindex.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| (Dat)BaseModelName | string | Haupttypname |
| (Dat)SubModelName | string | Untertypname |
| (Dat)VehicleTypeName | string | Fahrzeugartname |
| (Dat)ContainerName | string | Name/Benennung des Container |
| (Dat)ManufacturerName | string | Herstellername |

Der Inhalt einer [EquipmentPosition](#showid/1381 "Ausstattungen (Equipment, …Equipment, EquipmentPosition)") ist hier:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DatEquipmentId | long | Nummer der Ausstattungsvariante |
| Description | string | Beschreibung |

Beispiel:

```
                       <DATECodeEquipment>
                        <ns3:EquipmentPosition>
                           <DatEquipmentId>92600</DatEquipmentId>
                           <Description>Motor 3,2 Ltr. - 191 kW V6 24V KAT (BPK)</Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <DatEquipmentId>75703</DatEquipmentId>
                           <Description>Getriebe Automatik - Multitronic</Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <DatEquipmentId>10004</DatEquipmentId>
                           <Description>Karosserie: 4-türig</Description>
                        </ns3:EquipmentPosition>
                     </DATECodeEquipment>
```
