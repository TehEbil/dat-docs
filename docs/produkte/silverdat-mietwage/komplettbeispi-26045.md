---
title: "Komplettbeispiel"
topic_id: "26045"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Integration der Oberfläche > Komplettbeispiel"
---

# Komplettbeispiel

Die nachfolgende HTML-Datei stellt ein vereinfachtes Beispiel zur Integration des
Produkts SilverDAT 3 Mietwagenspiegel in eine Fremdanwendung dar. Bei diesem Beispiel dienen die Positionierungen, Größenangaben
und Farben nur zur Verdeutlichung. Struktur und Design müssen für die jeweilige Lösung
entsprechend angepasst werden und können unterschiedlich gestaltet werden, solange
die Kommunikation mit dem beschriebenen Protokoll übereinstimmt.

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "https://www.w3.org/TR/html4/loose.dtd">
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
                        action : "generateToken",
                        customerNumber : "9999999",
                         user : "myLogin",
                        password : "myPwd",
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
                    rentalPricesExternal.setDatGroupHeader( "true" );
                    rentalPricesExternal.setWorkflow( "true" );
                    rentalPricesExternal.setProcesses( "true" );
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
