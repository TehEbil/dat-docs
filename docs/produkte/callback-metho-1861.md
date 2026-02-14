---
title: "Callback-Methode für die Verarbeitung einer abgeschlossenen Fahrzeugauswahl"
topic_id: "1861"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Oberflächen-Schnittstelle > Integration der Oberfläche > Callback-Methode für die Verarbeitung einer abgeschlossenen Fahrzeugauswahl"
---

# Callback-Methode für die Verarbeitung einer abgeschlossenen Fahrzeugauswahl

Die Callback-Methode wird mit Klick auf den Weiter-Button auf der letzten Seite aufgerufen.
Sie übermittelt das Ergebnis der Fahrzeugauswahl am Ende des eingestellten Pageflow,
nachdem der Benutzer nach diesem eingestellten Pageflow eine Fahrzeugauswahl durchgeführt
hat.

Die Callback-Methode muss zuvor implementiert sein. Sie benötigt einen Parameter,
der das Ergebnis entgegennimmt. Das Ergebnis besteht aus einem XML-String. Der XML-String
entspricht dem DAT VXS-Schnittstellenformat und enthält eine Fahrzeugidentifikation
mit unterschiedlich großen Datenmengen. Dies ist abhängig vom eingestellten Pageflow:

- DAT €uropa-Code®, 15-stellig
- Marktindex (Container), 5-stellig
- Bauzeit, 4-stellig, DAT-Notation
- Typcode (sofern das entsprechende Recht hierzu vorhanden ist)
- Technische Daten
- Ausstattungen
- ...

Der XML-String ist wie folgt aufgebaut:

```
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
  <dossier xmlns:ns1="http://www.dat.de/vxs">
    <ns1:Vehicle>
      <ns1:VehicleIdentNumber/>
      <ns1:DatECode>019050850010006</ns1:DatECode>
      <ns1:ConstructionTime>4570</ns1:ConstructionTime>
      <ns1:InitialRegistration>2007-08-01+02:00</ns1:InitialRegistration>
      <ns1:VehicleTypeName>Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
      <ns1:ManufacturerName origin="dat">Volkswagen</ns1:ManufacturerName>
      <ns1:BaseModelName origin="dat">Golf VI (5K1)(10.2008-&gt;)</ns1:BaseModelName>
      <ns1:SubModelName origin="dat">Trendline</ns1:SubModelName>
      <ns1:VehicleType>1</ns1:VehicleType>
      <ns1:Manufacturer>905</ns1:Manufacturer>
      <ns1:BaseModel>85</ns1:BaseModel>
      <ns1:SubModel>1</ns1:SubModel>
      <ns1:Country>DE</ns1:Country>
      <ns1:VinActive>false</ns1:VinActive>
      <ns1:VinEquipmentChanged>false</ns1:VinEquipmentChanged>
      <ns1:VinChecksum/>
      <ns1:SubModelVariant>6</ns1:SubModelVariant>
      <ns1:RegistrationData><ns1:KbaCode>0603/AMB</ns1:KbaCode>
      </ns1:RegistrationData>
      <ns1:Engine>
        <ns1:EnginePowerKw origin="dat">75</ns1:EnginePowerKw>
        <ns1:EnginePowerHp origin="dat">101</ns1:EnginePowerHp>
        <ns1:Cylinders origin="dat">4</ns1:Cylinders>
        <ns1:Capacity origin="dat">1598</ns1:Capacity>
        <ns1:Consumption>7.4</ns1:Consumption>
        <ns1:Co2Emission>176.0</ns1:Co2Emission>
      </ns1:Engine>
      <ns1:TechInfo>
        <ns1:PowerHp origin="dat">102</ns1:PowerHp>
        <ns1:PowerKw origin="dat">75.0</ns1:PowerKw>
        <ns1:Capacity origin="dat">1598</ns1:Capacity>
        <ns1:Cylinder origin="dat">4</ns1:Cylinder>
        <ns1:CylinderArrangement origin="dat">R </ns1:CylinderArrangement>
        <ns1:GearboxType>manual</ns1:GearboxType>
        <ns1:ConsumptionInTown origin="dat">9.9</ns1:ConsumptionInTown>
        <ns1:ConsumptionOutOfTown origin="dat">6.8</ns1:ConsumptionOutOfTown>
        <ns1:Consumption origin="dat">7.4</ns1:Consumption>
        <ns1:Co2Emission origin="dat">176.0</ns1:Co2Emission>
        <ns1:InsuranceTypeClassLiability>16</ns1:InsuranceTypeClassLiability>
        <ns1:InsuranceTypeClassCascoPartial>17</ns1:InsuranceTypeClassCascoPartial>
        <ns1:InsuranceTypeClassCascoComplete>17</ns1:InsuranceTypeClassCascoComplete>
      </ns1:TechInfo>
      <ns1:Equipment>
        <ns1:SeriesEquipment>
          <ns1:EquipmentPosition>
            <ns1:DatEquipmentId>504</ns1:DatEquipmentId>
            <ns1:Description>Longlife-Service</ns1:Description>
          </ns1:EquipmentPosition>
          <ns1:EquipmentPosition>
            <ns1:DatEquipmentId>2904</ns1:DatEquipmentId>
            <ns1:Description>Nichtraucher-Paket</ns1:Description>
          </ns1:EquipmentPosition>
          <ns1:EquipmentPosition>
            <ns1:DatEquipmentId>15200</ns1:DatEquipmentId>
            <ns1:Description>Außenspiegel elektr. verstell- und heizbar</ns1:Description>
            <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
            <ns1:EquipmentType>glass</ns1:EquipmentType>
          </ns1:EquipmentPosition>
          <ns1:EquipmentPosition>
            <ns1:DatEquipmentId>15804</ns1:DatEquipmentId>
            <ns1:Description>Außenspiegel asphärisch, links</ns1:Description>
            <ns1:EquipmentType>glass</ns1:EquipmentType>
          </ns1:EquipmentPosition>
          <ns1:EquipmentPosition>
            <ns1:DatEquipmentId>18104</ns1:DatEquipmentId>
            <ns1:Description>Scheinwerfer: Hella</ns1:Description>
            <ns1:EquipmentType>glass</ns1:EquipmentType>
          </ns1:EquipmentPosition>
          <ns1:EquipmentPosition>
            <ns1:DatEquipmentId>18207</ns1:DatEquipmentId>
            <ns1:Description>Blinkleuchte in Außenspiegel integriert</ns1:Description>
            <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
            <ns1:EquipmentType>glass</ns1:EquipmentType>
          </ns1:EquipmentPosition>
          <ns1:EquipmentPosition>
            <ns1:DatEquipmentId>18904</ns1:DatEquipmentId>
            <ns1:Description>Tagfahrlicht</ns1:Description>
            <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
            <ns1:EquipmentType>glass</ns1:EquipmentType>
          </ns1:EquipmentPosition>
          <ns1:EquipmentPosition>
            <ns1:DatEquipmentId>22304</ns1:DatEquipmentId>
            <ns1:Description>Wärmeschutzverglasung grün getönt</ns1:Description>
            <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
            <ns1:EquipmentType>glass</ns1:EquipmentType>
          </ns1:EquipmentPosition>
          . . .
```

Je nach gesetztem Filter (Restriction), ist der Marktindex (Container) optional oder
zwingend vorhanden:

| Filter (Restriction) | Marktindex |
| --- | --- |
| ALL | Optional |
| REPAIR | Optional |
| APPRAISAL | Pflicht |

Die Bauzeit (ConstructionTime) ist nur dann gesetzt, wenn der Benutzer entweder eine
VIN-Abfrage durchgeführt hat oder die Bauzeit im entsprechenden Dialog in der DAT
€uropa-Code® Fahrzeugauswahl ausgewählt hat.

Die Callback-Methode muss vom Schnittstellenpartner so implementiert werden, dass
sie die Verarbeitung der zurückgelieferten Daten übernimmt oder auslöst. Dies kann
auf zwei Wegen erreicht werden:

- Die DAT €uropa-Code® Fahrzeugauswahl wird aus der bereits geladenen Seite entfernt, die Rückgabewerte
  werden via XMLHttpRequest an den Server des Schnittstellenpartners übermittelt und
  die Seite wird wieder mit Inhalten des Schnittstellenpartners befüllt.
- Die Rückgabewerte werden an eine andere HTML-Seite geschickt.

Ein einfaches Beispiel einer derartigen Callback-Methode sieht wie folgt aus:

```
<script type="text/javascript" language="JavaScript">
  function callbackFromSphinx ( object, xml ){
    //delete Sphinx iFrame from DOM-Tree
    sphinx.deleteIframe();
    //show return values
    alert ( "Vehicle selection is ready: " + xml.xml );
  }
</script>
```

Der Name der Callback-Methode ist frei wählbar.
