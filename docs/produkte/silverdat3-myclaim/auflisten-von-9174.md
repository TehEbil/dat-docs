---
title: "Auflisten von möglichen nachfolgenden Status zu einem Auftrag"
topic_id: "9174"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Auflisten von möglichen nachfolgenden Status zu einem Auftrag"
---

# Auflisten von möglichen nachfolgenden Status zu einem Auftrag

Diese Funktion bietet die Möglichkeit, in einem bestimmten Status eines Auftrags,
eine Liste an möglichen nachfolgenden Status abzufragen.

Bitte beachten Sie, das bei der Rückgabe eines Status mit statusType = custom, in der Funktion changeContract für den Statuswechsel der Wert aus dem Attribut <name> verwendet werden soll.

<PossibleContractStatusTransitions>  
 <description>Auftrag wurde geschlossen</description>  
 <icon>icon-status-ok3</icon>  
 <name>Geschlossen</name>  
 <networkType>OPEN</networkType>  
 <originalName>Geschlossen</originalName>  
 <statusId>5</statusId>  
 <statusType>custom</statusType>  
</PossibleContractStatusTransitions>

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Id eines Auftrags | X |

Rückgabe

Liste aller möglichen nachfolge Status
