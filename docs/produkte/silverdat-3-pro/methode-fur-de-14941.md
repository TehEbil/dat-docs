---
title: "Methode für den Statuswechsel"
topic_id: "14941"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Status umbuchen > Methode für den Statuswechsel"
---

# Methode für den Statuswechsel

Sie ändern den Status eines Vorgangs mit der Funktion changeContractStatus. Bitte beachten Sie, dass diese Funktion Bestandteil des Service MyClaimExternalService ist (siehe unten). Um den Status zu wechseln, müssen sie den Parameter StatusType setzen.

Wenn Sie Parameterwert Erfasst setzen, dann wird der Dossier Status zu Erfasst gewechselt.

Wenn Sie Parameterwert Disponiert setzen, dann wird der Dossier Status zu Disponiert gewechselt.

Wenn Sie Parameterwert Verkauft setzen, dann wird der Dossier Status zu Verkauft gewechselt

Wenn Sie Parameterwert opened setzen, wird der Dossier Status von Verkauft zu Erfasst umgebucht.

Hinweis: Sie setzen die Ankaufsdaten mit der Funktion setPurchaseData, die Zugangsdaten mit setAdmissionData und die Verkaufsdaten mit setSalesData. Bitte lesen Sie zuerst das Kapitel "Status umbuchen" durch.

Parameter changeContractStatus

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ContractID | Long | Eindeutige Vorgangserkennung (DossierId) | numerisch | x |
| StatusType | String | Der Status wird gesetzt. Bitte beachten Sie, dass man nicht in jeden Status wechseln kann. Siehe Kapitel "Status umbuchen". | Erfasst,  Disponiert,  Bestand,  Verkauft,  opened | x |

WSDL

https://www.dat.de/myClaim/soap/v2/MyClaimExternalService
