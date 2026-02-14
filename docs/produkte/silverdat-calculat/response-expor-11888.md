---
title: "Response exportManualPositions"
topic_id: "11888"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Exportieren von manuellen Positionen > Response exportManualPositions"
---

# Response exportManualPositions

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns4:exportManualPositionsResponse xmlns:ns4="http://sphinx.dat.de/services/VehicleRepairService">
         <manualPositions xmlns:ns1="http://www.dat.de/vxs">
            <ns1:DatCategory>
               <ns1:DatPosition>
                  <ns1:Country>A</ns1:Country>
                  <ns1:Designation>sdf</ns1:Designation>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>A</ns1:Country>
                  <ns1:Designation>asd</ns1:Designation>
               </ns1:DatPosition>
               <ns1:name>My Manual Motorhaube</ns1:name>
            </ns1:DatCategory>
            <ns1:DatCategory>
               <ns1:name>Hagelschaden ATUM (fuer PL)</ns1:name>
            </ns1:DatCategory>
            <ns1:DatCategory>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Price>123000</ns1:Price>
                  <ns1:Designation>Test M with lump</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:DiscountPercentage>123000</ns1:DiscountPercentage>
                  <ns1:Nfa>123000</ns1:Nfa>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test M with Time</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:DiscountPercentage>123000</ns1:DiscountPercentage>
                  <ns1:Nfa>123000</ns1:Nfa>
                  <ns1:Worktime>123000</ns1:Worktime>
                  <ns1:LacquerMaterial>123000</ns1:LacquerMaterial>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Price>123000</ns1:Price>
                  <ns1:Designation>Test N</ns1:Designation>
                  <ns1:DiscountPercentage>123000</ns1:DiscountPercentage>
                  <ns1:Worktime>123000</ns1:Worktime>
                  <ns1:WorkLevel>0</ns1:WorkLevel>
                  <ns1:WorkType>3</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test O</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:Worktime>123000</ns1:Worktime>
                  <ns1:WorkLevel>1</ns1:WorkLevel>
                  <ns1:WorkType>60</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test P</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:Worktime>123000</ns1:Worktime>
                  <ns1:WorkLevel>0</ns1:WorkLevel>
                  <ns1:WorkType>3</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test S</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:Worktime>123000</ns1:Worktime>
                  <ns1:WorkLevel>0</ns1:WorkLevel>
                  <ns1:WorkType>2</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test T</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:Worktime>123000</ns1:Worktime>
                  <ns1:WorkLevel>1</ns1:WorkLevel>
                  <ns1:WorkType>2</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test Z</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:Worktime>123000</ns1:Worktime>
                  <ns1:WorkLevel>0</ns1:WorkLevel>
                  <ns1:WorkType>1</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>TestF</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:Worktime>123000</ns1:Worktime>
                  <ns1:WorkLevel>0</ns1:WorkLevel>
                  <ns1:WorkType>2</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>amount L</ns1:Designation>
                  <ns1:Worktime>100</ns1:Worktime>
                  <ns1:LacquerMaterial>1000</ns1:LacquerMaterial>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test A</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:Worktime>1000</ns1:Worktime>
                  <ns1:WorkLevel>0</ns1:WorkLevel>
                  <ns1:WorkType>-1</ns1:WorkType>
                  <ns1:SupplementDifficulty>1000</ns1:SupplementDifficulty>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Price>123000</ns1:Price>
                  <ns1:Designation>Test / plastic</ns1:Designation>
                  <ns1:Worktime>123000</ns1:Worktime>
                  <ns1:WorkLevel>1</ns1:WorkLevel>
                  <ns1:WorkType>3</ns1:WorkType>
                  <ns1:RepairType>plastic</ns1:RepairType>
                  <ns1:CountLevelS>1</ns1:CountLevelS>
                  <ns1:CountLevelM>2</ns1:CountLevelM>
                  <ns1:CountLevelL>3</ns1:CountLevelL>
                  <ns1:CountLevelGlass>1</ns1:CountLevelGlass>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test / glass</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:WorkLevel>-1</ns1:WorkLevel>
                  <ns1:WorkType>-1</ns1:WorkType>
                  <ns1:RepairType>glass</ns1:RepairType>
                  <ns1:CountLevelS>0</ns1:CountLevelS>
                  <ns1:CountLevelM>0</ns1:CountLevelM>
                  <ns1:CountLevelL>0</ns1:CountLevelL>
                  <ns1:CountLevelGlass>3</ns1:CountLevelGlass>
                  <ns1:FlatRateValue>123000</ns1:FlatRateValue>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test / all</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:WorkLevel>-1</ns1:WorkLevel>
                  <ns1:WorkType>-1</ns1:WorkType>
                  <ns1:RepairType>general</ns1:RepairType>
                  <ns1:CountLevelS>0</ns1:CountLevelS>
                  <ns1:CountLevelM>0</ns1:CountLevelM>
                  <ns1:CountLevelL>0</ns1:CountLevelL>
                  <ns1:CountLevelGlass>1</ns1:CountLevelGlass>
                  <ns1:FlatRateValue>123000</ns1:FlatRateValue>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Price>12223000</ns1:Price>
                  <ns1:Designation>Test L mit pauschal</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:DiscountPercentage>12000</ns1:DiscountPercentage>
                  <ns1:Nfa>123000</ns1:Nfa>
                  <ns1:FlatRateValue>123000</ns1:FlatRateValue>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test L with time</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:DiscountPercentage>12000</ns1:DiscountPercentage>
                  <ns1:Nfa>12000</ns1:Nfa>
                  <ns1:Worktime>12000</ns1:Worktime>
                  <ns1:LacquerMaterial>123000</ns1:LacquerMaterial>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test I</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:Worktime>12300</ns1:Worktime>
                  <ns1:WorkLevel>1</ns1:WorkLevel>
                  <ns1:WorkType>2</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Price>200</ns1:Price>
                  <ns1:Designation>Test E</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:UsedPart>1</ns1:UsedPart>
                  <ns1:DiscountPercentage>100</ns1:DiscountPercentage>
                  <ns1:Nfa>100</ns1:Nfa>
                  <ns1:WorkLevel>0</ns1:WorkLevel>
                  <ns1:WorkType>3</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test D</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:Worktime>1000</ns1:Worktime>
                  <ns1:WorkLevel>0</ns1:WorkLevel>
                  <ns1:WorkType>-1</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:DatPosition>
                  <ns1:Country>D</ns1:Country>
                  <ns1:Designation>Test B</ns1:Designation>
                  <ns1:PreDamage>1</ns1:PreDamage>
                  <ns1:Worktime>1000</ns1:Worktime>
                  <ns1:WorkLevel>0</ns1:WorkLevel>
                  <ns1:WorkType>-1</ns1:WorkType>
               </ns1:DatPosition>
               <ns1:name>TestCategory</ns1:name>
            </ns1:DatCategory>
            <ns1:DatCategory>
               <ns1:name>HRK (fuer PL)</ns1:name>
            </ns1:DatCategory>
            <ns1:DatCategory>
               <ns1:name>new</ns1:name>
            </ns1:DatCategory>
            <ns1:DatCategory>
               <ns1:name>Hagelschaden (Ford) (fur PL)</ns1:name>
            </ns1:DatCategory>
            <ns1:DatPosition>
               <ns1:Country>A</ns1:Country>
               <ns1:Designation>sdf</ns1:Designation>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>A</ns1:Country>
               <ns1:Designation>asd</ns1:Designation>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>D</ns1:Country>
               <ns1:Designation>Test B</ns1:Designation>
               <ns1:PreDamage>1</ns1:PreDamage>
               <ns1:Worktime>1000</ns1:Worktime>
               <ns1:WorkLevel>0</ns1:WorkLevel>
               <ns1:WorkType>-1</ns1:WorkType>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>D</ns1:Country>
               <ns1:Designation>Test D</ns1:Designation>
               <ns1:PreDamage>1</ns1:PreDamage>
               <ns1:Worktime>1000</ns1:Worktime>
               <ns1:WorkLevel>0</ns1:WorkLevel>
               <ns1:WorkType>-1</ns1:WorkType>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>A</ns1:Country>
               <ns1:Designation>sdf</ns1:Designation>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>A</ns1:Country>
               <ns1:Designation>asd</ns1:Designation>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>D</ns1:Country>
               <ns1:Designation>Test B</ns1:Designation>
               <ns1:PreDamage>1</ns1:PreDamage>
               <ns1:Worktime>1000</ns1:Worktime>
               <ns1:WorkLevel>0</ns1:WorkLevel>
               <ns1:WorkType>-1</ns1:WorkType>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>D</ns1:Country>
               <ns1:Designation>Test D</ns1:Designation>
               <ns1:PreDamage>1</ns1:PreDamage>
               <ns1:Worktime>1000</ns1:Worktime>
               <ns1:WorkLevel>0</ns1:WorkLevel>
               <ns1:WorkType>-1</ns1:WorkType>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>D</ns1:Country>
               <ns1:Designation>testVerschieben4</ns1:Designation>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Designation>verschieben</ns1:Designation>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>A</ns1:Country>
               <ns1:Designation>teil zum verschieben</ns1:Designation>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>A</ns1:Country>
               <ns1:Designation>testverschieben</ns1:Designation>
            </ns1:DatPosition>
            <ns1:DatPosition>
               <ns1:Country>D</ns1:Country>
               <ns1:Designation>gfh</ns1:Designation>
               <ns1:WorkLevel>-1</ns1:WorkLevel>
               <ns1:WorkType>-1</ns1:WorkType>
            </ns1:DatPosition>
         </manualPositions>
      </ns4:exportManualPositionsResponse>
   </S:Body>
</S:Envelope>
```
