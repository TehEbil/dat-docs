---
title: "Hinzufügen eines benutzerdefinierten Tags zu einem Auftrag"
topic_id: "25216"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Hinzufügen eines benutzerdefinierten Tags zu einem Auftrag"
---

# Hinzufügen eines benutzerdefinierten Tags zu einem Auftrag

Die SOAP-Funktion setCustomTag ermöglicht es, benutzerdefinierte Tags zu einem Schadenvorgang
(Contract) hinzuzufügen, zu entfernen oder zu ersetzen. Im Kontext einer Webanwendung
zur Schadenkalkulation und -freigabe für Fahrzeuge könnte dies bedeuten, dass Benutzer
bestimmte Tags oder Kennzeichnungen zu einem Schadenvorgang hinzufügen können, um
ihn zu kategorisieren oder zu kennzeichnen.

Abb1. Beispiel Approval Type RKÜ

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | long |  | ID des Vorgabgs | X |
| tagAddRemoveReplaceAction | String | Add    Remove | Add: Weist dem Vorgang einen Tag zu.    Remove: Entfernt den Tag vom Vorgang | X |
| tagIdentification | String |  |  | X |
| networkType | String |  |  | X |

Rückgabe

Zähler, wie viele Rollen im Vorgang erfolgreich dem Tag zugewiesen wurden
