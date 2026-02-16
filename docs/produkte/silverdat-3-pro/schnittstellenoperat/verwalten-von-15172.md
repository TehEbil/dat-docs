---
title: "Verwalten von Vorgängen"
topic_id: "15172"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen"
---

# Verwalten von Vorgängen

Mit Hilfe der Funktionen des ValuationServiceN verwalten Sie Ihre Bewertungen in der SilverDAT 3 PRO über die Soap Schnittstelle.

Variante mit unvollständiger Fahrzeugidentifikation

Bestimmte Funktionen dieses Services bieten die Möglichkeit Vorgänge zu verarbeiten,
die keine oder nur eine unvollständige Fahrzeugidentifikation beinhalten. Dieser Mode
wird nachfolgend als Variante mit unvollständiger Fahrzeugidentifikation bezeichnet.
Mit dieser Variante besteht die Möglichkeit einen Vorgang anzulegen bevor das Fahrzeug
identifiziert wurde. Dies ermöglicht einer Fremdanwendung den gezielten Aufruf von
SilverDAT 3 PRO über die Oberflächen-Integration mit der Möglichkeit, dass erst der Anwender das
Fahrzeug identifiziert. Diese Variante eignet sich ebenfalls für eine manuelle Korrektur
durch den Anwender. Dies ist dann nötig, falls bei der Fahrzeugidentifikation über
die Schnittstelle etwas nicht funktioniert hat und man deshalb keinen vollständigen
DAT €uropa-Code® erhalten hat.

Um die Variante mit unvollständiger Fahrzeugidentifikation zu aktivieren müssen Sie
im Request das Element Coverage angeben und die Werte NOVALUATIONRESULT oder NONE setzen.

Berechtigung

Die Funktionen der Bewertung werden hinsichtlich der Berechtigung nicht differenziert,
Sie besitzen entweder die Berechtigung für alle Funktionen oder für keine.

Kurzübersicht der Funktionen

| Funktion | Beschreibung | Variante mit unvollständiger Fahrzeugidentifikation |
| --- | --- | --- |
| [createValuationN](erstellen-eine-15178.md) | Erstellen eines neuen Wertmittlungs oder Bewertungsvorgangs in der Anwendung | X |
| [doValuationInMemoryN](erstellen-eine-15176.md) | Erstellen einer Bewertungsvorgangs im Speicher |  |
| [getValuationN](holen-einer-be-15180.md) | Holen eines Bewertungsvorgangs | X |
| [changeValuationN](andern-einer-b-15170.md) | Ändern eines Bewertungsvorgangs | X |
| [resetValuation2defaultN](zurucksetzen-e-15208.md) | Zurücksetzen einer Bewertung auf die DAT Standardeinstellungen |  |

Die spezifischen Schnittstellen-Funktionen der SilverDAT 3 PRO zum Verwalten der Bewertungen und ihre Beschreibungen rufen Sie über folgende URL's
auf:

WSDL

<https://www.dat.de/myClaim/soap/v2/ValuationServiceN?wsdl>

Serviceaufruf

<https://www.dat.de/myClaim/soap/v2/ValuationServiceN>
