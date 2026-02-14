---
title: "Auflisten der Adressbücher"
topic_id: "14237"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Adressbuchverwaltung > Auflisten der Adressbücher"
---

# Auflisten der Adressbücher

listAddressBook

Listet alle Adressbücher entsprechend der Filterkriterien z.B. nach Stadt, Name Postleitzahl
usw.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| filter | ContactPerson | city, firstName, email....... | Kontaktperson Filterparameter zur weiteren Eingränzung der Suche | X |
| pageLimit | Int |  | Schränkt die Anzahl der aufgelisteten Aufträge ein. |  |
| pageOffset | Int |  | Überspringt die übergebene Anzahl an Datensätzen bis der erste Auftrag angezeigt wird. |  |

Rückgabe

Liste aller Adressbücher
