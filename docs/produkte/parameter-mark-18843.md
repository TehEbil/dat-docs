---
title: "Parameter MarketDataFromVXS"
topic_id: "18843"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Börsendaten via webScan REST-API abrufen > Funktionsumfang webScan > Parameter MarketDataFromVXS"
---

# Parameter MarketDataFromVXS

###### Parameter MarketDataFromVXS Element data | Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht | | --- | --- | --- | --- | --- | | Dossier | Dossier | Enthält die VXS Dossier Struktur. | | X | Element Dossier | Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht | | --- | --- | --- | --- | --- | | Language | String | Sprachkürzel | Sprachkürzel (Language) | X | | Vehicle | Vehicle | Enthält bewertungsrelevante Daten als Unterelemente | | X | Element Vehicle | Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht | | --- | --- | --- | --- | --- | | Country | String | Landeskürzel des betreffenden Datenlands | ISO 3166 ALPHA-2 weitere Infos siehe Popup-Fenster | X | | DatECode | String | DAT €uropa-Code® | 15-stellig | X | | Container | String | Marktindex | [Landessetzung, 2-stellig][Nummer des Marktindex, 3-stellig] | X | | ConstructionTime | Integer | Bauzeit weitere Infos siehe Popup-Fenster | 4-stellig numerisch | X | | MileageEstimated | Integer | Kilometerstand | numerisch | X | | InitialRegistration | Date | Erstzulassungsdatum | YYYY-MM-DD | X |
