---
title: "Response getFillingQuantities"
topic_id: "22901"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abrufen der Füllmengen anhand des DAT €urope-Codes > Response getFillingQuantities"
---

# Response getFillingQuantities

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns4:getFillingQuantitiesResponse xmlns:ns4="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
         <FillingQuantities xmlns:ns1="http://www.dat.de/vxs">
            <ns1:Fluid desc="Hydraulische Betätigung, Getriebe" type="3">
               <ns1:Capacity desc="Füllmenge (gesamt)" min="0.50" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Product>PENTOSIN CHF 11S</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid desc="Hinterachsgetriebe" type="3">
               <ns1:Capacity desc="Füllmenge (gesamt)" max="1.60" min="1.00" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Product>TITAN SINTOPOID FE SAE 75W-85 (XTL-Technology)</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid desc="Servolenkung" type="6">
               <ns1:Capacity desc="Füllmenge (gesamt)" min="1.10" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Product>PENTOSIN CHF 11S</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid desc="Hydraulisches Brems-/Kupplungssystem" type="4">
               <ns1:Capacity desc="Füllmenge (gesamt)" max="2.25" min="1.40" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Interval type="1">Wechseln 24 Monate</ns1:Interval>
                  <ns1:Product>MAINTAIN DOT 5.1</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid code="646.82x" desc="Motor" type="1">
               <ns1:Capacity desc="Füllmenge (gesamt)" min="6.50" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Interval type="1">Wechseln 25000 km/ 12 Monate</ns1:Interval>
                  <ns1:Product>TITAN GT1 PRO FLEX SAE 5W-30 (XTL-Technology)</ns1:Product>
                  <ns1:Product>TITAN GT1 SAE 5W-40 (XTL-Technology)</ns1:Product>
                  <ns1:Product>TITAN GT1 PRO C-3 SAE 5W-30 (XTL-Technology)</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid desc="Kühlsystem" type="8">
               <ns1:Capacity desc="Füllmenge (gesamt)" min="6.70" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Interval type="1">Wechseln 250000 km/ 180 Monate</ns1:Interval>
                  <ns1:Product>MAINTAIN FRICOFIN DP</ns1:Product>
                  <ns1:Product>MAINTAIN FRICOFIN</ns1:Product>
                  <ns1:Product>MAINTAIN FRICOFIN -35 (Ready-Mix)</ns1:Product>
                  <ns1:Product>MAINTAIN FRICOFIN DP -35 (Ready-Mix)</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid code="722.6xx 5/1" desc="Automatikgetriebe" type="3">
               <ns1:Capacity desc="Füllmenge (gesamt)" max="8.00" min="7.50" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="3452">Nur bei erstem Wechsel</ns1:Usage>
                  <ns1:Interval type="1">Wechseln 60000 km</ns1:Interval>
                  <ns1:Product>TITAN ATF 4134</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid code="716.6xx 6/1" desc="Schaltgetriebe" type="3">
               <ns1:Capacity desc="Füllmenge (gesamt)" min="1.50" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Product>TITAN SINTOFLUID FE SAE 75W</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid desc="Kühlsystem" type="8">
               <ns1:Capacity desc="Füllmenge (gesamt)" min="6.70" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Interval type="1">Wechseln 250000 km/ 180 Monate</ns1:Interval>
                  <ns1:Product>MAINTAIN FRICOFIN</ns1:Product>
                  <ns1:Product>MAINTAIN FRICOFIN DP -35 (Ready-Mix)</ns1:Product>
                  <ns1:Product>MAINTAIN FRICOFIN DP</ns1:Product>
                  <ns1:Product>MAINTAIN FRICOFIN -35 (Ready-Mix)</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid desc="Hydraulische Betätigung, Getriebe" type="3">
               <ns1:Capacity desc="Füllmenge (gesamt)" min="0.50" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Product>PENTOSIN CHF 11S</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid desc="Hinterachsgetriebe" type="3">
               <ns1:Capacity desc="Füllmenge (gesamt)" max="1.60" min="1.00" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Product>TITAN SINTOPOID FE SAE 75W-85 (XTL-Technology)</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid desc="Servolenkung" type="6">
               <ns1:Capacity desc="Füllmenge (gesamt)" min="1.10" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Product>PENTOSIN CHF 11S</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid desc="Hydraulisches Brems-/Kupplungssystem" type="4">
               <ns1:Capacity desc="Füllmenge (gesamt)" max="2.25" min="1.40" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Interval type="1">Wechseln 24 Monate</ns1:Interval>
                  <ns1:Product>MAINTAIN DOT 5.1</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid code="646.82x" desc="Motor" type="1">
               <ns1:Capacity desc="Füllmenge (gesamt)" min="6.50" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="3782">Flexibel (max)</ns1:Usage>
                  <ns1:Product>TITAN GT1 PRO C-3 SAE 5W-30 (XTL-Technology)</ns1:Product>
                  <ns1:Product>TITAN GT1 SAE 5W-40 (XTL-Technology)</ns1:Product>
                  <ns1:Product>TITAN GT1 PRO FLEX SAE 5W-30 (XTL-Technology)</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid code="722.6xx 5/1" desc="Automatikgetriebe" type="3">
               <ns1:Capacity desc="Füllmenge (gesamt)" max="8.00" min="7.50" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="3452">Nur bei erstem Wechsel</ns1:Usage>
                  <ns1:Interval type="1">Wechseln 60000 km</ns1:Interval>
                  <ns1:Product>TITAN ATF 4134</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
            <ns1:Fluid code="716.6xx 6/1" desc="Schaltgetriebe" type="3">
               <ns1:Capacity desc="Füllmenge (gesamt)" min="1.50" unit="Liter"/>
               <ns1:Recommendation>
                  <ns1:Usage type="0">Normal</ns1:Usage>
                  <ns1:Product>TITAN SINTOFLUID FE SAE 75W</ns1:Product>
               </ns1:Recommendation>
            </ns1:Fluid>
         </FillingQuantities>
      </ns4:getFillingQuantitiesResponse>
   </S:Body>
</S:Envelope>
```
