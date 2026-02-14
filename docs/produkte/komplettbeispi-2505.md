---
title: "Komplettbeispiel"
topic_id: "2505"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Integration der Oberfläche > Komplettbeispiel"
---

# Komplettbeispiel

```
<!DOCTYPE html> 
<head>
   <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
   <meta charset="utf-8">
   <meta name="description" content="" />
   <meta name="viewport" content="width=device-width" />
   <title>DAT Workshop</title>
   <link rel="shortcut icon" type="image/x-icon" href="favicon.ico">
   <style>
      body { border: none; margin: none; }
      .modelIFrame{
      width: 100%;
      height: 720px;
      border: none;
      }
      .header{
      width: 100%;
      height: 5%;
      border: 1px solid #66CC66;
      text-align:center;
      margin-bottom: 10px;
      }
      .footer{
      width: 100%;
      height: 5%;
      border: 1px solid #66CC66;
      text-align:center;
      margin-top: 10px;
      }
   </style>
   <script language="JavaScript" src="https://www.dat.de/sphinx/js/lazyload.js" type="text/javascript"></script>
   <script language="JavaScript" src="https://www.dat.de/sphinx/js/externalSphinx.js" type="text/javascript"></script>
   <script language="JavaScript" src="https://code.jquery.com/jquery-2.2.4.min.js" type="application/javascript"></script>
   <script type="text/javascript" language="JavaScript">
       function load() {
             var values = new Object();
             //Es kann entweder eine gültige Vorgangsnummer (contractID) wie beispielsweise via Anlage eines neuen Vorgangs beinhalten oder komplett fehlen. 
             //Sollte der Parameter fehlen oder leer gelassen werden, betrachtet SilverDAT calculatePro den Aufruf als Neuanlage eines Vorgangs.
             values.az = 9999999; //Aktenzeichen
             //Header aktivieren
             values. displayHeader = true; 
             //Menü aktivieren
             values. showProcessMenu = true;
             //onClick event handler auf dem Abschließen-Button auf der Seite, die durch den Parameter lastPage zur letzten Seite deklariert worden ist.
             //Beim Klick wird der übergeordneten Anwendung über URL-Änderung mitteilt, dass der Prozess durchlaufen ist. 
             values.defaultReadyHandler = true; 
             //Nur wenn das Product calculateExpert aufgerufen werden soll
             sphinx.productVariant = 'calculateExpert'; 
             //Dies ist eine Callback-URL, die aufgerufen wird, wenn der Anwender einen Abschließen-Button in der Anwendung betätigt. 
             //Wird es gesetzt, hängt die Anwendung ein Konstrukt, wie z.B. "?ready=xxx&cid=yyy" an die URL. 
             values.urlReadyHandler = 'http://www.urlreadyhandler.de';
             // Reifendialog deaktivieren
             values.tires = false; 
             //Drucksymbol aktivieren
             values. hidePrintIcon = true;
             //zusätzliche Parameter firstPage, lastPage 
             //Steuert der Einstiegsmaske. 
             //Sperrt alle vorhergehenden Masken. Bearbeitet werden können nur alle nachfolgenden Masken
             sphinx.firstPage = "model";
             //Steuerung der Ausstiegsmaske. Verhindert damit das Springen in darauf folgende Masken, da alle nachfolgenden Masken gesperrt sind. 
             //Bearbeitet werden können nur die bis dahin freigegebenen Masken.
             sphinx.lastPage = "calculationResult";
             //Steuert den Zielhost & Anwendung
             sphinx.host = 'https://www.dat.de/VehicleRepairOnline';
             // Sprung in die grafische Teileauswahl mit der Möglichkeit bis zur Kalkulationsergebnis-Seite (lastPage) vorzuspringen 
             sphinx.init(sphinx.host + "/VehicleRepairOnline/grapaselservice/GraphicalPartSelectionPage.html", "graphicSelectionPage", document.getElementById('iframeContainer'), "modelIFrame", null, callbackFromSphinx);
             // Mögliche Aufrufziele: eventList, contractOpening, model, equipmentPage, activityRelatedData, graphicSelectionPage, calculationResult;
             //Vorgangsübersicht
             //sphinx.init(sphinx.host + "/eventList/eventList.html",  "eventList",  document.getElementById('iframeContainer'),  "modelIFrame");
             //Auftragseröffnung
             //sphinx.init(sphinx.host + "/vehicleRepair/contractOpening.tmpl","contractOpening", document.getElementById('iframeContainer'), "modelIFrame");
             //Fahrzeugauswahl
             sphinx.init(sphinx.host + "/vehicleSelection/model.tmpl","model",document.getElementById('iframeContainer'), "modelIFrame");
             //Austattungen
             //sphinx.init(sphinx.host + "/vehicleSelection/equipmentPage.tmpl","equipmentPage", document.getElementById('iframeContainer'), "modelIFrame");
             //Vorgangsbezogene Daten
             //sphinx.init(sphinx.host +  "/vehicleRepair/vroActivityRelatedDataPage.tmpl", "activityRelatedData",  document.getElementById('iframeContainer'),  "modelIFrame");
             //Grafische Teileauswahl
             //sphinx.init(sphinx.host +  "/vehicleRepair/graphicalPartSelectionPage.tmpl", "graphicSelectionPage",  document.getElementById('iframeContainer'), "modelIFrame");
             //Kalkulationsergebnis
             //sphinx.init(sphinx.host +  "/vehicleRepair/calculationResultPage.tmpl", "calculationResultPage",  document.getElementById('iframeContainer'), "modelIFrame");
             //Drucken und senden
             //sphinx.init(sphinx.host + "/vehicleRepair/printAndSendPage.tmpl", "printAndSendPage", document.getElementById('iframeContainer'),"modelIFrame");
             //Regelsätze
             //sphinx.init(sphinx.host + "/vehicleRepair/administrationPage.tmpl", "administrationPage", document.getElementById('iframeContainer'), "modelIFrame");
             //Betriebsdaten
             //sphinx.init(sphinx.host + "/vehicleRepair/vehicleRepairOnline/companyData.html", "companyData", document.getElementById('iframeContainer'), "modelIFrame");
             //Einstellungen
             //sphinx.init(sphinx.host + "/vehicleRepair/settingsPage.tmpl", "settingsPage", document.getElementById('iframeContainer'), "modelIFrame");
             //Druckvorlagen-Verwaltung
             //sphinx.init(sphinx.host + "/vehicleRepair/layoutAdminPage.tmpl", "layoutAdminPage", document.getElementById('iframeContainer'), "modelIFrame");
             //JWT-Authentifizierung
                         $.ajax( { url: 'https://www.dat.de/AuthorizationManager/service--/endpoint/tokenService',
                        data: {
                            payload : JSON.stringify({
                                             action : "generateToken",
                                             customerNumber : "Kundennummer",
                                             user : "Benutzer",
                                             password : "Passwort"
                                         })
                            },
                        type: 'POST',
                        error: function (error) { alert(error); },
                        success: function ( data, textStatus, jqXHR ) {
                            var DAF = sphinx.getDAFXml(values);
                            var loginInfo = sphinx.encryptPassword(new DatTokenInformation(data));
                            try{
                                sphinx.execute(loginInfo, DAF, errCB);
                            }
                            catch(e){
                                document.getElementById('iframeContainer').innerHTML = e;
                            }
                        }
                    } );
        }

        function errCB(e){alert(e);}
        //Callback-Methode für die Verarbeitung eines abgeschlossenen Vorgangs
        function callbackFromSphinx(object, xml){
            //object.response = xml.xml;
            alert(xml.xml);
        }
    </script>
    <body onload="load();">
       <div id="header" class="header">
          <h3>Custom Header</h3>
       </div>
       <div id="iframeContainer"></div>
       <div id="footer" class="footer">
          <h3>Custom Footer</h3>
       </div>
    </body>
    </html>
```
