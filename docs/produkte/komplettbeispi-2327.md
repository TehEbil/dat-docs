---
title: "Komplettbeispiel"
topic_id: "2327"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Integration der Oberfläche > Komplettbeispiel"
---

# Komplettbeispiel

Die nachfolgende HTML-Datei stellt ein vereinfachtes Beispiel zur Integration der
SilverDAT 3 valuateExpert/PlusPartner in eine Fremdanwendung dar. Bei diesem Beispiel dienen die Positionierungen, Größenangaben
und Farben nur zur Verdeutlichung. Struktur und Design müssen für die jeweilige Lösung
entsprechend angepasst werden und können unterschiedlich gestaltet werden, solange
die Kommunikation mit dem beschriebenen Protokoll übereinstimmt.

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
    <title>SilverDAT 3 valuateExpert Web-UI integration example</title>
    <style type='text/css'></style>
    <script type="text/javascript" src="https://www.datgroup.com/valuateNG/app/js/external.js"></script>
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
                    valuateNGExternal.setName( "Test name" );
                    valuateNGExternal.setProductVariant( "valuateNG.expert" );
                    valuateNGExternal.setLocale( "de_DE" );
                    valuateNGExternal.setIsDisengagedN("false");
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
                    valuateNGExternal.setMileageEstimated( "145000" );
                    valuateNGExternal.setMileageType( "Estimated" );
                    valuateNGExternal.setOnExecuteSuccess(
                    function () {
                        $.ajax( {
                            type: "POST",
                            url: "https://myhostname/valuateNGExternalClient/result",
                            dataType: "json",
                            data: {
                                "result": valuateNGExternal.getDossier()
                            }
                        } );
                    } );
                    valuateNGExternal.login();
                    valuateNGExternal.setOnLoginSuccess(valuateNGExternal.execute);
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
