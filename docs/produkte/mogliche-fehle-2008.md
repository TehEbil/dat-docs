---
title: "Mögliche Fehlercodes getVehicleIdentificationByCodeSwitzerland"
topic_id: "2008"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation Schweiz - anhand Kennzeichen, Stammnummer oder Typenscheinnummer > Mögliche Fehlercodes getVehicleIdentificationByCodeSwitzerland"
---

# Mögliche Fehlercodes getVehicleIdentificationByCodeSwitzerland

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| missing licence plate, baseNumber or type note number | Either licence plate or base number or type note number must be given. | Es muss entweder der Parameter licencePlate (Kennzeichen), der Parameter baseNumber (Stammnummer) oder der Parameter typeNoteNumber (Typenscheinnummer) angegeben werden. |
| Type note number plate in illegal format | The type note number must match the following regular expression: "[0-9][A-Z][0-9A-Z][0-9][0-9][0-9]" | Der Parameter typeNoteNumber (Typenscheinnummer) wurde in einem falschen Format angegeben (genau 6 Stellen, die erste und die letzten drei Stellen als Ziffern, die zweite als Großbuchstabe, die dritte als Ziffer oder Großbuchstabe). |
| Base number plate in illegal format | The base number must match the following regular expression: "[0-9]{3}\\.[0-9]{3}\\.[0-9]{3}" | Der Parameter baseNumber (Stammnummer) wurde in einem falschen Format angegeben (drei dreistellige Zahlen, getrennt durch Punkte). |
