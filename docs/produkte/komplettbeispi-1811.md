---
title: "Komplettbeispiel"
topic_id: "1811"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Oberflächen-Schnittstelle > Integration der Oberfläche > Komplettbeispiel"
---

# Komplettbeispiel

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
  <head>
    <style> 
    body { border: none; margin: none; }
    .modelIFrame{
      width: 100%;
      height: 720px;
      border: none;
    }
    .header{
      width: 100%;
      height: 10%;
      border: 1px solid #898B8D;
      text-align:center;
      margin-bottom: 10px;
      background: #DBD8D4;
    }
    .footer{
      width: 100%;
      height: 5%;
      border: 1px solid #898B8D;
      text-align:center;
      margin-top: 10px;
      background: #DBD8D4;
    }
    </style>
    <script language="JavaScript" src="https://www.dat.de/sphinx/js/lazyload.js" type="text/javascript"></script>
    <script language="JavaScript" src="https://www.dat.de/sphinx/js/externalSphinx.js" type="text/javascript"></script>
    <script language="JavaScript" src="https://code.jquery.com/jquery-2.2.4.min.js" type="application/javascript"></script>
    <script type="text/javascript" language="JavaScript">
  function callbackFromSphinx ( object, xml ){
    //either delete Sphinx iFrame
    //sphinx.deleteIframe();
    //and then add your own content to the DOM tree
    //or alert ( xml);
    //or submit response to another page
    //document.myForm.datResponse.value=xml;
    //document.myForm.submit();
    alert("Vehicle selection is ready: " + xml.xml);
  }

  //handle error messages
  function errorFunc(e){
    alert(e);
  }

  function load(){
    var values = new Object();

    // don't show DAT header
    values.displayHeader = false;

    // hide VIN-query button
    //values.withoutVinQueryButton = true;

    //vehicle filter restriction, one of ALL, REPAIR or APPRAISAL, default = ALL
    values.Restriction = 'APPRAISAL';
    // prohibit the change of Restriction (if true the Restriction selection is hidden)
    values.noRestrictionInp = true;

    // Country code for the target market (international licence plate country code, 3 chars)
    // corresponds to the datCountryIndicator (Values: 'D', 'A', 'CH', 'I', 'E', 'F', ...)
    //values.CountryCode = 'I';

    // DossierID for loading a instance from database to the application
    //values.az = '123456'

    //DAT Europa-Code
    values.DatECode = '018601250190001';
    //or splitted DAT Europa-Code
    //values.VehicleType = 1;
    //values.Manufacturer = 860;
    //values.BaseModel = 125;
    //values.SubModel = 19;
    //values.SubModelVariant = 1;

    //Container
    values.Container = 'DE001';

    //VehicleIdentification Number
    //values.VehicleIdentNumber = '';

    //KBA 
    //values.KbaCode = ''; 

    // NatCode (for Austria only)
    //values.natCode = '';

    // Licence plate (for Italy and Switzerland only)
    //values.licencePlate = '';

    // Base number (for Switzerland only)
    //values.baseNumber = '';

    // Type note number (for Switzerland only)
    //values.typeNoteNumber = '';

    //if available vehicle initial registration date in milliseconds since 1/1/1970 
    values.InitialRegistration = 1390387939000; 
    //values.constructionTime = 4900;

    // equipment filter, one of ALL, GENERAL, EXTERIOR, INTERIOR, CHASSIS, AGGREGATE or GLASS (default = ALL)
    values.equFilter = 'ALL';
    // comma separated list of dat standard/orptional equipment numbers (eg. '23605,73606')
    values.equDatNr = '';
    // comma separated list of additional equipments (eg. 'auxiliary heating, auxiliary lights')
    values.equAdd = '';

    // save selection at the end of process
    values.withSaveAsEvent = true;
    values.eventName = 'from external';

    // set the pageflow (possible values: 'model selection', 'equipment selection', 'vehicle summary' and 'vehicle data')
    sphinx.firstPage = 'model selection';
    sphinx.lastPage = 'vehicle data';
    var destination = 'model selection';

    // host: DAT €uropa Code vehicle selection
    sphinx.host='https://www.dat.de/DATECodeSelection';
    sphinx.init(sphinx.host + "/vehicleSelection/model.tmpl", "model", document.getElementById('iframeContainer'), "modelIFrame", null, callbackFromSphinx);

    // authentication through DAT-AuthorizationToken
    $.ajax( { url: 'https://www.dat.de/AuthorizationManager/service--/endpoint/tokenService',
      data: {
        payload : JSON.stringify({
          action : "generateToken",
          customerNumber : "your_CustomerNumber",
          user : "your_CustomerLogin",
          password : "your_Password"
        })
      },
    type: 'POST',
    error: function (error) { alert(error); },
    success: function ( data, textStatus, jqXHR ) {
      var DAF = sphinx.getDAFXml(values);
      var loginInfo = sphinx.encryptPassword(new DatTokenInformation(data));
      // call Sphinx
      try{
        sphinx.execute(loginInfo, DAF, errorFunc);
      }
      catch(e){
        document.getElementById('iframeContainer').innerHTML = e;
      }
    }
    });
  }
  </script>
  </head>
  <body onload="load();">
    <div id="header" class="header">
      <h3>Custom Header</h3>
      <h4>Prozess: Modell -> Ausstattungen -> Zusammenfassung -> Fahrzeugdaten -> Speichern in Datenbank</h4>
    </div>
    <div id="iframeContainer"></div>
    <div id="footer" class="footer"><h3>Custom Footer</h3></div>
      <form name="myForm" method="post" action="http://www.cs.tut.fi/cgi-bin/run/~jkorpela/echo.cgi"/>
      <input type="hidden" name="datResponse" value="" />
      </form>
  </body>
</html>
```
