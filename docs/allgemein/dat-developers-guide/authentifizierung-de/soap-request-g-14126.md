---
title: "SOAP-Request generateToken"
topic_id: "14126"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Authentifizierung der SilverDAT Webservices > JSON Web Token Authentication (DAT-AuthorizationToken) > SOAP-Request generateToken"
---

# SOAP-Request generateToken

Jede DAT-Online-Anwendung stellt im Authentication-Service die SOAP-Schnittstellenfunktion generateToken zur Verfügung.

Beispiele für applikationseigene Service-URLs:

| SilverDAT Anwendung | WSDL |
| --- | --- |
| SilverDAT 3 PRO | https://www.datgroup.com/myClaim/soap/v2/MyClaimExternalAuthenticationService?wsdl |
| [Autoglas Plus SilverDAT inside + SilverDAT calculateGlass](../../../produkte/autoglas-plus-silverdat-i/index.md) | https://www.datgroup.com/GlassRep/services/Authentication?wsdl |
| [SilverDAT 3 valuateFinance](../../../produkte/silverdat-3-valuatefinanc/index.md) | https://www.datgroup.com/FinanceLine/soap/Authentication?wsdl |
| SilverDAT 3 valuateExpert/  PlusPartner | https://www.datgroup.com/valuateNG/soap/Authentication?wsdl |
| [SilverDAT calculatePro](../../../produkte/silverdat-calculatepro-si/index.md) | https://www.datgroup.com/VehicleRepairOnline/services/Authentication?wsdl |
| DAT €uropa-Code® Fahrzeugauswahl | https://www.datgroup.com/DATECodeSelection/services/Authentication?wsdl |

Es ist jeweils der Service des DAT-Produktes zu verwenden, dessen Service-Funktion
bei dem im Anschluss folgenden Aufruf der eigentlichen Webservice-Funktion verwendet
wird.
