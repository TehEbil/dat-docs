---
title: "Response createDossierN mit zu hoher Laufleistung"
topic_id: "24851"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Erstellen eines neuen Vorgangs > Response createDossierN mit zu hoher Laufleistung"
---

# Response createDossierN mit zu hoher Laufleistung

Response S:Fault

| Parameter | Datentyp | Beschreibung |
| --- | --- | --- |
| faultcode | String | dat:S:Server |
| faultString | String | NOT\_EVALUABLE invalid mileage/+/0/368000 |
| faultActor | String | de.dat.sphinx.valadv.trading.business.TradingDossierHandler |
| detail |  | siehe Unterelemente |

Unterelemente von detail

| Parameter | Datentyp | Beschreibung |
| --- | --- | --- |
| datMileageCorrMin | Decimal | Laufleistungskorrektur für die minimal bewertbare Laufleistung |
| datMileageCorrMax | Decimal | Laufleistungskorrektur für die bewertbare mögliche Laufleistung |
| datMileageMin | Integer | minimal bewertbare Laufleistung |
| datMileageMax | Integer | maximal bewertbare Laufleistung |

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <S:Fault>
         <faultcode xmlns:dat="http://www.dat.de">dat:S:Server</faultcode>
         <faultstring>NOT_EVALUABLE invalid mileage/+/74000/1074000</faultstring>
         <faultactor>de.dat.sphinx.valadv.trading.business.TradingDossierHandler</faultactor>
         <detail>
            <datMileageCorrMin>7445.69</datMileageCorrMin>
            <datMileageCorrMax>-11633.90</datMileageCorrMax>
            <datMileageMin>74000</datMileageMin>
            <datMileageMax>1074000</datMileageMax>
         </detail>
      </S:Fault>
   </S:Body>
</S:Envelope>
```
