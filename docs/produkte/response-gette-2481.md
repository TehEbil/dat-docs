---
title: "Response getTemplates"
topic_id: "2481"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abruf aller existierenden Druckvorlagen > Response getTemplates"
---

# Response getTemplates

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns2:getTemplatesResponse xmlns:ns2="http://sphinx.dat.de/services/VehicleRepairService" xmlns:ns3="http://www.dat.de/vxs">
         <ExportProduct>
            <displayName>Kalkulationsergebnis</displayName>
            <fileName>calculation/calculationResult.docx</fileName>
            <identifier>409</identifier>
            <origin>DAT-Standard</origin>
            <printProductName>CALC_ESTIMATE</printProductName>
         </ExportProduct>
         <ExportProduct>
            <displayName>Rechnung</displayName>
            <fileName>calculation/calculationResult.docx</fileName>
            <identifier>410</identifier>
            <origin>DAT-Standard</origin>
            <printProductName>CALC_INVOICE</printProductName>
         </ExportProduct>
         <ExportProduct>
            <displayName>Kalkulation SPO</displayName>
            <fileName>calculation/SPOReport.docx</fileName>
            <identifier>961</identifier>
            <origin>DAT-Standard</origin>
            <printProductName>CALC_PARTS_SPO</printProductName>
         </ExportProduct>
         <ExportProduct>
            <displayName>Besichtigungsbericht</displayName>
            <fileName>calculation/inspectionReport.docx</fileName>
            <identifier>962</identifier>
            <origin>DAT-Standard</origin>
            <printProductName>INSPECTION_REPORT</printProductName>
         </ExportProduct>
      </ns2:getTemplatesResponse>
   </S:Body>
</S:Envelope>
```
