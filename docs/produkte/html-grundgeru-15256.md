---
title: "HTML-Grundgerüst"
topic_id: "15256"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Integration der Oberfläche > HTML-Grundgerüst"
---

# HTML-Grundgerüst

Die bereitzustellende HTML-Datei sollte in etwa wie folgt aussehen:

```
<html>
    <head>
        <title>Web-UI Integration Example</title>
        <style type='text/css'></style>
    </head>
    <body></body>
</html>
```

In das HTML-Grundgerüst muss zwingend die benötigte JavaScript-Datei von DAT inkludiert
werden:

```
<html>
    <head>
        <title>Web-UI Integration Example</title>
        <style type='text/css'></style>
        <script type="text/javascript" 
        src="https://www.datgroup.com/FinanceLine/financeline/js/externalSphinxFL.js"></script>
    </head>
    <body></body>
</html>
```

Die Datei externalSphinxFL.js stellt dabei ein globales JavaScript-Objekt namens sphinx zur Verfügung, das für alle Interaktionen mit SilverDAT 3 valuateFinance benutzt wird.

Mit Hilfe der Aktion generateToken erstellen Sie den JSON Web Token für den Login.

```
<html>
    <head>
        <title>Web-UI Integration Example</title>
        <style type='text/css'></style>
        <script type="text/javascript" 
        src="https://www.datgroup.com/FinanceLine/financeline/js/externalSphinxFL.js"></script>
        <script type="text/javascript">
            $.ajax( {
            url: 'https://www.datgroup.com/AuthorizationManager/service--/endpoint/tokenService',
            data: {
                payload: JSON.stringify( {
                    action: "generateToken",
                    customerNumber: "9999999",
                    user: "myLogin",
                    password: "password",
                    interfacePartnerNumber : "9999999",
                    interfacePartnerSignature : "jA0EAwMCJ..."
                    } )
            },
            type: 'POST',
            error: function ( error ) {
                alert( error );
            },
            success: setUpSphinx
            } );
        }
        </script>
    </head>
    <body></body>
</html>
```

Als nächstes wird der Event Handler des Window Objekts für den Login und die Anzeige
einer vorgegebenen Seite der SilverDAT 3 valuateFinance benötigt.

```
<html>
    <head>
        <title>Web-UI Integration Example</title>
        <style type='text/css'></style>
        <script type="text/javascript" 
        src="https://www.datgroup.com/FinanceLine/financeline/js/externalSphinxFL.js"></script>
        <script type="text/javascript">
            $.ajax( {
            url: 'https://www.datgroup.com/AuthorizationManager/service--/endpoint/tokenService',
            data: {
                payload: JSON.stringify( {
                    action: "generateToken",
                    customerNumber: "9999999",
                    user: "myLogin",
                    password: "password",
                    interfacePartnerNumber : "9999999",
                    interfacePartnerSignature : "jA0EAwMCJ..."
                    } )
            },
            type: 'POST',
            error: function ( error ) {
                alert( error );
            },
            success: setUpSphinx
            } );
        };

        function setUpSphinx (token) {
            sphinx.setProductUrl( 'https://www.datgroup.com/FinanceLine/' ).
            sphinx.setIframeName( 'iFrameSilverDAT' );
            sphinx.hostUrl = "https://myhostname/FinanceLineClient/client.html";
            sphinx.credentials = {
                token: token
            };
            sphinx.params = {
                datCountryIndicator : "DE",
                locale : "de_DE",
                action : "createDossier",
                dossierid : "",
                type : "evaluation",
                vxs : "",
                page : "model selection",
                pageList : "",
                vehicleIdentNumber : "",
                vehicleIdentNumberRequest : "",
                initialRegistration : "",
                mileageEstimated : "",
                kbaNumber : "",
                nationalCodeAustria : "",
                datECode : "",
                container : "",
                constructionTime : "",
                workflow : "true",
                save : "true"
            };

            sphinx.onLoginFailure = function ( response ) {
                alert( 'DAT login failed!\nReason: ' + response.message );
            };
            sphinx.onFinished = function () {
                sphinx.exportDossier();
            };
            sphinx.afterExportDossier = function () {
                $( '#vxsResult' ).val( sphinx.response.xml );
                sphinx.logout();
            };
        };
        </script>
    </head>
    <body></body>
</html>
```

Zur Kommunikation mit dem DAT-Server und dem entsprechenden Aufruf einer SilverDAT 3 valuateFinance Seite in einem IFrame werden weitere Angaben benötigt. Die Beschreibung der Parameter finden Sie unter
[Aufruf der SilverDAT 3 valuateFinance Oberfläche](#showid/2240 "Aufruf der Oberfläche").

Der Aufruf von SilverDAT 3 valuateFinance erfolgt im Body.

```
<html>
    <head>
        <title>Web-UI Integration Example</title>
        <style type='text/css'></style>
        <script type="text/javascript" 
        src="https://www.datgroup.com/FinanceLine/financeline/js/externalSphinxFL.js"></script>
        <script type="text/javascript">
            $.ajax( {
            url: 'https://www.datgroup.com/AuthorizationManager/service--/endpoint/tokenService',
            data: {
                payload: JSON.stringify( {
                    action: "generateToken",
                    customerNumber: "9999999",
                    user: "myLogin",
                    password: "password",
                    interfacePartnerNumber : "9999999",
                    interfacePartnerSignature : "jA0EAwMCJ..."
                    } )
            },
            type: 'POST',
            error: function ( error ) {
                alert( error );
            },
            success: setUpSphinx
        } );

        function setUpSphinx (token) {
            sphinx.setProductUrl( 'https://www.datgroup.com/FinanceLine/' );
            sphinx.setIframeName( 'iFrameSilverDAT' );
            sphinx.hostUrl = "https://myhostname/FinanceLineClient/client.html";
            sphinx.credentials = {
                token: token
            };
            sphinx.params = {
                datCountryIndicator : "DE",
                locale : "de_DE",
                action : "createDossier",
                dossierid : "",
                type : "evaluation",
                vxs : "",
                page : "model selection",
                pageList : "",
                vehicleIdentNumber : "",
                vehicleIdentNumberRequest : "",
                initialRegistration : "",
                mileageEstimated : "",
                kbaNumber : "",
                nationalCodeAustria : "",
                datECode : "",
                container : "",
                constructionTime : "",
                workflow : "true",
                save : "true"
            };

            sphinx.onLoginFailure = function ( response ) {
                alert( 'DAT login failed!\nReason: ' + response.message );
            };
            sphinx.onFinished = function () {
                sphinx.exportDossier();
            };
            sphinx.afterExportDossier = function () {
                $( '#vxsResult' ).val( sphinx.response.xml );
                sphinx.logout();
            };
        };
    </script>
    <script type="text/javascript">
                };
            })();
        </script>
    </head>
    <body>
        <input type="button" onclick="sphinx.sendDossierRequest();" value="SilverDAT valuateFinance starten"/>
    </body>
</html>
```

Mit der Funktion sphinx.sendDossierRequest führen Sie den Aufruf der SilverDAT 3 valuateFinance Oberfläche durch.
