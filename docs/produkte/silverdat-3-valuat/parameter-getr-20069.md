---
title: "Parameter getReferenceMileageForVehicle"
topic_id: "20069"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Hilfsfunktionen > Bezugsfahrstrecke eines Fahrzeugs abfragen > Parameter getReferenceMileageForVehicle"
---

# Parameter getReferenceMileageForVehicle

Element request

| Parameter | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- |
| actualCdYearMonth | Datenmonat | YYYYMM |  |
| constructionTime | Bauzeit | 4-stellig, numerisch | bedingt entweder constructionTime oder initialRegistration muss angegeben werden |
| initialRegistration | Erstzulassung | YYYY-MM-DD | bedingt entweder constructionTime oder initialRegistration muss angegeben werden |
| container | Marktindex | [Landessetzung, 2stellig][Nummer des Marktindex, 3stellig] | X |
| datECode | DAT €uropa-Code® | 15-stellig, numerisch | X |
