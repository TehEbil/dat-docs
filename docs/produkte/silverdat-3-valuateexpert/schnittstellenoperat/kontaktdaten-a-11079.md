---
title: "Kontaktdaten anlegen"
topic_id: "11079"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Kontaktdaten anlegen"
---

# Kontaktdaten anlegen

Mit der Funktion setContactData legen Sie die Kontaktdaten zu einem bestehenden Vorgang an.

Parameter setContactData

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Eindeutige Vorgangskennung | numerisch | X |
| Salutation | String | Anrede | COMP=Firma  MR=Herr  MRS=Frau |  |
| Street | String | Straße |  |  |
| City | String | Stadt |  |  |
| VatNumber | String | Umsatzsteuernummer |  |  |
| zipN | String | Postleitzahl | 0-99999 |  |
| FirstName | String | Vorname |  |  |
| LastName | String | Nachname |  |  |
| Name2 | String | weiterer Name |  |  |
| Company | String | Firma |  |  |
| CustomerContactdata | CustomerContactdata | Enthält die Kontaktdaten als Kindelemente |  |  |
| CustomerKind | String | Kundenart, Defaultwert = DVR | RQSTR=Auftraggeber  DVR=Halter  WSHP=Autohaus Werkstatt  LCUST=Leasing Kunde |  |
| CustomerNumber | String | Kundennummer |  |  |
| CustomerType | String | Kunden-Typ | NONE=Kein(e)  SINGL=Einzeln  FMLY=Familie  CMRCE=Handel  TRADE=Gewerbe |  |
| PrivacyPolicy | privacyPolicyRequest | Enthält die Vorgaben für die Privatsphäre als Kindelemente |  |  |

Element vxs:CustomerContactdata

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| EMail | String | E-Mail |  |  |
| Fax | String | Fax |  |  |
| PhoneMobile | String | Telefon mobil |  |  |
| PhoneBusiness | String | Telefon geschäftlich |  |  |

Element vxs:PrivacyPolicy

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ByEmail | String | per E-Mail | YES=Ja  NO=Nein  NA=nicht zutreffend |  |
| ByMobilePhone | String | per Mobiltelefon | YES=Ja  NO=Nein  NA=nicht zutreffend |  |
| ByPhoneOrFax | String | per Telefon/Fax | YES=Ja  NO=Nein  NA=nicht zutreffend |  |
| ByPost | String | Postalisch | YES=Ja  NO=Nein  NA=nicht zutreffend |  |
| DateOfPrivacyPolicy | Date | Datum der Datenschutzerklärung | JJJJ-MM-DD |  |
| RecordPrivacyPolicy | Boolean | Datenschutzerklärung erfassen | true=Ja  false=Nein |  |
