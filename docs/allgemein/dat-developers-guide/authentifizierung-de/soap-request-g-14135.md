---
title: "SOAP-Request generateToken (Beispiel)"
topic_id: "14135"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Authentifizierung der SilverDAT Webservices > JSON Web Token Authentication (DAT-AuthorizationToken) > SOAP-Request generateToken > SOAP-Request generateToken (Beispiel)"
---

# SOAP-Request generateToken (Beispiel)

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
                  xmlns:aut="http://sphinx.dat.de/services/Authentication">
   <soapenv:Header/>
   <soapenv:Body>
      <aut:generateToken>
         <request>
            <customerNumber>1234567</customerNumber>
            <customerLogin>loginName</customerLogin>
            <customerPassword>password</customerPassword>
            <interfacePartnerNumber>7654321</interfacePartnerNumber>
            <interfacePartnerSignature>GHHSLO...</interfacePartnerSignature>
            <!--Optional:-->
            <!--<productVariant>valuateNG.expert</productVariant>-->
         </request>
      </aut:generateToken>
   </soapenv:Body>
</soapenv:Envelope>
```
