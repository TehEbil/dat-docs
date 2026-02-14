---
title: "CustomerDataExt"
topic_id: "1722"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Customer Service > Datentypen > CustomerDataExt"
---

# CustomerDataExt

"customerName1" Element : String[30], Pflicht

Der Firmenname oder Kundenname als String.

Das Element ist zwingend erforderlich und auf maximal 30 Zeichen begrenzt.

"customerName2" Element : String[30], optional

Ergänzendes Element zum Feld "customerName1". Kann z.B. für den Firmenname/Kundenname oder einen Namenszusatz genutzt werden.

Das Element ist optional und auf 30 Zeichen begrenzt.

"customerName3" Element : String[30], optional

Ergänzendes Element zum Feld "customerName2". Kann z.B. für den Firmenname/Kundenname oder einen Namenszusatz genutzt werden.

Das Element ist optional und auf 30 Zeichen begrenzt.

"customerStreet" Element : String[40]

Der Straßenname des Kunden.

"customerStreetNumber" Element : String[20], optional

Die Hausnummer des Kunden.

"customerZip" : String[10]

Die Postleitzahl des Kunden.

"customerCity" : String[40]

Der Ort des Kunden.

"customerCountry" : String[2]

Die Landeskennung nach ISO2. Sie ist immer zweistellig.

"customerTel" : String[20], optional

Telefonnummer.

"customerEmail" : String[100]

E-Mailadresse.

"externalCustomerID" : String[12]

Externe Kundennummer.
