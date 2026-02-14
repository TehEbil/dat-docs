---
title: "Kundendaten anlegen oder ändern"
topic_id: "14799"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Kundendaten anlegen oder ändern"
---

# Kundendaten anlegen oder ändern

Mit der Funktion createOrUpdateContactData legen Sie Kundendaten (Adresse, Telefonnummer) an oder ändern diese. Für einen Vorgang
der SilverDAT 3 PRO kann jeweils nur ein Halter owner und ein Käufer buyer angelegt werden. Wenn Sie das Element overwrite auf true setzen, überschreiben Sie die bestehenden Kontaktdaten.

Request createOrUpdateContactData

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| contractId | long | Eindeutige Vorgangsnummer |  | X |
| contactData | contactData | Besitzt Unterelemente (siehe unten) |  | X |
| overwrite | Boolean | Bei true werden die Kontaktdaten überschrieben | true false | bedingt |

Element contactData

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| address | contactDataAddress | Besitzt Unterelemente (siehe unten) |  |  |
| common | contactDataCommon | Siehe Element common |  | X |
| privacyPolicy | contactDataPrivacyPolicy | Siehe Element privacyPolicy |  |  |
| taxationInfo | contactDataTaxationInfo | Siehe Element taxationInfo |  |  |
| comment | string | Bemerkung |  |  |

Element address

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| addressType | addressType | Kontaktart | accounting delivery contact defaultContact |  |
| country | dataCountry | Land |  |  |
| email | string | E-Mail Addresse |  |  |
| fax | string | Fax |  |  |
| phoneBusiness | string | geschäftliche Telefonnummer |  |  |
| phoneMobile | string | Mobiltelefon |  |  |
| phonePersonal | string | private Telefonnummer |  |  |
| poBox | string | Postfach |  |  |
| poBoxZipCode | string | Postleitzahl |  |  |
| street | string | Straße |  |  |
| streetCity | string | Ort |  |  |
| streetNumber | string | Straßennummer |  |  |
| streetZipCode | string | Postleitzahl |  |  |

Element common

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| birthday | dateTime | Geburtstag | YYYY-MM-DD |  |
| birthplace | string | Geburtsort |  |  |
| companyName | string | Name |  |  |
| contactDataType | addresskind | Kontaktart | buyer owner | X |
| firstName | string | Vorname |  |  |
| lastName | string | Nachname |  | X |
| title | string | Anrede |  |  |

Element privacyPolicy

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| byEmail | string | Bei Belegung mit 1 darf der Kunde per Email kontaktiert werden. | 0 1 |  |
| byMobilePhone | string | Bei Belegung mit 1 darf der Kunde per Telefon kontaktiert werden. | 0 1 |  |
| byPhoneOrFax | string | Bei Belegung mit 1 darf der Kunde per Fax kontaktiert werden. | 0 1 |  |
| byPost | string | Bei Belegung mit 1 darf der Kunde per Post kontaktiert werden. | 0 1 |  |
| dateOfPrivacyPolicy | dateTime | Datum der Datenschutzerklärung | YYYY-MM-DD |  |
| entryDate | dateTime | Eintragsdatum | YYYY-MM-DD |  |
| recordPrivacyPolicy | boolean | Datenschutzerklärung liegt vor | true false |  |
| user | string | Benutzername |  |  |

Element taxationInfo

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| customerBase | addressState | Kundenart Hier können Sie zusätzlich eigene Werte in den Stammdaten anlegen. | none single family commerce trade |  |
| customerNumber | string | Kundennummer |  |  |
| taxNumber | string | Steuernummer |  |  |
