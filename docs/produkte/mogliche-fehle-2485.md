---
title: "Mögliche Fehlercodes importDossier"
topic_id: "2485"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Erstellen, Aktualisiern und Überschreiben eines Vorgangs > Mögliche Fehlercodes importDossier"
---

# Mögliche Fehlercodes importDossier

| Fehlercode | Fehlertext | Beschreibung |
| --- | --- | --- |
| Server.methodHasNoRequest |  | Sie haben keinen Request übergeben. |
| Server.valueNotfound | dossier | Bitte überprüfen Sie der übergebene Parameter Dossier. Der Wert ist leer oder ungültig. |
| Server.valueNotfound | crud | Bitte überprüfen Sie der übergebene Parameter crud. Der Wert ist leer oder ungültig. |
| Server.valueNotfound | mandatory " + HTTP\_HEADER\_X\_ONBEHALFOF + " for TRANSACTION |  |
| Server.valueNotfound | mandatory field missing or wrong format | Pflichtfeld oder falsches Format |
| Server.valueNotfound | mandatroy field | Pflichtfeld |
| Server.wrongValue | dossierId for CREATE is not empty. | Bitte löschen Sie dossierId beim Importieren eines neues Dossiers |
| Server.wrongValue | dossierId for UPDATE has no value. | Bitte übergeben Sie eine gültige dossierId bei Aktualisieren eines Dossiers. |
| Server.wrongValue | Unknown CRUD Method | CRUD Methode nicht bekannt |
| Server.wrongValue | mandatory " + HTTP\_HEADER\_X\_ONBEHALFOF + " for TRANSACTION |  |
| Server.uniqueParamter | contractName [contractName] must be unique. | Der contractName Parameter muss eindeutig sein. Der ausgewählte contractName ist schon in Verwendung. |
