---
title: "HTML-Grundgerüst"
topic_id: "2316"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Integration der Oberfläche > HTML-Grundgerüst"
---

# HTML-Grundgerüst

Die bereitzustellende HTML-Datei sollte in etwa wie folgt aussehen:

```
<html>
    <head>
        <title>SilverDAT 3 valuateExpert Web-UI integration example</title>
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
        <title>SilverDAT 3 valuateExpert Web-UI integration example</title>
        <style type='text/css'></style>
        <script type="text/javascript"
        src="https://www.datgroup.com/valuateNG/app/js/external.js"></script>
        <script src="https://code.jquery.com/jquery-3.1.1.min.js"></script>
    </head>
    <body></body>
</html>
```

Die Datei external.js stellt ein globales JavaScript-Objekt namens valuateNGExternal zur Verfügung. Dieses Objekt wird nachfolgend für alle Interaktionen mit SilverDAT 3 valuateExpert/PlusPartner benutzt.

Als nächstes wird der Event Handler des Window Objekts für den Login und die Anzeige
einer vorgegebenen Seite der SilverDAT 3 valuateExpert/PlusPartner benötigt.

```
<html>
<head>
    <title>SilverDAT 3 valuateExpert Web-UI integration example</title>
    <style type='text/css'></style>
    <script type="text/javascript"
    src="https://www.datgroup.com/valuateNG/app/js/external.js"></script>
    <script src="https://code.jquery.com/jquery-3.1.1.min.js"></script>
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
                    } );
        });
        function initExternal(token) {
            if ( typeof valuateNGExternal != 'undefined' ) {
                valuateNGExternal.ready( function () {
                    valuateNGExternal.setExternalUrl( "http://myhostname/ExternalvaluateExpert/client.html" );
                    valuateNGExternal.setIframeName( "valuateNG.external.iframe" );
                    valuateNGExternal.setSessionAuthentication( "false" );
                    valuateNGExternal.setToken(token)
                    valuateNGExternal.setProductVariant( "valuateNG.expert" );
                    valuateNGExternal.setLocale( "de_DE" );
                    valuateNGExternal.setCountry( "DE" );
                    valuateNGExternal.setDossierId( "" );
                    valuateNGExternal.setDossier( "" );
                    valuateNGExternal.setStartPage( "valuation.create" );
                    valuateNGExternal.setPageList( "" );
                    valuateNGExternal.setDatGroupHeader( "true" );
                    valuateNGExternal.setWorkflow( "true" );
                    valuateNGExternal.setProcesses( "false" );
                    valuateNGExternal.setSave( "true" );
                    valuateNGExternal.setMode( "" );
                    valuateNGExternal.setDatECode( "010600370430004" );
                    valuateNGExternal.setContainer( "DE001" );
                    valuateNGExternal.setConstructionTime( "4495" );
                    valuateNGExternal.setOnExecuteSuccess(
                    function () {
                        $.ajax( {
                            type: "POST",
                            url:
                                "https://myhostname/valuateNGExternalClient/result",
                            dataType: "json",
                            data: {
                                "result": valuateNGExternal.getDossier()
                                }
                            } );
                    } );
                    valuateNGExternal.setOnLoginSuccess(valuateNGExternal.execute);
                    valuateNGExternal.login();
                } );
            }
            else {
                alert( "https://www.datgroup.com/valuateNG/app/js/external.js not found!" );
            }
        }
    </script>
</head>
```

Zur Kommunikation mit dem DAT-Server und dem entsprechenden Aufruf einer SilverDAT 3 valuateExpert/PlusPartner Seite in einem Iframe werden weitere Angaben benötigt. Die Beschreibung der Parameter finden Sie unter
[Aufruf der SilverDAT 3 valuateExpert Oberfläche](#showid/2318 "Aufruf der Methoden von SilverDAT 3 valuateExpert Oberflächeintegration").

Die Integration des Iframes erfolgt im Body.

```
<html>
<head>
    <title>SilverDAT 3 valuateExpert Web-UI integration example</title>
    <style type='text/css'></style>
    <script type="text/javascript"
    src="https://www.datgroup.com/valuateNG/app/js/external.js"></script>
    <script src="https://code.jquery.com/jquery-3.1.1.min.js"></script>
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
                    } );
        });
        function initExternal(token) {
            if ( typeof valuateNGExternal != 'undefined' ) {
                valuateNGExternal.ready( function () {
                    valuateNGExternal.setExternalUrl( "http://myhostname/ExternalvaluateExpert/client.html" );
                    valuateNGExternal.setIframeName( "valuateNG.external.iframe" );
                    valuateNGExternal.setSessionAuthentication( "false" );
                    valuateNGExternal.setToken(token)
                    valuateNGExternal.setProductVariant( "valuateNG.expert" );
                    valuateNGExternal.setLocale( "de_DE" );
                    valuateNGExternal.setCountry( "DE" );
                    valuateNGExternal.setDossierId( "" );
                    valuateNGExternal.setDossier( "" );
                    valuateNGExternal.setStartPage( "valuation.create" );
                    valuateNGExternal.setPageList( "" );
                    valuateNGExternal.setDatGroupHeader( "true" );
                    valuateNGExternal.setWorkflow( "true" );
                    valuateNGExternal.setProcesses( "false" );
                    valuateNGExternal.setSave( "true" );
                    valuateNGExternal.setMode( "" );
                    valuateNGExternal.setDatECode( "010600370430004" );
                    valuateNGExternal.setContainer( "DE001" );
                    valuateNGExternal.setConstructionTime( "4495" );
                    valuateNGExternal.setOnExecuteSuccess(
                    function () {
                        $.ajax( {
                            type: "POST",
                            url:
                                "https://myhostname/valuateNGExternalClient/result",
                            dataType: "json",
                            data: {
                                "result": valuateNGExternal.getDossier()
                                }
                            } );
                    } );
                    valuateNGExternal.setOnLoginSuccess(valuateNGExternal.execute);
                    valuateNGExternal.login();
                } );
            }
            else {
                alert( "https://www.datgroup.com/valuateNG/app/js/external.js not found!" );
            }
        }
    </script>
</head>
<body style="margin: 0; border: 0; padding: 0; background-color: #FFD155;">
    <table cellpadding="0" cellspacing="0" style="width: 100%; height: 100%;">
        <tbody>
        <tr style="height: 50px;">
            <td></td>
            <td><p style="font-size: 20px;">Sample application including SilverDAT 3 valuateExpert</p></td>
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

Mit der Methode valuateNGExternal.execute führen Sie den Aufruf der SilverDAT 3 valuateExpert/PlusPartner Oberfläche durch.
