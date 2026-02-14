---
title: "getData Request (Beispiel)"
topic_id: "14146"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Authentifizierung der SilverDAT Webservices > Delegated Sign On (DSO) Service > getData Request (Beispiel)"
---

# getData Request (Beispiel)

HTTP POST-Request

Der DSO-Partner übergibt den von der DAT an den DSO-Partner übermittelten token als
"dsoToken" an die DSO-Webservicefunktion "getData".

| Name | Datentyp | mögliche Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| dsoToken | String | dynamisch erzeugt | Von der DAT dynamisch erzeugt und an den DSO-Partner übermittelter token. | X |

Beispiel für einen dsoToken-Wert:

eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJkYXQiLCJpZCI6IjM1ZDdhOWNjLWVmMDgtNGRmNi1iYzFiLTcyYTAyMDAzMjVlMyJ9.tOZEBlJg45fwcDhr80AFMeB4z0G-Ym5qsFn2nxBbFII
