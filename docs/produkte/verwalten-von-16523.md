---
title: "Verwalten von unvollstaendigen Aktenzeichen"
topic_id: "16523"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Unvollständiges Aktenzeichen > Verwalten von unvollstaendigen Aktenzeichen"
---

# Verwalten von unvollstaendigen Aktenzeichen

Das unvollständige Aktenzeichen ermöglicht es Ihnen Vorgänge über die DAT Schnittstellen
anzulegen, die keine oder nur eine unvollständige Fahrzeugidentifikation beinhalten.
Mit dieser Variante besteht die Möglichkeit einen Vorgang anzulegen bevor das Fahrzeug
identifiziert wurde. Dies ermöglicht einer Fremdanwendung den gezielten Aufruf von
SilverDAT 3 valuateExpert/PlusPartner über die Oberflächen-Integration mit der Möglichkeit, dass erst der Anwender das
Fahrzeug identifiziert. Diese Variante eignet sich ebenfalls für eine manuelle Korrektur
durch den Anwender. Dies ist dann nötig, falls bei der Fahrzeugidentifikation über
die Schnittstelle etwas nicht funktioniert hat und man deshalb keinen vollständigen
DAT €uropa-Code® erhalten hat.

Um das unvollständige Aktenzeichen zu nutzen müssen Sie im Request das Element Coverage angeben und den Wert NOVALUATIONRESULT oder NONE setzen.
