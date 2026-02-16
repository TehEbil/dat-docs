---
title: "Abrufen eines Auftrags"
topic_id: "1471"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Abrufen eines Auftrags"
---

# Abrufen eines Auftrags

Funktion getContract die anhand der übergebenden Auftrags ID es ermöglicht (Auftrags ID kann über [findContract](finden-eines-a-1473.md) ermittelt werden) einen kompletten Auftrag mit allen Details wie z.B. das Dossier, teilnehmende Partner, Auftragsstatus usw. abzurufen.

Bitte beachten Sie, das Sie mit getContract keine Bewertungen abrufen können. Bewertungsvorgänge
können über die Funktion [getValuation](../../silverdat-3-pro/schnittstellenoperat/holen-einer-be-15180.md) abgeholt werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | ID des Auftrags | X |

Rückgabe

Alle Details eines Auftrags (Dossier, teilnehmende Partner, Auftragsstatus usw.)
