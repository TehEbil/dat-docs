---
title: "Ölfüllstandsmengen FillingQuantities"
topic_id: "2901"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Technische Daten (TechInfo) > Ölfüllstandsmengen FillingQuantities"
---

# Ölfüllstandsmengen FillingQuantities

| Element | Typ | Beschreibung | Abrufbar über Anwendung |
| --- | --- | --- | --- |
| Fluid | Element | Definition der Flüssigkeit als Liste | CalculatePro |

Fluid

| Element | Typ | Beschreibung | Abrufbar über Anwendung |
| --- | --- | --- | --- |
| Capacity | Element | Füllstandsmenge als Liste | CalculatePro |
| Recommendation | Element | Empfehlung von Produkten als Liste | CalculatePro |
| type | Integer | Typ der Flüssigkeit; mögliche Werte:  1 - Motoröl  andere noch nicht bekannt  zurzeit 0 | CalculatePro |
| desc | String | Benennung des Typs | CalculatePro |
| code | String | Zusätzliche Information | CalculatePro |

Capacity

| Element | Typ | Beschreibung | Abrufbar über Anwendung |
| --- | --- | --- | --- |
| type | Integer | Typ der Füllstandsmenge; möglicher Wert:  1 - Füllmenge (gesamt)  5 - Filterkapazität | CalculatePro |
| desc | String | Benennung der Füllstandsmenge | CalculatePro |
| min | Decimal | Minimale Füllstandsmenge | CalculatePro |
| max | Decimal | Maximale Füllstandsmenge | CalculatePro |
| unit | String | Maßeinheit (z.B. Liter) | CalculatePro |
| condition | String | optional, zusätzliche Information | CalculatePro |

Recommendation

| Element | Typ | Beschreibung | Abrufbar über Anwendung |
| --- | --- | --- | --- |
| Usage | String | Definitiones der Einsatzmöglichkeit; mögliche Werte (siehe auch Attribut type):  Normal Erschwert | CalculatePro |
| Interval | String | Intervallbenennung; mögliche Werte: siehe auch Attribut type):  Wechseln Prüfen | CalculatePro |
| Product | String | Produkte als Liste | CalculatePro |

Usage

| Attribut | Typ | Beschreibung | Abrufbar über Anwendung |
| --- | --- | --- | --- |
| type | integer | Einsatztyp; mögliche Werte:  0 - Normal 3449 - erschwert | CalculatePro |

Interval

| Attribut | Typ | Beschreibung | Abrufbar über Anwendung |
| --- | --- | --- | --- |
| type | integer | Intervalltyp; mögliche Werte: 1 - Wechseln 2 - Prüfen | CalculatePro |
