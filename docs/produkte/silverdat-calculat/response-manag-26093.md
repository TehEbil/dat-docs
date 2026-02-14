---
title: "Response manageAttachments"
topic_id: "26093"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Hochladen, Überschreiben und Löschen von Dokumenten > Response manageAttachments"
---

# Response manageAttachments

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns4:manageAttachmentsResponse xmlns:ns4="http://sphinx.dat.de/services/VehicleRepairService">
         <uploadStatusList>
            <uploadStatus>
               <Attachment xmlns:ns1="http://www.dat.de/vxs">
                  <ns1:AttachmentId>1203227</ns1:AttachmentId>
               </Attachment>
               <message>Upload succesful</message>
               <status>200</status>
            </uploadStatus>
            <uploadStatus>
               <Attachment xmlns:ns1="http://www.dat.de/vxs">
                  <ns1:AttachmentId>1203228</ns1:AttachmentId>
               </Attachment>
               <message>Upload succesful</message>
               <status>200</status>
            </uploadStatus>
         </uploadStatusList>
      </ns4:manageAttachmentsResponse>
   </S:Body>
</S:Envelope>
```
