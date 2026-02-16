---
title: "HTML-Grundgerüst"
topic_id: "26039"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Integration der Oberfläche > HTML-Grundgerüst"
---

# HTML-Grundgerüst

Die bereitzustellende HTML-Datei sollte in etwa wie folgt aussehen:

```
<html>
    <head>
        <title>SilverDAT 3 Mietwagenspiegel Web-UI integration example</title>
        <style type='text/css'></style>
    </head>
    <body></body>
</html>
```

In das HTML-Grundgerüst müssen die zwingend benötigten JavaScript-Dateien von DAT
inkludiert werden:

```
<html>
    <head>
        <title>SilverDAT 3 Mietwagenspiegel Web-UI integration example</title>
        <style type='text/css'></style>
        <script type="text/javascript" src="https://www.datgroup.com/rentalPrices/app/js/external.js"></script>
        <script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
    </head>
    <body></body>
</html>
```

Die Datei external.js stellt ein globales JavaScript-Objekt namens rentalPricesExternal zur Verfügung. Dieses Objekt wird nachfolgend für alle Interaktionen mit SilverDAT 3 Mietwagenspiegel verwendet.

Als nächstes wird der Event Handler des Window Objekts für den Login und die Anzeige
einer vorgegebenen Seite des Produkts SilverDAT 3 Mietwagenspiegel benötigt.

```
<html>
    <head>
        <title>SilverDAT 3 Mietwagenspiegel Web-UI integration example</title>
        <style type='text/css'></style>
        <script type="text/javascript" src="https://www.datgroup.com/rentalPrices/app/js/external.js"></script>
        <script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
        <script type="text/javascript">
            $(document).ready(function(){
                $.ajax( {
                    url: 'https://www.datgroup.com/AuthorizationManager/service--/endpoint/tokenService',
                    data: {
                        payload : JSON.stringify({
                            action: "generateToken",
                            customerNumber: "9999999",
                            user: "myLogin",
                            password: "myPwd",
                            interfacePartnerNumber : "9999999",
                            interfacePartnerSignature : "783466..."
                        })
                    },
                    type: 'POST',
                    error: function (error) { alert(error); },
                    success: initExternal
                });
            });
            function initExternal(token) {
                if ( typeof rentalPricesExternal != 'undefined' ) {
                    rentalPricesExternal.ready( function () {
                        rentalPricesExternal.setExternalUrl( "https://myhostname/ExternalRentalPrices/client.html" );
                        rentalPricesExternal.setIframeName( "rentalPrices.external.iframe" );
                        rentalPricesExternal.setToken(token);
                        rentalPricesExternal.setSessionAuthentication( "false" );
                        rentalPricesExternal.setLocale( "de_DE" );
                        rentalPricesExternal.setCountry( "DE" );
                        rentalPricesExternal.setStartPage( "rentalPrices.model" );
                        rentalPricesExternal.setPageList( "" );
                        rentalPricesExternal.setDatGroupHeader( "true" );
                        rentalPricesExternal.setWorkflow( "true" );
                        rentalPricesExternal.setProcesses( "true" );
                        rentalPricesExternal.setSave( "true" );
                        rentalPricesExternal.setMode( "" );
                        rentalPricesExternal.execute();
                    });
                }
                else {
                    alert( "external.js not found!" );
                }
            }
        </script>
</head>
```

Zur Kommunikation mit dem DAT-Server und dem entsprechenden Aufruf einer SilverDAT 3 Mietwagenspiegel Seite in einem Iframe werden weitere Angaben benötigt. Die Beschreibung der Parameter finden Sie unter
[Aufruf der SilverDAT 3 valuateExpert Oberfläche](../../silverdat-3-valuateexpert/integration-der-ober/aufruf-der-met-2318.md).

Die Integration des Iframes erfolgt im Body.

```
<html>
    <head>
        <title>SilverDAT 3 Mietwagenspiegel Web-UI integration example</title>
        <style type='text/css'></style>
        <script type="text/javascript" src="https://www.datgroup.com/rentalPrices/app/js/external.js"></script>
        <script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
        <script type="text/javascript">
            $(document).ready(function(){
                $.ajax( {
                    url: 'https://www.datgroup.com/AuthorizationManager/service--/endpoint/tokenService',
                    data: {
                        payload : JSON.stringify({
                            action: "generateToken",
                            customerNumber: "9999999",
                            user: "myLogin",
                            password: "myPwd",
                            interfacePartnerNumber : "9999999",
                            interfacePartnerSignature : "783466..."
                        })
                    },
                    type: 'POST',
                    error: function (error) { alert(error); },
                    success: initExternal
                });
            });
            function initExternal(token) {
                if ( typeof rentalPricesExternal != 'undefined' ) {
                    rentalPricesExternal.ready( function () {
                        rentalPricesExternal.setExternalUrl( "https://myhostname/ExternalRentalPrices/client.html" );
                        rentalPricesExternal.setIframeName( "rentalPrices.external.iframe" );
                        rentalPricesExternal.setToken(token);
                        rentalPricesExternal.setSessionAuthentication( "false" );
                        rentalPricesExternal.setLocale( "de_DE" );
                        rentalPricesExternal.setCountry( "DE" );
                        rentalPricesExternal.setStartPage( "rentalPrices.model" );
                        rentalPricesExternal.setPageList( "" );
                        rentalPricesExternal.setDatGroupHeader( "true" );
                        rentalPricesExternal.setWorkflow( "true" );
                        rentalPricesExternal.setProcesses( "true" );
                        rentalPricesExternal.setSave( "true" );
                        rentalPricesExternal.setMode( "" );
                        rentalPricesExternal.execute();
                    });
                }
                else {
                    alert( "external.js not found!" );
                }
            }
        </script>
</head>
<body style="margin: 0; border: 0; padding: 0; background-color: #FFD155;">
    <table cellpadding="0" cellspacing="0" style="width: 100%; height: 100%;">
        <tbody>
        <tr style="height: 50px;">
            <td></td>
            <td><p style="font-size: 20px;">Sample application including SilverDAT 3 Mietwagenspiegel</p></td>
            <td></td>
        </tr>
        <tr>
            <td></td>
            <td style="width: 1094px; height: 768px;">
                <iframe name="valuateNG.external.iframe" style="width: 100%; height: 100%;
                background-color: #FFFFFF; border: 0;"></iframe>
            </td>
            <td></td>
        </tr>
        <tr style="height: 50px;">
        </tr>
        </tbody>
    </table>
</body>
</html>
```

Mit der Methode rentalPricesExternal.execute führen Sie den Aufruf der SilverDAT 3 Mietwagenspiegel Oberfläche durch.
