---
title: "Entfernen einer Partnerzuweisung aus einem Auftrag"
topic_id: "2599"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Zuweisen von Benutzern und Partnern zu einem Auftrag > Entfernen einer Partnerzuweisung aus einem Auftrag"
---

# Entfernen einer Partnerzuweisung aus einem Auftrag

Die Funktion unAssignPartnerFromContract entfernt die Zuweisung eines Partners innerhalb eines Auftrags.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Identifizierungsnummer des Auftrags | x |
| rolePartner | String | REPAIRER, INSURANCE, EXPERT, MANUFACTURER | Rolle des Partners dessen Zuweisung entfernt werden soll | x |

Rückgabe

- true: Falls Entfernen der Zuweisung erfolgreich

- false: Falls Entfernen der Zuweisung nicht erfolgreich
