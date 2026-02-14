---
title: "Aufbereitung der Authentifizierungsinformationen"
topic_id: "2322"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Integration der Oberfläche > Aufruf der Methoden von SilverDAT 3 valuateExpert Oberflächeintegration > Aufbereitung der Authentifizierungsinformationen"
---

# Aufbereitung der Authentifizierungsinformationen

Die Anmeldung an SilverDAT 3 valuateExpert/PlusPartner über die Oberflächen-Schnittstelle erfolgt entsprechend der Anmeldung bei den Soap-Funktionen
zweistufig mittels der JSON Web Token Authentifikation. Im ersten Schritt erstellen Sie das Token mittels der Funktion
JSON.stringify und im zweiten Schritt melden Sie sich mittels der Funktion valuateNGExternal.setToken an. Das DAT-AuthorizationToken hat eine Gültigkeit von 30 Minuten. Die Anmeldedaten
sind identisch mit denjenigen für SOAP.

Token erstellen

| Name | Datentyp | mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| action | string | generateToken | Feste Kennung | X |
| customerNumber | string | 1234567 | Gültige Kundennummer mit Lizenz zum Produkt | X |
| user | string | myuser | Gültiger Benutzername zur o.g. Kundennummer | X |
| password | string | password | Persönliches Kennwort des Benutzers | X |
| interfacePartnerNumber | string | 1234567 | Gültige Kundennummer des Schnittstellenpartners mit Lizenz zum Produkt | X |
| interfacePartnerSignature | string | AF4662380.... | Generierter SHA256 Hash für den Schnittstellenpartner.  (Kann NICHT selbst erzeugt werden, wird von DAT zur Verfügung gestellt) | X |

Ein einfaches Beispiel zum Erstellen des JSON Web Tokens sieht wie folgt aus:

```
            payload: JSON.stringify( {
                action: "generateToken",
                customerNumber: "9999999",
                user: "myLogin",
                password: "password"
                interfacePartnerNumber : "9999999",
                interfacePartnerSignature : "jA0EAwMCJ..."
                } )
```

Anmelden

| Name | Datentyp | mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| token | string | 670a8f439c... |  | X |

| Name | Funktion von valuateNGExternal | Datentyp | Bedeutung | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- | --- |
| token | setToken | string | DAT\_Authorization Token | Ein aus der Kundennummer, dem Nutzernamen und dem Passwort erstellter Token. Der Token kann nicht selbst erstellt werden und wird über einen Webservice generiert. | X |
| ProductVariant | setProductVariant | string | Produktvariante | valuateNG.expert, valuateNG.expertPlusPartner | X |

Produktvarianten

| Produkt | Produktvariante | Pflicht |
| --- | --- | --- |
| SilverDAT 3 valuateExpert | valuateNG.expert | X |
| SilverDAT 3 valuateExpertPlusPartner | valuateNG.expertPlusPartner | X |

Bei allen anderen Anwendungen gibt es keine Produktvariante.

Ein einfaches Beispiel zur Übergabe des Tokens sieht wie folgt aus:

```
            valuateNGExternal.setToken(token)
            valuateNGExternal.setProductVariant( "valuateNG.expert" );
```
