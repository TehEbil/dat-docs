---
title: "Stammdaten holen"
topic_id: "12216"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Stammdaten holen"
---

# Stammdaten holen

Mithilfe der nachfolgenden beschriebenen Funktionen holen Sie die Stammdaten, die
Sie für das Umbuchen benötigen. Die Werte aus den Stammdaten benötigen Sie unter anderem
für die Funktionen setPurchaseData, setAdmissionData und setSalesData, die für SilverDAT 3 Pro verfügbar sind.

Übersicht der Funktionen

| Funktion | Beschreibung | Service |
| --- | --- | --- |
| getAcceptanceDetailsList | Holen der Hereinnahmedaten | TradingServiceN |
| getVehicleGroupList | Holen der Fahrzeuggruppen | TradingServiceN |
| getBusinessTypeList | Holen der Geschäftsarten | TradingServiceN |
| getSalesDetailsList | Holen der Verkaufsangaben | TradingServiceN |
| getPossibleContactPersons | Holen der Ansprechpartner | MyClaimExternalService |

Übersicht für die Verwendung der Funktionen

| Funktionen | enthalten den Parameter | Abhängigkeit zu der Funktion |
| --- | --- | --- |
| getAcceptanceDetailsListResponse | AcceptanceDetails | setPurchaseData  setAdmissionData |
| getVehicleGroupListResponse | VehicleGroup | setPurchaseData  setAdmissionData  setSalesData |
| getBusinessTypeListResponse | BusinessType | setSalesData |
| getSalesDetailsListResponse | SalesDetails | setSalesData |
| getPossibleContactPersons | BuyerId, SellerId | setPurchaseData  setAdmissionData  setSalesData |

Für weitere Informationen siehe Kapitel "Status umbuchen".

WSDL

https://www.dat.de/myClaim/soap/v2/TradingServiceN?wsdl

https://www.dat.de/myClaim/soap/v2/MyClaimExternalService?wsdl

Serviceaufruf

https://www.dat.de/myClaim/soap/v2/TradingServiceN

https://www.dat.de/myClaim/soap/v2/MyClaimExternalService
