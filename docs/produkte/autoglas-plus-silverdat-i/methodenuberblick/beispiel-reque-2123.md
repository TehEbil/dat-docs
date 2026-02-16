---
title: "Beispiel-Request zu getContract"
topic_id: "2123"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Methodenüberblick > Methoden > Abrufen eines einzelnen Vorgangs mit getContract > Zwingend erforderliche Parameter > Beispiel-Request zu getContract"
---

# Beispiel-Request zu getContract

###### Beispiel-Request zu getContract ``` <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:glas="http://sphinx.dat.de/services/GlassRep" xmlns:dms="http://sphinx.dat.de/services/DMSGetContracts"> <soapenv:Header/> <soapenv:Body> <glas:getContract> <!--Optional:--> <!--type: string--> <contractNumber>D</contractNumber> </glas:getContract> </soapenv:Body> </soapenv:Envelope> ```
