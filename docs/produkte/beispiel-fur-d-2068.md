---
title: "Beispiel für den Daten-Upload via POST"
topic_id: "2068"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Aufruf der Anwendungsoberfläche über Schnittstelle > Beispiel für den Daten-Upload via POST"
---

# Beispiel für den Daten-Upload via POST

```
<html>
    <body>
        <h1>Auftragserfassung via File-Upload</h1>
        File muss UTF8 encoded sein.
        <FORM ENCTYPE='multipart/form-data' method='POST' action='http://www.dat.de/GlassRep/$createcontract'>
            <INPUT TYPE="hidden" NAME="customerNumber" value="0000000" />
            <INPUT TYPE="hidden" NAME="userLogin" value="username" />
            <INPUT TYPE="hidden" NAME="signature" value="akEwRUF3TUNock1YRVUxN20rTmd5U1o0TzdmWkZLdzNadWdCOU1FRUFIekR2Ry93VDhNQSsRXc9PQ==" />
            <INPUT TYPE="hidden" NAME="productVariant" value="glassrep.agp" />
            <INPUT TYPE='file' NAME='vxsFile'>
            <INPUT TYPE='submit' VALUE='Auftrag erfassen'>
        </FORM>
        <h1>Auftragserfassung via Form Field</h1>
        <FORM method='POST' action='http://www.dat.de/GlassRep/$createcontract'>
            <textarea name="inputxml" cols="50" rows="10"></textarea>
            <INPUT TYPE="hidden" NAME="customerNumber" value="0000000" />
            <INPUT TYPE="hidden" NAME="userLogin" value="username" />
            <INPUT TYPE="hidden" NAME="signature" value="akEwRUF3TUNock1YRVUxN20rTmd5U1o0TzdmWkZLWkRiTXh1dEs5YG0yeWN2Ry93VDhNQSsvRXcPQ==" />
            <INPUT TYPE="hidden" NAME="productVariant" value="glassrep.agp" />
            <INPUT TYPE='submit' VALUE='Auftrag erfassen'>
        </FORM>
    </body>
</html>
```
