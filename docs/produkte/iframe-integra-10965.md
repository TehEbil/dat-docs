---
title: "Iframe Integration von myclaim in Anwendungen von Drittanbietern"
topic_id: "10965"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Iframe Integration von myclaim in Anwendungen von Drittanbietern"
---

# Iframe Integration von myclaim in Anwendungen von Drittanbietern

Einfache IFrame Integration:

```
<html> 
 <head> 
  <title>MyClaim iframe</title> 
 </head> 
 <body> 
  <iframe width="1600" height="800" src="https://host/myClaim/json/security/Login?fabrikat=FABRIKAT_HERE&token=TOKEN_HERE"></iframe> 
 </body> 
</html>
```

Erweiterte IFrame Integration mit Ereignis-Listener:

Mit addEventListener können Sie jede Art von Nachricht „abhören“ und nach dem Typ "event" suchen.

Die Option zum Übergeben an das Eltern-Element ist standardmäßig für jedes Ereignis
deaktiviert.

Wenn dieser Wert auf "true" gesetzt ist und myClaim als iframe eingebettet ist, wird eine Nachricht an den übergeordneten Frame gesendet.
Siehe $.postEventMessageToParent( eventName, data ) in utils.js

```
<html> 
 <head> 
  <title>MyClaim iframe</title> 
 </head> 
  <body> 
   <iframe width="1600" height="800" src="https://host/myClaim/json/security/Login?token=TOKEN_HERE&customerNumber=CUSTOMER_NUMBER_HERE&login=LOGIN_HERE"></iframe> 
   <script type="text/javascript"> 
    window.addEventListener( "message", function( msgEvent ) { 
    var msgData = msgEvent.data; 
    if ( msgData && msgData.type === "event" ) { 
    // msgData.event represents the type of event 
    console.log( msgData.event, msgData.data ); 
} 
}, false); 
 </script> 
 </body> 
</html>
```

Ereignissestruktur:

Die an das Eltern-Element gesendete Nachricht hat die folgende Struktur

```
{ 
 type: "event", 
 event: eventName, 
 data: data     
}
```

Vorhandene Ereignisse:

Auftrag gespeichert

```
{ 
 type: "event", 
 event: "inbox_templateSaved", 
 data: claim object 
}
```

Neue Bewertung

```
{ 
 type: "event", 
 event: "inbox_valuated", 
 data: claim object 
}
```

Partner geändert

```
{ 
 type: "event", 
 event: "inbox_partnerChange", 
 data: { 
 "claimId": 1162532, 
 "partnerFrontEndByRole": { 
 "REPAIRER": { 
 "id": 21, 
 "claimId": 1162532, 
 "name": "DAT Entwicklung", 
 "role": "REPAIRER", 
 "originAddress": null, 
 "assignable": false, 
 "unassignable": false, 
 "settlementId": null, 
 "settlement": null, 
 "compliant": null 
} 
}, 
"dataSources": null 
} 
}
```

Kalkulation aktualisieren

```
{ 
type: "event", 
event: "refresh_calculation", 
data: { 
"discounts": [ ], 
"wages": [ ], 
"spareParts": null, 
"workPositions": null, 
"auxiliaryCosts": null, 
"paintingPositions": null, 
"addresses": [], 
"media": null, 
"calculationSettings": {}, 
"sourceArchive": null, 
"printOut": null, 
"protocolData_id": 1284184, 
"vehicle": { }, 
"paymentData": { }, 
"insuranceData": { }, 
"workCostsList": null, 
"paintingCosts": null, 
"repairPositions": [ ], 
"aggregates": null, 
"rearrangedCalculationPositions": null, 
"attachmentsForDossier": null, 
"auxiliaryCosts_total_total": null, 
"surchargeDiscount_total": 200.04, 
"datNetId": "97-ASPIS-DE-20180119144515379", 
"modifications_created_login": "vanhquen", 
"modifications_created_time": 1516807242339, 
"modifications_edited_login": "vanhquen", 
"modifications_edited_time": 1516807242339, 
"painting_total_material": 34.67, 
"painting_total_total": 351.47, 
"painting_total_work": 316.8, 
"published": false, 
"referenceNumber": "97-ASPIS-DE-", 
"referenceVersion": null, 
"spareParts_total_parts": 126.3, 
"spareParts_total_smallParts": null, 
"spareParts_total_smallPartsLim": null, 
"spareParts_total_discount": null, 
"spareParts_surchageDeduction": null, 
"spareParts_total_total": 126.3, 
"totalPrice": 941.81, 
"totalPrice_paymentInsurer": 1120.75, 
"totalPrice_paymentOwner": 0.0, 
"totalPrice_vat": 178.94, 
"totalPrice_vatIncluded": 1120.75, 
"uploaded": 1516807242339, 
"uploader_id": 126772, 
"work_total_body": 264.0, 
"work_total_electric": null, 
"work_total_mechanic": null, 
"work_total_dents": null, 
"work_total_before_discount": null, 
"work_total_total": 264.0, 
"claim_id": 1161704, 
"printOut_id": null, 
"sourceArchive_id": null, 
"totalPrice_beforeDiscount": 941.81, 
"totalPrice_vat_beforeDiscount": 178.94, 
"totalPrice_brut_beforeDiscount": 1120.75, 
"totalDiscountPrice": null, 
"totalDiscountPrice_vat": null, 
"totalDiscountPrice_brutto": null, 
"totalPriceDeductible": null, 
"totalPriceDeductible_vat": null, 
"totalPriceDeductible_brutto": null, 
"customer_id": 21, 
"dentMethod": null, 
"isOptimized": true, 
"calculationType": "VRO_API", 
"main_calculation_id": null, 
"mainCalculation": null, 
"externalPricesOrigin": null, 
"customTags": null, 
"italiaSummaries": null, 
"legends": [], 
"isBiWOptimized": null, 
"totalWorkingTime": 12.0, 
"spareParts_procurementCosts": null, 
"spareParts_procurementCostsLim": null, 
"spareParts_disposalCosts": null, 
"spareParts_disposalCostsLim": null, 
"additionalCostsFlatAmount": null, 
"spareparts_total_wear": null, 
"spareparts_total_parts_wear": null, 
"spareparts_total_total_wear": null, 
"totalprice_wear": null, 
"totalprice_wear_round": null, 
"deductionsTotalGross": null, 
"deductionsTotalNet": null, 
"id": 149498 
} 
}
```

Status geändert

```
{ 
 type: "event", 
 event: "inbox_statusChanged", 
 data: { 
 "claim": 1161704, 
 "status": { 
 "active": true, 
 "description": null, 
 "icon": "icon-status-uploaded", 
 "name": "Kalkuliert", 
 "statusType": "uploaded", 
 "networkType": "IFERT", 
 "networkTypeName": "IFERT", 
 "owner_id": null, 
 "statusOrder": 0, 
 "parents": null, 
 "children": null, 
 "recipients": ["REPAIRER", "INSURANCE", "MANUFACTURER"], 
 "exclusions": [], 
 "handlers": null, 
 "identification": null, 
 "id": 1000421 
} 
} 
}
```
