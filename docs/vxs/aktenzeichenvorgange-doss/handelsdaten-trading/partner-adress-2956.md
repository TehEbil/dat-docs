---
title: "Partner-Adressen (Owner, PrevOwner, etc.)"
topic_id: "2956"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Handelsdaten (TradingData) > Partner-Adressen (Owner, PrevOwner, etc.)"
---

# Partner-Adressen (Owner, PrevOwner, etc.)

Hier gibt es mehrere jeweils gleich aufgebaute Elemente, die jeweils unter <TradingData> zu finden sind:

Verfügbare Elemente:

| Element | Beschreibung |
| --- | --- |
| Owner | Halter |
| PrevOwner | Vorbesitzer (ehem. Halter nach Ankauf) |
| Reservation | Reservierung |
| Insurance | Versicherung |
| Insurant | Versicherungsnehmer |
| Driver | Fahrer |
| Opponent | Gegner (Versicherungsfall) |
| Expert | Sachverständiger / Experte |
| Dealership | Autohaus |
| Prospect(s) | Interessenten. Da es hier mehrere geben kann, sind die Prospect-Elemente unter einem Element Prospects zusammengefasst. |
| Garage | Werkstatt |

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| CompanyName | string | Firma |
| LastName | string | Nachname |
| FirstName | string | Vorname |
| Title | string | Anrede |
| Birthday | date | Geburtstag |
| Birthplace | string | Geburtsort |
| Country | string | Land ISO 3166 ALPHA-2 s. Werteliste Country |
| VatEntitled | boolean | USt-Abzugsberechtigt? |
| TaxNumber | string | USt-Id |
| CustomerNumber | string | Kundennummer |
| CustomerType | string | Kundenart |
| CustomerTypeShort | string | Kundenart (Kürzel) |
| Street | string | Straße + Hausnummer |
| StreetZipCode | string | PLZ für Straßenadresse |
| StreetCity | string | Ort für Straßenadresse |
| PoBox | string | Postfach |
| PoBoxZipCode | string | PLZ für Postfach |
| PoBoxCity | string | Ort für Postfach |
| EMail | string | E-Mail-Adresse |
| PhoneBusiness | string | Telefon geschäftlich |
| PhonePersonal | string | Telefon privat |
| PhoneMobile | string | Telefon mobil (Handy) |
| Fax | string | Telefax |
| Bank | string | Name der Bank |
| BIC | string | SWIFT-Adresse |
| BLZ | string | Bankleitzahl |
| AccountNo | string | Kontonummer |
| IBAN | string | International Bank Account Number |
| ContactType | string | Kontaktart |
| ContactComment | string | Kommentar zum Kontakt |
| ContactDate | string | Datum zum Kontakt |
