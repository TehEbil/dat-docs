---
title: "Aufbereitung der Eingabeparameter"
topic_id: "26041"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Integration der Oberfläche > Aufruf der Methoden der SilverDAT 3 Mietwagenspiegel Oberflächeintegration > Aufbereitung der Eingabeparameter"
---

# Aufbereitung der Eingabeparameter

Alle benötigten Vorgaben für den Aufruf der Oberflächen-Schnittstelle des Produkts
SilverDAT 3 Mietwagenspiegel setzen Sie mit den rentalPricesExternal Objektfunktionen. Bitte beachten Sie, dass die nachfolgend beschriebenen Parameter
aufgrund der jeweiligen Berechtigungen und Systemeinstellungen eingeschränkt oder
auch nicht verfügbar sein können.

Der Client benötigt für die Kommunikation mit der aufrufenden Anwendung den Endpunkt
Ihrer Server-Anwendung. Bitte geben Sie den entsprechenden Endpunkt mit der Methode
setExternalUrl an. Der verwendete Inlineframe iframe benötigt einen Namen, damit man diesen in JavaScript referenzieren kann, bitte setzen Sie den Namen des iframe mit der Methode setIframeName. Um mit SilverDAT 3 Mietwagenspiegel arbeiten zu können, muss man sich zuerst anmelden. Sie können sich mittels der JSON
Web Token Authentifikation anmelden. Die Anmeldung mittels JSON Web Token erfolgt
entsprechend der Anmeldung bei den Soap-Funktionen zweistufig. Im ersten Schritt erstellen
Sie das Token mittels der Funktion JSON.stringify und im zweiten Schritt melden Sie sich mittels der Funktion setToken an. Das DAT-AuthorizationToken hat eine Gültigkeit von 30 Minuten. Die Beschreibung
hierzu finden Sie unter [Aufbereitung der Authentifizierungsinformationen](../../silverdat-3-valuateexpert/integration-der-ober/aufbereitung-d-2322.md). Ein einfaches Beispiel zur Übergabe des Tokens sieht wie folgt aus:

```
            valuateNGExternal.setToken(token)
```

Für den Aufruf muss man den gewünschten Zielmarkt einstellen, diesen setzen Sie mit
der Methode setCountry, zum Beispiel "DE". Ebenfalls muss noch die Oberflächensprache - das Sprachkürzel (Language) mit der Methode setLocale eingestellt werden. Diese Vorgabe verhält sich entsprechend der Sprachumschaltung
in der Oberfläche. Mit der Methode setStartPage bestimmen Sie das Aufrufziel. Diese Angabe ist der wichtigste Parameter zur Steuerung
der Oberflächen-Schnittstelle, je nach Vorgabe sind unterschiedliche Aktionen und
Seitenaufrufe möglich. Bitte beachten Sie hierbei die Abhängigkeiten, die zugehörige
Beschreibung finden Sie unter [Aufrufziele](aufrufziele-26043.md). Damit sind die Mindestanforderungen für einen einfachen Aufruf erfüllt.

Falls Sie beim Aufruf der Oberflächen-Schnittstelle, die für den Benutzer zugänglichen
Seiten einschränken möchten, dann können Sie dies mit der Methode setPageList vorgeben. Die gewünschten Seiten tragen Sie als kommaseparierte Liste ein.

Ein einfaches Beispiel für setPageList sieht wie folgt aus:

```
            rentalPricesExternal.setLocale( "de_DE" );
            rentalPricesExternal.setCountry( "DE" );
            rentalPricesExternal.setStartPage( "rentalPrices.model" );
            rentalPricesExternal.setPageList( "rentalPrices.model,rentalPrices.rentalCarClassAndLocationSearch" );
```

Mit der Methode execute rufen Sie die SilverDAT 3 Mietwagenspiegel Oberfläche mit allen angegebenen Parametern auf.

Ein einfaches Beispiel sieht wie folgt aus:

```
    rentalPricesExternal.execute();
```
