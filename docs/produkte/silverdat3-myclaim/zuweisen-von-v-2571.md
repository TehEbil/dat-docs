---
title: "Zuweisen von Vertragskonditionen"
topic_id: "2571"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Zuweisen von Vertragskonditionen"
---

# Zuweisen von Vertragskonditionen

Diese Funktion weist Vertragskonditionen einem spezifischen Auftrag für einen bestimmten
Partner zu.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | ID des Auftrags | X |
| rolePartner | String | MANUFACTURER, REPAIRER, INSURER, EXPERT | Rolle des Partners | X |
| settlementIdentification | String |  | Identifikationsname der Vertragskondition | X |

Rückgabe

True falls Zuweisung der Vertragskonditionen erfolgreich, andernfalls false
