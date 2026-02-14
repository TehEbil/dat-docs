---
title: "Finden eines Auftrags"
topic_id: "1473"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Finden eines Auftrags"
---

# Finden eines Auftrags

Die Funktion findContract identifiziert einen oder mehrere Aufträge anhand des übergebenen Aktenzeichennamens
und gibt dessen Auftrags ID‘s zurück. Zusätzlich kann das Ergebnis anhand der Partneridentifikation
(z.B. der Name einer Versicherung) weiter eingeschränkt werden.

Falls der Name des Aktenzeichens bekannt ist, kann diese Funktion verwendet werden
um zuerst die ID des gewünschten Aktenzeichens zu bestimmen. Mit dieser ID kann dann
mit der Funktion getContract das gesamte Aktenzeichen geholt werden.

Parameter partnerIdentification ist case sensitive, daher sollten Sie die Groß- / Kleinschreibung beachten.

 Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| referenceNumber | String |  | Aktenzeichen des Auftrags | X |
| partnerIdentification | String |  | Name des Partners (zb. Name der Versicherung) |  |

Beispiel

```
/* 1 */
MyClaimExternalService_Service mycExtService_service = new MyClaimExternalService_Service();
MyClaimExternalService myClaimExternalService = mycExtService_service.getMyClaimExternalServicePort();

/* 2 */
final String JAVAX_XML_REQUEST_HEADERS = "javax.xml.ws.http.request.headers";
BindingProvider bindingProviderMyClaimExternalService = (BindingProvider) myClaimExternalService;
Map<String, List<String>> reqHeadersMyClaimExternalService = (Map<String,List<String>>) bindingProviderMyClaimExternalService.getRequestContext().get( JAVAX_XML_REQUEST_HEADERS );
if (reqHeadersMyClaimExternalService == null) {
  reqHeadersMyClaimExternalService = new HashMap<String, List<String>>();
  bindingProviderMyClaimExternalService.getRequestContext().put(JAVAX_XML_REQUEST_HEADERS,reqHeadersMyClaimExternalService);
}
bindingProviderMyClaimExternalService.put("Cookie", cookieHeaders);

/* 3 update contract */
String referenceNumber;  /* you gotta know */
String partnerIdentification; /* you gotta know */
String rolePartner = CustomerRole.INSURANCE;  /* ... or another mnemonic from the enum */

/* 3.1 assign partner to role in contract */
List<Long> contractIds = findContract(referenceNumber, partnerIdentification);
Long contractId = contractIds.get(0);
boolean assignmentSuccessful = myClaimExternalService.getContract(contractId);
```

Rückgabe

Auftrags ID eines Aktenzeichens respektive Auftrags
