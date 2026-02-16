---
title: "Status umbuchen"
topic_id: "12132"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Status umbuchen"
---

# Status umbuchen

Mithilfe der nachfolgend beschriebenen Funktionen verwalten Sie die Daten für die
Maske Ankauf, Zugang und Verkauf in SilverDAT 3 Pro. Diese Funktionen finden Sie unter dem Service TradingServiceN. Weiter unten finden Sie wichtige Informationen zum Umbuchen.

Übersicht der Funktionen

| Funktion | Beschreibung | Service |
| --- | --- | --- |
| setPurchaseData | Daten für den Ankauf anlegen | TradingServiceN |
| setAdmissionData | Daten für den Zugang anlegen | TradingServiceN |
| setSalesData | Daten für den Verkauf anlegen | TradingServiceN |

Status umbuchen

Mit der Methode changeContractStatus ändern Sie den Status des Vorgangs, indem Sie den Parameter StatusType entsprechend setzen. Hierbei ist es wichtig die Reihenfolge einzuhalten, um zum Status
"Verkauft" zu gelangen.

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

| Status Übergang | StatusType | Vorbedingungen |
| --- | --- | --- |
| Erfasst -> Disponiert | Disponiert | Daten für den Ankauf müssen gesetzt sein, entweder manuell oder mit der Funktion setPurchaseData. |
| Disponiert -> Bestand | Bestand | Daten für den Zugang müssen gesetzt sein, entweder manuell oder mit der Funktion setAdmissionData. |
| Bestand -> Verkauft | Verkauft | Daten für den Verkauf müssen gesetzt sein, entweder manuell oder mit der Funktion setSalesData. |
| Verkauft -> Erfasst | opened | Keine Daten müssen gesetzt werden. |

Aufruf der Methoden, um alle Daten und Status vom Ankauf zum Verkauf nach der Reihenfolge
zu setzen (wie in der Oberfläche)

1. Bitte rufen Sie die Funktion createValuationN mit vollständiger Fahrzeugidentifikation auf

2. Mithilfe der Funktion createOrUpdateContactData tragen Sie die Halter- und Käufer-Daten ein. Die Abfrage der Halter- und Käufer-Daten
erfolgt mit der Funktion getPossibleContactPersons .

3. Die möglichen Ansprechpartner fragen Sie mit der Methode getPossibleContactPersons ab. Die Id von getPossibleContactPersonsResponse benötigen Sie für BuyerId oder SellerId.

4. Bitte setzen Sie mit der Funktion setPurchaseData die Ankaufsdaten.

5. Mit der Methode changeContractStatus den Parameter StatusType: Disponiert setzen, somit wird der Status Disponiert für das Dossier gesetzt.

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

6. Bitte setzen Sie mit der Funktion setAdmissionData die Zugangsdaten.

7.Mit der Methode changeContractStatus den Parameter StatusType: Bestand setzen, somit wird der Status Bestand für das Dossier gesetzt.

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

8. Bitte setzen Sie mit der Funktion setSalesData die Verkaufsdaten.

9. Mit der Methode changeContractStatus den Parameter StatusType: Verkauft setzen, somit wird der Status Verkauft für das Dossier gesetzt.

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

optional: 10.Mit der Methode changeContractStatus den Parameter StatusType: opened setzen, somit wird der Status Erfasst für das Dossier gesetzt. Wiederholung ab 4.
möglich.

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

Hinweis: Rückbuchen ist von jedem Status möglich, wenn die Pflichtfelder jeweils passend
zum Status gesetzt sind. Siehe Kapitel "[Daten für den Ankauf anlegen](daten-fur-den-12131.md)", "[Daten für den Zugang anlegen](daten-fur-den-12134.md)" und "[Daten für den Verkauf anlegen](daten-fur-den-12137.md)". Den aktuellen Status können Sie auch mit getValuationN abfragen. Hierfür muss der Parameter Coverage EXTENDEDBYTRADING gesetzt werden.

WSDL

https://www.dat.de/myClaim/soap/v2/TradingServiceN?wsdl

Serviceaufruf

https://www.dat.de/myClaim/soap/v2/TradingServiceN
