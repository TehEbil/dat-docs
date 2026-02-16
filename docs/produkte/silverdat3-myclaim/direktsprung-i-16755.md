---
title: "Direktsprung in einem bestimmten Bereich innerhalb eines Vorgangs"
topic_id: "16755"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Direktsprung in einem bestimmten Bereich innerhalb eines Vorgangs"
---

# Direktsprung in einem bestimmten Bereich innerhalb eines Vorgangs

Um in der SilverDat 3 einen Vorgang in einem bestimmten Reiter zu öffnen, gibt es die Möglichkeit am Ende
der URL den Namen des bestimmten Reiters bzw. Tabs zu übergeben.

Mit dieser Methode wird der Benutzer direkt in den gewünschten Bereich des Vorgangs
navigiert.

Diese Funktion ist im Moment ausschließlich nur in der SilverDAT 3 verfügbar

Zur Auswahl stehen:

|  |  |
| --- | --- |
| Tab Register | Tab ID (tabId) |
| Auftragsübersicht (Order opening) | tab-contractOpening |
| Fahrzeugauswahl (Vehicle selection) | tab-vehicleSelection |
| Austattung (Equipment) | tab-equipmentSelection |
| Vorgangsbezogene Daten (Procedure-related data) | tab-activityRelatedData |
| Teileauswahl (Parts selection) | tab-graphicalPartSelection |
| Kalkulation (Calculaction) | tab-calculationResult |
| Rechnung (Invoice) | tab-invoice |

Beispiel:

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=vro\_calculation&tabId=TAB\_HERE

Aufruf der Bewertung

Um einen Vorgang in der SilverDAT 3 direkt im Bewertungsvorgang öffnen zu können, werden die folgende Parameter in der
URL zur Übergabe benötigt.

1. fabrikat: Das Netz in dem der Vorgang sich befindet (Optional)- ist identisch mit dem networkType
2. token: Authentifizierungstoken (Wie Sie einen Token generieren entnehmen Sie bitte im Kapitel
   [JSON Web Token Authentication](../../allgemein/dat-developers-guide/authentifizierung-de/json-web-token-14087.md)
3. claim: Die ID des zu öffnenden Vorgangs
4. subView: Der Bewertungsprozess über der jeweiligen Maske.
5. subViewMode: Die Hauptmaske des jeweiligen Bewertungsprozesses.
6. tabId: Die Id der zu öffnenden Maske.

In den folgenden Tabellen werden für alle Prozesse und alle Masken der Bewertung die
jeweiligen Elementen (subView / subViewMode / tabId) zur Übergabe der URL aufgelistet.

Direkteinsprung in den Vorgang:

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=bundle\_landing\_page

Zur Auswahl stehen:

|  |  |
| --- | --- |
| Tab Register | Tab ID (tabId) |
| Direkteinsprung in den Vorgang | subView=bundle\_landing\_page |

1. Prozess für die Bewertung - Wertermittlung

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=bundle\_valuation&tabId=TAB\_HERE

Zur Auswahl stehen:

|  |  |
| --- | --- |
| Tab Register | Tab ID (tabId) |
| Wertermittlung | subView=bundle\_valuation |
| Fahrzeugauswahl | tab-GS\_VEHICLE\_SELECTION |
| Ausstattungen | noch nicht verfügbar |
| Kunde | tab-contractOpening |
| Zustand | tab-FirstValuationConditionPage |
| Wertermittlung | tab-FirstValuationValuationPage |
| webScan | tab-WEB\_SCAN |
| Kalkulation | tab-CALCULATION |
| Fahrzeugdaten | tab-FirstValuationVehicleDataFromValPage |
| Instandsetzungskosten | tab-RepairParametersPage |

2. Prozess für die Bewertung - Ankauf

2.1 Ankaufsangebot

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=bundle\_valuation&subViewMode=PURCHASE\_OFFER&tabId=TAB\_HERE

Zur Auswahl stehen:

|  |  |
| --- | --- |
| Tab Register | Tab ID (tabId) |
| Kunde | subView=bundle\_purchase&subViewMode=PURCHASE\_OFFER |
| Kunde | tab-contractOpening |
| Daten | tab-PURCHASE\_DATAEDITOR |

2.2 Ankauf

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=bundle\_purchase&subViewMode=PURCHASE&tabId=TAB\_HERE

Zur Auswahl stehen:

|  |  |
| --- | --- |
| Tab Register | Tab ID (tabId) |
| Ankauf | subView=bundle\_purchase&subViewMode=PURCHASE |
| Kunde | tab-contractOpening |
| Kalkulation | tab-CALCULATION |
| webScan | tab-WEB\_SCAN |
| Daten | tab-PURCHASE\_DATAEDITOR |

2.3 Zugang

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=bundle\_purchase&subViewMode=ADMISSION&tabId=TAB\_HERE

Zur Auswahl stehen:

|  |  |
| --- | --- |
| Tab Register | Tab ID (tabId) |
| Zugang | subView=bundle\_purchase&subViewMode=ADMISSION |
| Kunde | tab-contractOpening |
| Kalkulation | tab-CALCULATION |
| webScan | tab-WEB\_SCAN |

3. Prozess für die Bewertung - Verkauf

3.1 Börsenaufbereitung

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=bundle\_sales&subViewMode=SALES\_PREPARATION&tabId=TAB\_HERE

Zur Auswahl stehen:

|  |  |
| --- | --- |
| Tab Register | Tab ID (tabId) |
| Börsenaufbereitung | subView=bundle\_sales&subViewMode=SALES\_PREPARATION |
| Steuerung | tab-equipmentForMarketplacesPage |
| Allgemein | tab-SALES\_PREPARATION\_GENERAL |
| Ausstattungen | tab-SALESPREPARATION\_EQUIPMENT |
| Fahrzeugdaten | tab-SALESPREPARATION\_PROPERTIES |
| Bilder | tab-SALESPREPARATION\_PICTURES |
| Bank | tab-SALESPREPARATION\_BANK |
| Vorschau Dekoration | tab-SALESPREPARATION\_DECORATIONPREVIEW |
| Daten Preisschild | tab-PRICETAG\_DATAEDITOR |

3.2 Verkaufsangebot

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=bundle\_sales&subViewMode=SALES\_OFFER&tabId=TAB\_HERE

Zur Auswahl stehen:

|  |  |
| --- | --- |
| Tab Register | Tab ID (tabId) |
| Verkaufsangebot | subView=bundle\_sales&subViewMode=SALES\_OFFER |
| Kunde | tab-contractOpening |
| Kalkulation | tab-CALCULATION |
| Bank | tab-SALESPREPARATION\_BANK |
| Daten | tab-SALES\_DATAEDITOR |

3.3 Reservierung

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=bundle\_sales&subViewMode=RESERVATION&tabId=TAB\_HERE

Zur Auswahl stehen:

|  |  |
| --- | --- |
| Tab Register | Tab ID (tabId) |
| Reservierung | subView=bundle\_sales&subViewMode=RESERVATION |
| Kunde | tab-contractOpening |

3.4 Verkauf

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=bundle\_sales&subViewMode=SALES&tabId=TAB\_HERE

Zur Auswahl stehen:

|  |  |
| --- | --- |
| Tab Register | Tab ID (tabId) |
| Verkauf | subView=bundle\_sales&subViewMode=SALES |
| Kunde | tab-contractOpening |
| Kalkulation | tab-CALCULATION |
| Garantie | tab-WARRANTY |
| Daten | tab-SALES\_DATAEDITOR |
