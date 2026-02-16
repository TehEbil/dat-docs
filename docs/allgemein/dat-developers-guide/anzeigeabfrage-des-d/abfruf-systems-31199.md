---
title: "Abfruf Systemstatus über Schnittstelle"
topic_id: "31199"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Anzeige/Abfrage des DAT Systemstatus > Abfruf Systemstatus über Schnittstelle"
---

# Abfruf Systemstatus über Schnittstelle

Um den Systemstatus abzurufen, steht Ihnen die Schnittstellenfunktion getSystemStatus.json zur Verfügung. Diese Funktion ist ausschließlich über das REST-Protokoll zugänglich.
Zur Authentifizierung benötigen Sie ein DAT-AuthorizationToken, das im HTTP-Header übermittelt werden muss.

Im Gegensatz zur Nutzung der API in unseren Anwendungen erfordert hier die Generierung
des DAT-AuthorizationToken lediglich die folgenden Parameter: customerNumber, customerName und customerPassword. Ein DAT-AuthorizationToken das mit allen Parametern erzeugt wurde funktioniert selbstverständlich
auch. Detaillierte Informationen zur Erstellung eines Tokens finden Sie im Kompendium
unter dem Abschnitt "[generateToken](../authentifizierung-de/soap-request-g-14126.md)".

Bitte beachten Sie, dass für den Aufruf der Funktion keine zusätzlichen Parameter
erforderlich sind; ein leerer Body genügt.

Beispiel Request:

```
POST https://www.datgroup.com/getSystemStatus.json
DAT-AuthorizationToken: eyJhbGciOiJIU...TTh08GqgUKJRdxTWcQ0M
```

Beispiel Response:

```
{
    "lasttimemodified": 1756733102,
    "Applications": {
        "authorizationmanager": {
            "key": "authorizationmanager",
            "name": "User Administration Service",
            "description": "Administration von Benutzerdaten und Rechten",
            "status": 1
        },
        "datecodeselection": {
            "key": "datecodeselection",
            "name": "DAT Europacode Selection",
            "description": "Fahrzeugidentifikation für Schnittstellenpartner",
            "status": 1
        },
        "financeline": {
            "key": "financeline",
            "name": "valuation Service for Finance",
            "description": "Gebrauchtfahrzeugbewertung für Banken und Leasinggesellschaften",
            "status": 1
        },
        "myclaim": {
            "key": "myclaim",
            "name": "myClaim Service",
            "description": "SilverDAT 3 / myClaim inkl. kundenspezifischer Varianten",
            "status": 1
        },
        "myclaim - api": {
            "key": "myclaim - api",
            "name": "myClaim API Service",
            "description": "Schnittstellenservice für SilverDAT 3 / myClaim inkl. kundenspezifischer Varianten",
            "status": 1
        },
        "vehiclerepaironline": {
            "key": "vehiclerepaironline",
            "name": "calculation Service",
            "description": "Reparaturkostenkalkulation für Autohaus / Werkstatt / Sachverständige",
            "status": 1
        },
        "vehiclerepaironline - api": {
            "key": "vehiclerepaironline - api",
            "name": "calculation API Service",
            "description": "Schnittstellenservice für Reparaturkostenkalkulation für Autohaus / Werkstatt / Sachverständige",
            "status": 1
        }
    },
    "message": "Aktuelle Information: Wegen Wartungsarbeiten kein Zugriff auf www.dat.de und Online-Anwendungen am Samstag, xx.xx. ab 18 bis 24 Uhr",
    "status": "OK",
    "lastTimeModified": "01.09.2025 15:20"
}
```
