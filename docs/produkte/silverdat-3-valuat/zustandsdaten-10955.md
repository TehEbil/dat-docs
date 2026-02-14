---
title: "Zustandsdaten löschen"
topic_id: "10955"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Zustandsdaten löschen"
---

# Zustandsdaten löschen

Mit der Funktion deleteConditionDetails löschen Sie Zustandsdetails aus einem bestehenden Vorgang. Die einzelnen Id's RepairCostId, ValueIncreaseId und ValueReductionId lassen sich ebenfalls löschen.

Die Funktion deleteConditionDetails setzt die Parameter RepairCostsGross, RepairCosts, DecreaseInValueGross, DecreaseInValue, IncreaseInValueGross und IncreaseInValue zurück.

Parameter deleteConditionDetails

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Eindeutige Vorgangskennung | numerisch | x |
| RepairCostIdList | repairCostIdList | Die zugehörigen Kindelemente enthalten die Zustandsdetails der Kategorie: Reparaturkosten |  | bedingt |
| ValueIncreaseIdList | valueIncreaseIdList | Die zugehörigen Kindelemente enthalten die Zustandsdetails der Kategorie: Werterhöhungen |  | bedingt |
| ValueReductionIdList | valueReductionIdList | Die zugehörigen Kindelemente enthalten die Zustandsdetails der Kategorie: Wertminderungen |  | bedingt |

Element vxs:RepairCostIdList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| RepairCostId | Long | Eindeutige Nummerierung der Reparaturkosten | numerisch | bedingt |

Element vxs:ValueIncreaseIdList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ValueIncreaseId | Long | Eindeutige Nummerierung der Werterhöhung | numerisch | bedingt |

Element vxs:ValueReductionIdList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ValueReductionId | Long | Eindeutige Nummerierung der Wertminderung | numerisch | bedingt |
