---
title: "Aufbereitung der Authentifizierungsinformationen"
topic_id: "1859"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Oberflächen-Schnittstelle > Integration der Oberfläche > Aufbereitung der Authentifizierungsinformationen"
---

# Aufbereitung der Authentifizierungsinformationen

Die DAT €uropa-Code® Fahrzeugauswahl benötigt folgende Elemente zur Authentifizierung:

- DAT Kundennummer, 7-stellig
- Benutzername
- Passwort

Mit diesen Elementen wird über die Funktion generateToken aus dem AuthenticationService ein DAT-AuthorizationToken erzeugt. Das Token kann dann in Form eines JavaScript-Objekts vom Typ DatLoginInformation für den Start der Applikation übermittelt werden. Die entsprechende Klasse ist in sphinx.js definiert.

```
  // authentication through DAT-AuthorizationToken
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
    ...
    // call Sphinx (DATECodeSelection)
    ...
    }
  });
```

Authentifizierungsinformationen mit Passwort aus Sicherheitsgründen niemals innerhalb
JavaScript senden! Der Schnittstellenpartner sollte unbedingt die Daten für das Erzeugen
des DAT-AuthorizationToken durch einen POST von seinem eigenen Server generieren oder eine vergleichbare Umsetzung
implementieren.
