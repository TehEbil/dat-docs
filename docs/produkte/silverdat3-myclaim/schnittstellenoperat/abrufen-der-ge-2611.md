---
title: "Abrufen der Geo Koordinaten einer angegeben Adresse"
topic_id: "2611"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Abrufen der Geo Koordinaten einer angegeben Adresse"
---

# Abrufen der Geo Koordinaten einer angegeben Adresse

Die Funktion getGeoCoordinates ermöglicht es anhand von übergebenen Adressdaten, dessen Geografischen Koordinaten
zu bestimmen. Als Antwort werden somit die Werte der Breiten,- und Längengrade zurückgegeben.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| streetNr | String | 1 | Straßennummer |  |
| street | String | Musterweg | Straße |  |
| zip | String | 70700 | Postleitzahl |  |
| city | String | Musterstadt | Stadt | X |
| isoCountryCode | String | DE | Ländercode | X |

Rückgabe

Längengrad (lng) und Breitengrad (lat) der Angegebenen Adresse
