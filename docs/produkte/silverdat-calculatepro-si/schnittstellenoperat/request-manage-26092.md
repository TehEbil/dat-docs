---
title: "Request manageAttachments"
topic_id: "26092"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Hochladen, Überschreiben und Löschen von Dokumenten > Request manageAttachments"
---

# Request manageAttachments

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:manageAttachments>
         <request>
            <contractId>2169932</contractId>
            <crud>UPLOAD</crud>
            <attachments>
               <Attachment>
                  <filename>picture1</filename>
                  <suffix>jpg</suffix>
<b64Data>iVBORw0KGgoAAAANSUhEUgAAAbAAAAE+CAYAAADs9EWCAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAFg0SURBVHhe7d17sC1Zfdj3+cv+I1alrKLKqpDIkWJXEadi2VUWVbZxOYE8LCqKRCQZ6wGWyjwsBpUDScTgRKAI4cQgJzxkC7BkDbYkEMx77gxz58E8gZlh5j7O+3Hv3DtvhmF4C5CQc9Kr91ln/3r1t7vXr9fq1d17rz8+tef26l6777nS+tJ7997....ABJRU5ErkJggg==</b64Data>
               </Attachment>
                <Attachment>
                  <filename>picture2</filename>
                  <suffix>png</suffix>
                  <b64Data>iVBORw0KGgoAAAANSUhEUgAAAdQAAAF4CAYAAADt+Qj5AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAIiwSURBVHhe7d1nlC3pXd/7eSXewBvghe27FmEtgtfF+BohTAYDFpcoYda6ApMEJpksCSNhQERxAQkbCSMEAgkQSaMZafLJOffJOZ+ZMzOKKEcQmLtv/av72f3bz/5WPfWveqp67+568V3n1BN2j/qY/rhq166+528fvW/SpL955P6l628fff...4AAAAASUVORK5CYII=</b64Data>
                </Attachment>
            </attachments>
         </request>
      </veh:manageAttachments>
   </soapenv:Body>
</soapenv:Envelope>
```
