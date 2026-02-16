---
title: "Ansprechpartner holen"
topic_id: "12329"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Stammdaten holen > Ansprechpartner holen"
---

# Ansprechpartner holen

Mit der Funktion getPossibleContactPersons holen Sie alle Ansprechpartner, die in den Stammdaten angelegt wurden. Die Ansprechpartner
benötigen Sie für die Parameter SellerId und BuyerId der Funktionen setPurchaseData, setAdmissionData und setSalesData. Im Response von getPossibleContactPersons erhalten Sie die zum Ansprechpartner zugehörige Id, die Sie für die Parameter SellerId und BuyerId der Funktionen setPurchaseData, setAdmissionData und setSalesData benötigen.

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns3:getPossibleContactPersonsResponse xmlns:ns3="http://www.dat.eu/myClaim/soap/v2/MyClaimExternalService">
         <PossibleContactPersons>
            <firstName>Max</firstName>
            <id>2781</id>
            <name>34, Mustermann</name>
            <salutation>titleMr</salutation>
            <surname>34</surname>
         </PossibleContactPersons>
      </ns3:getPossibleContactPersonsResponse>
   </S:Body>
</S:Envelope>
```

Hier finden Sie die Beschreibung der Funktion zum [Auflisten von Ansprechpartnern](../../silverdat3-myclaim/schnittstellenoperat/auflisten-von-9171.md)

Ein Beispiel finden Sie unter folgenden Link: getPossibleContactPersons

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:myc="http://www.dat.eu/myClaim/soap/MyClaimExternalService">
   <soapenv:Header/>
   <soapenv:Body>
      <myc:getPossibleContactPersons/>
   </soapenv:Body>
</soapenv:Envelope>
```
