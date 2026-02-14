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
| [createValuationN](#showid/15178 "Erstellen einer neuen Bewertung in der Anwendung") | Erstellen eines neuen Wertmittlungs oder Bewertungsvorgangs in der Anwendung | X |
| [doValuationInMemoryN](#showid/15176 "Erstellen einer Bewertung im Speicher") | Erstellen einer Bewertungsvorgangs im Speicher |  |
| [getValuationN](#showid/15180 "Holen einer Bewertung") | Holen eines Bewertungsvorgangs | X |
| [changeValuationN](#showid/15170 "Ändern einer Bewertung") | Ändern eines Bewertungsvorgangs | X |
| [resetValuation2defaultN](#showid/15208 "Zurücksetzen einer Bewertung auf die DAT Standardeinstellungen") | Zurücksetzen einer Bewertung auf die DAT Standardeinstellungen |  |

Die spezifischen Schnittstellen-Funktionen der SilverDAT 3 PRO zum Verwalten der Bewertungen und ihre Beschreibungen rufen Sie über folgende URL's
auf:

WSDL

<https://www.dat.de/myClaim/soap/v2/ValuationServiceN?wsdl>

Serviceaufruf

<https://www.dat.de/myClaim/soap/v2/ValuationServiceN>
