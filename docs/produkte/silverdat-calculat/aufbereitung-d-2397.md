---
title: "Aufbereitung der Authentifizierungsinformationen"
topic_id: "2397"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Integration der Oberfläche > Aufbereitung der Authentifizierungsinformationen"
---

# Aufbereitung der Authentifizierungsinformationen

Die Authentifizierungsdaten werden in einem JavaScript Objekt vom Typ DatTokenInformation gekapselt. Das Objekt ist in externalsphinx.js definiert.

Dem Konstruktor müssen die folgenden Authentifizierungsinformationen übergeben werden.

- DAT Kundennummer, 7-stellig
- Benutzername
- Passwort

Im einfachsten - jedoch auch unsichersten und daher nicht empfohlenen - Fall stellt
sich das Aufbereiten der Authentifizierungsinformationen wie folgt dar. Die Methode
sphinx.encryptPassword() akzeptiert sowohl ein DatTokenInformation Objekt als auch ein Referenz auf eine Callback Funktion die ein DatTokenInformation Objekt zurückgibt.

```
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
```

Die Authentifizierungsinformationen beinhalten das Passwort und sollten daher aus
Sicherheitsgründen niemals direkt in JavaScript angegeben werden. Stattdessen sollten die Schnittstellenpartner aus Sicherheitsgründen
die Daten für das Erstellen des DatLoginInformation-Objekts durch einen XMLHttpRequest von seinem eigenen Server laden oder eine vergleichbare Umsetzung implementieren.
