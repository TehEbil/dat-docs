---
title: "getConstructionPeriodsN"
topic_id: "8152"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getConstructionPeriodsN"
---

# getConstructionPeriodsN

Beschreibung

Funktion, die mithilfe des DAT €uropa-Code® und des Marktindex den verfügbaren Bauzeitraum liefert. Der Bauzeitraum wird eingegrenzt
durch die Angabe von Bauzeitbeginn und Bauzeitende.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| restriction | Enumeration | ALL / REPAIR / APPRAISAL | Alle Daten / nur FI-Daten / nur FB-Daten durchsuchen | X |
| DatECode | String | DAT €uropa-Code | Gültiger DAT €uropa-Code | X |
| Container | String | Marktindex | Gültiger Marktindex |  |

Rückgabe

Zurückgeliefert werden Bauzeitbeginn und Bauzeitende jeweils in der Form Monat/Jahr
verschlüsselt in DAT-Notation und eine Liste aller vorhandenen Bauzeiten. Diese Liste
enthält folgende Informationen:

- ist mit Bauzeitklassen (true/false)
- ist mit Modelljahr (true/false)
- Bauzeitbeginn und Bauzeitende der Liste in DAT-Notation
- Bauzeitklassen mir Name und Wert (Bauzeit in DAT-Notation)

WSDL

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>?wsdl

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | services | VehicleSelectionService |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | services | VehicleSelectionService |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | services | VehicleSelectionService |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | soap | VehicleSelectionService |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | soap | VehicleSelectionService |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | soap/v2 | VehicleSelectionService |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | soap/v2 | VehicleSelectionService |
