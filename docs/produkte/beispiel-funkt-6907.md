---
title: "Beispiel: Funktionsaufruf createCustomer"
topic_id: "6907"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Customer Service > Customer Service Schnittstellenoperationen > Neuen Kunden anlegen oder deaktivierten Kunden reaktivieren: createCustomer > Beispiel: Funktionsaufruf createCustomer"
---

# Beispiel: Funktionsaufruf createCustomer

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/" xmlns:cs="http://sphinx.dat.de/cs">
  <S:Body>
    <cs:createCustomer>
      <customer>
        <customerName1>Max</customerName1>
        <customerName2>Mustermann GmbH</customerName2>
        <customerName3></customerName3>
        <customerStreet>Gartenstraße</customerStreet>
        <customerStreetNumber>3b</customerStreetNumber>
        <customerZip>77007</customerZip>
        <customerCity>Stuttgart</customerCity>
        <customerCountry>DE</customerCountry>
        <customerTel>+49 (0)711 123 - 456</customerTel>
        <customerEmail>max.mustermann@mustermann-gmbh-test.de</customerEmail>
        <externalCustomerID>muster-963-25874</externalCustomerID>
      </customer>
      <filterName>Den Filternamen erhalten Sie über vertrieb@dat.de</filterName>
      <userEmail>max.mustermann@mustermann-gmbh-test.de</userEmail>
    </cs:createCustomer>
  </S:Body>
</S:Envelope>
```
