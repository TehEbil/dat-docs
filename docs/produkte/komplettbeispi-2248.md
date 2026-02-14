---
title: "Komplettbeispiel"
topic_id: "2248"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Integration der Oberfläche > Komplettbeispiel"
---

# Komplettbeispiel

Die nachfolgende HTML-Datei stellt ein vereinfachtes Beispiel zur Integration der
SilverDAT 3 valuateFinance in eine Fremdanwendung dar. Bei diesem Beispiel dienen die Buttons, Positionierungen,
Größenangaben und Farben nur zur Verdeutlichung. Struktur und Design müssen für die
jeweilige Lösung entsprechend angepasst werden und können unterschiedlich gestaltet
werden, solange die Kommunikation mit dem beschriebenen Protokoll übereinstimmt.

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
    <title>Web-UI Integration Example</title>
    <style type='text/css'>
        html, body {
            height: 100%;
            margin: 0;
            border: 0;
            padding: 0;
        }

        body {
            background-color: #FFD155;
        }

        textarea {
            background-color: #FFD155;
        }

        #divSilverDAT {
            width: 100%;
            height: 95%;
            border-width: 5px;
            border-style: solid;
        }

        #iframeSilverDAT {
            width: 100%;
            height: 100%;
            border: 0;
            background-color: #FFFFFF;
        }
    </style>
    <script src="https://code.jquery.com/jquery-3.1.1.min.js"></script>
    <script type="text/javascript" src="https://www.datgroup.com/FinanceLine/financeline/js/externalSphinxFL.js"></script>
    <script type="text/javascript">
        $.ajax( {
                url: 'https://www.datgroup.com/AuthorizationManager/service--/endpoint/tokenService',
                data: {
                    payload: JSON.stringify( {
                    action: "generateToken",
                    customerNumber: "9999999",
                    user: "myUser",
                    password: "myPassword",
                    interfacePartnerNumber: "9999999",
                    interfacePartnerSignature: "jA0EAwMCJ..."
                    } )
                },
                type: 'POST',
                error: function ( error ) {
                    alert( error );
            },
            success: setUpSphinx
            } );
        function setUpSphinx (token) {
            sphinx.setProductUrl( 'https://www.datgroup.com/FinanceLine/' ).setIframeName( 'iframeSilverDAT' );
            sphinx.hostUrl = "https://myhostname" + "/FinanceLinePostClient/client.html";
            sphinx.credentials = {
                token : token
            };
            sphinx.params = {
                datCountryIndicator : "DE",
                locale : "de_DE",
                name: "Test-Name",
                action : "createDossier",
                dossierid : "",
                type : "evaluation",
                vxs : "",
                page : "model selection",
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
<body>
<table cellpadding="0" cellspacing="0" style="width: 100%; height: 100%;">
    <tbody>
    <tr style="height: 5px;">
        <td width="15%"></td>
        <td width="80%"></td>
        <td width="5%"></td>
    </tr>
    <tr style="height: 25px">
        <td></td>
        <td>
            <input type="button" onclick="sphinx.sendDossierRequest();" value="SilverDAT valuateFinance starten"/>
        </td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td style="height: 90%">
            <div id="divSilverDAT">
                <iframe name="iframeSilverDAT" id="iframeSilverDAT"></iframe>
            </div>
        </td>
        <td></td>
    </tr>
    <tr style="height: 2%">
    </tr>
    </tbody>
</table>
<table cellpadding="0" cellspacing="0" style="width: 100%; height: 50%;">
    <tbody>
    <tr style="height: 0;">
        <td width="15%"></td>
        <td width="80%"></td>
        <td width="5%"></td>
    </tr>
    <tr>
        <td></td>
        <td>
            VXS-Ergebnis:&nbsp;&nbsp;&nbsp;&nbsp;<input type="button" onclick="sendVXS()" value="VXS-Ergebnis senden"/>
            <textarea readonly id="vxsResult" rows="20" cols="50" style="width: 100%; height: 100%;"></textarea>
        </td>
        <td></td>
    </tr>
    <tr style="height: 45px;">
    </tr>
    </tbody>
</table>
</body>
</html>
```
