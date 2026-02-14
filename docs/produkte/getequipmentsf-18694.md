---
title: "getEquipmentsForUniversalSubType"
topic_id: "18694"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getEquipmentsForUniversalSubType"
---

# getEquipmentsForUniversalSubType

In unseren Anwendungen steht die neue Schnittstellenfunktion getEquipmentsForUniversalSubType
zur Auswahl der Sammeluntertypen (Variante A) zur Verfügung.

Die Schnittstellenfunktion getEquipmentsForUniversalSubType ist ausschließlich über REST verfügbar!  
Die Verwendung dieser Funktion ist nur für die Schadenskalkulation sinnvoll.

Beschreibung

Mit Hilfe dieser Funktion ist der Schnittstellenpartner in der Lage, seinen Kunden
bzgl. Sammeluntertyp dieselbe Auswahl bzgl. Untertyp und Ausstattungen anzubieten,
wie es die Oberfläche der Fahrzeugauswahl macht:

Der Anwender kann nun durch Auswahl der Ausstattungen den Untertyp einschränken, wenn
er möchte. Im Ergebnis der Schnittstellenfunktion besagt die Aufzählung im Inhalt
des Feldes „subModels", für welchen der Untertypen eine betreffende Ausstattung denkbar
ist.

VXS

Nachdem der Anwender des Schnittstellenpartners seine Auswahl getätigt hat, kann der
Schnittstellenpartner ein entsprechendes VXS zusammenbauen, wobei hier folgende Felder
wichtig sind:

Manueller Namen des Untertyps:

```
<ns2:SubModelName origin="user">mein Untertyp</ns2:SubModelName>
```

Situation "Sammeluntertyp" ist eingeschaltet:

```
<ns2:IsUniversalSubModel>true</ns2:IsUniversalSubModel>
```

Und die Ausstattungen, die der Anwender wollte:

```
<ns2:Equipment>
    <ns2:SeriesEquipment>
        <ns2:EquipmentPosition>
            <ns2:DatEquipmentId>2701</ns2:DatEquipmentId>
            <ns2:Description>Aerodynamik-Paket M-Technic</ns2:Description>
            <ns2:AddedByLogikCheck>false</ns2:AddedByLogikCheck>
        </ns2:EquipmentPosition>

        <!-- … more … --!>

    </ns2:SeriesEquipment>
</ns2:Equipment>
```

Bei den Ausstattungen gibt es im Falle „Sammeluntertyp" keine Unterscheidung bzgl.
Serien- und Sonderausstattungen. Von daher kann der Schnittstellenpartner alle Ausstattungen
als Serienausstattungen eintragen.

VXS-Import

Ein dermaßen vorbereitetes VXS kann dann in den VXS-Importen der Calculate-Anwendungen
genutzt werden, z.B. durch einen Import per Datei.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| Restriction | Enumeration | REPAIR | Bitte nur REPAIR verwenden! | X |
| vehicleType | Integer | [getVehicleTypes](#showid/1904 "getVehicleTypes") | Fahrzeugart | X |
| Manufacturer | Integer | [getManufacturers](#showid/1834 "getManufacturers") | Hersteller | X |
| BaseModel | Integer | [getBaseModels](#showid/1838 "getBaseModelsN") | Haupttyp | X |

Rückgabe

Die Rückgabe umfasst die Liste der möglichen Untertypen und die Liste der möglichen
Ausstattungen. Sind für Ausstattungen Ausstattungsklassen vorhanden, werden diese
mit dem Schlüsselwort "equClass" ausgegeben.

Beispiel:

```
{
    "equClass": 11,
    "datEquipmentId": 75005,
    "description": "Getriebe 5-Gang",
    "subModels": [1, 2, 3]
}
```

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>/getEquipmentsForUniversalSubType

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | rest | VehicleSelectionService |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | rest | VehicleSelectionService |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | rest | VehicleSelectionService |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | rest | VehicleSelectionService |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | rest | VehicleSelectionService |
