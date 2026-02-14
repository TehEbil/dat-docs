---
title: "Zuweisen eines Benutzers"
topic_id: "2702"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Zuweisen von Benutzern und Partnern zu einem Auftrag > Zuweisen eines Benutzers"
---

# Zuweisen eines Benutzers

Die Funktion assignUsersToContract weist einen oder mehrere Benutzer einem Auftrag hinzu.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Identifizierungsnummer des Auftrags | X |
| userLogins | String[] |  | Benutzer Loginname | X |

Rückgabe

Login Informationen der gerade zugewiesenen Benutzer (ID, Name, Vorname, Loginname)
