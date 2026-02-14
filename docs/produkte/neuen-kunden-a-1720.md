---
title: "Neuen Kunden anlegen oder deaktivierten Kunden reaktivieren: createCustomer"
topic_id: "1720"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Customer Service > Customer Service Schnittstellenoperationen > Neuen Kunden anlegen oder deaktivierten Kunden reaktivieren: createCustomer"
---

# Neuen Kunden anlegen oder deaktivierten Kunden reaktivieren: createCustomer

Erzeugt einen neuen Kindkunden für einen DAT Kunden (Vaterkunde). Bei Anlage einer
neuen Kundennummer wird automatisch ein neuer Benutzer erstellt und in der Antwort
zurückgegeben.

Die Funktion kann ebenfalls dazu verwendet werden, um einen über die Funktion [disableCustomer](#showid/1736 "Kunde deaktivieren: disableCustomer") deaktivierten Kunden wieder zu reaktivieren.

Sind Eingabeparameter ungültig, wird der Funktionsaufruf mit einer Exception abgebrochen.
