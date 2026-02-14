---
title: "SparePartsVehicle"
topic_id: "17201"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Datentypen > SparePartsResultPerSparePartNumber > SparePartsVehicles > SparePartsVehicle"
---

# SparePartsVehicle

| Attribut | Typ | Beschreibung |
| --- | --- | --- |
| datProcessNumber | Integer | DAT-interne Datenverarbeitungsnummer (DVN) |
| partNumber | String | Ersatzteilnummer |
| vehicleType | Integer | Fahrzeugart |
| vehicleTypeName | String | Fahrzeugartbenennung |
| manufacturer | Integer | Hersteller |
| manufacturerName | String | Herstellerbenennung |
| baseModel | Integer | Haupttyp |
| baseModelName | String | Haupttypbenennung |
| constructionTimeFrom | Integer | Bauzeit von |
| constructionTimeTo | Integer | Bauzeit bis |
| constructionCondition | String | Verbauungsbedingung |
| excludingCondition | String | Ausschlussbedingung |
| manufacturerCodeCondition | String | Herstellercodes |
| vinCondition | String | Die letzten angegebenen Stellen müssen alphanumerisch größer sein |
| descriptionIdentifier | String | Kennzeichen, welche Beschreibung verwendet werden soll, wenn für das Teil mehrere Beschreibungen möglich sind |
| [sparePartsSubModels](sparepartssubm-17207.md) | complexType, [SparePartsSubModels[]](sparepartssubm-17207.md) | Liste Untertypen |
