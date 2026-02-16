---
title: "Informationen über Crossborder-Fahrzeuge"
topic_id: "10860"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand VIN (VIN-Abfrage) > Informationen über Crossborder-Fahrzeuge"
---

# Informationen über Crossborder-Fahrzeuge

Wenn der Hersteller uns Informationen über das Bestimmungsland, für welches das Fahrzeug
gebaut wurde, zur Verfügung stellt, wird diese Information im Element VINResult hinterlegt. In solchen Fällen wird im Element VINEquipment ein Hersteller-Code (ManufacturerCode) mit dem Wert "Country:xx" ausgegeben, wobei "xx" für das zweistellige Länderkürzel
steht, für das das Fahrzeug gebaut wurde. Beispielsweise liefert die VIN-Abfrage mit
der Test-VIN WAUDEXTESTSTUB002 in ManufacturerCode den Wert Country:NL, das Fahrzeug wurde für den niederländischen Markt gebaut.

```
...
   <ns1:VINEquipments>
      ...
      <ns1:VINEquipment>
         <ns1:ManufacturerCode>C28</ns1:ManufacturerCode>
         <ns1:ShortName>Betriebserlaubnis Nachtrag</ns1:ShortName>
      </ns1:VINEquipment>
      <ns1:VINEquipment>
         <ns1:ManufacturerCode>Country:NL</ns1:ManufacturerCode>
      </ns1:VINEquipment>
      <ns1:VINEquipment>
         <ns1:ManufacturerCode>D92</ns1:ManufacturerCode>
         <ns1:ShortName>4-Zyl.Turbodieselmotor 2,0 L/105 KW(4V) TDI Common-Rail Grundmotor ist: TH3/TG3/TM4/TP4/TP5</ns1:ShortName>
      </ns1:VINEquipment>
      ...
   </ns1:VINEquipments>
...
```

Siehe hierzu auch unsere [Test-VIN allgemein](test-vin-allge-2015.md), dort haben wir weitere Beispiele für Reimport-Fahrzeuge dokumentiert.
