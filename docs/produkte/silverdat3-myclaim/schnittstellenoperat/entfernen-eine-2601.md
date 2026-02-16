---
title: "Entfernen einer Benutzerzuweisung aus einem Auftrag"
topic_id: "2601"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Zuweisen von Benutzern und Partnern zu einem Auftrag > Entfernen einer Benutzerzuweisung aus einem Auftrag"
---

# Entfernen einer Benutzerzuweisung aus einem Auftrag

Die Funktion unAssignUserFromContract entfernt die Zuweisung eines Benutzers innerhalb eines Auftrags.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Identifizierungsnummer des Auftrags | x |
| userLogins | String[] | user1, user2.... | Loginnamen der Benutzer die dessen Zuweisung entfernt werden soll | x |

Rückgabe

Login Informationen der Benutzer von denen die Zuweisung aus dem Auftrag entzogen
wurde (ID, Name, Vorname, Loginname)
