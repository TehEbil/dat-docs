---
title: "Beispiel: Antwort createCustomerResponse"
topic_id: "6908"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Customer Service > Customer Service Schnittstellenoperationen > Neuen Kunden anlegen oder deaktivierten Kunden reaktivieren: createCustomer > Beispiel: Antwort createCustomerResponse"
---

# Beispiel: Antwort createCustomerResponse

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xs="http://sphinx.dat.de/cs">
  <S:Body>
    <ns2:createCustomerResponse xmlns:ns2="http://sphinx.dat.de/cs">
      <loginData>
        <customerNumber xs:type="xs:string">2222222</customerNumber>
        <externalCustomerID xs:type="xs:string">muster-963-25874</externalCustomerID>
        <userLogin xs:type="xs:string">UserLogin</userLogin>
        <userPassword xs:type="xs:string">UserPassword</userPassword>
      </loginData>
    </ns2:createCustomerResponse>
  </S:Body>
</S:Envelope>
```
