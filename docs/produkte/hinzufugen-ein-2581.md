---
title: "Hinzufügen einer Nachricht zu einem Auftrag"
topic_id: "2581"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Hinzufügen einer Nachricht zu einem Auftrag"
---

# Hinzufügen einer Nachricht zu einem Auftrag

Die Funktion addMessage erlaubt es in einem bestehenden Auftrag einen Kommentar hinzuzufügen. Welcher Akteur
innerhalb eines Auftrags die Nachricht erhält, kann mit dem Parameter "recipients" bestimmt werden.

In diesem Parameter vom Typ List können ein oder mehere Benutzerrollenübergeben werden die die Nachricht erhalten sollen.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| claimId | Long |  | ID des Auftrags | x |
| recipients | List<CustomerRole> | INSURANCE, MANUFACTURER, EXPERT, REPAIRER | Rolle des Partners | x |
| message | String |  | Nachricht die dem Auftrag hinzugefügt wird. | x |

Rückgabe

- true: Falls Nachricht hinzugefügt wurde

- false: Falls Nachricht nicht hinzugefügt wurde
