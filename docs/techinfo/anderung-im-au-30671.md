---
title: "Änderung im Aufruf der Oberflächenintegration"
topic_id: "30671"
breadcrumb: "Technische Informationen > Ausgabe Nr. 92 August 2025 > Fahrzeugbewertung > valuateExpert/valuateExpertPlusPartner > Abkündigungen > Änderung im Aufruf der Oberflächenintegration"
---

# Änderung im Aufruf der Oberflächenintegration

Mit dem Release Oktober 2025 wird es eine inkompatible Änderung der Oberflächenschnittstelle
der SilverDAT 3 valuateExpert und SilverDAT 3 valuateExpertPlusPartner geben.

Diese Anpassung ist technisch notwendig um mit der Sperrung von Drittanbieter-Cookies
umgehen zu können.

Bisher kann die Oberflächenschnittstelle folgendermaßen aufgerufen werden:

```
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
valuateNGExternal.execute();
```

Zukünftig muss der Aufruf, wie im folgenden Beispiel aussehen:

```
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
```

Die Zeile

```
valuateNGExternal.execute();
```

muss zwingend durch die beiden Zeilen

```
valuateNGExternal.login();
valuateNGExternal.setOnLoginSuccess(valuateNGExternal.execute);
```

ersetzt werden.

Der neue Aufruf kann ab sofort verwendet werden.

Bitte führen Sie die entsprechenden Anpassungen bis zum Release Oktober 2025 durch,
sodass auch nach dem Update alles erwartungsgemäß funktioniert.
