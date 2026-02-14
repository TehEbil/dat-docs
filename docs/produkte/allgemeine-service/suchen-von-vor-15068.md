---
title: "Suchen von Vorgängen"
topic_id: "15068"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Suchen von Vorgängen"
---

# Suchen von Vorgängen

Mit der Funktion searchDossierListN finden Sie bestehende Vorgänge.

Übersicht der Funktionalitäten und deren Verfügbarkeit

| Typ | DossierType | SilverDAT 3 valuateFinance | SilverDAT 3 valuateExpert/  PlusPartner | SilverDAT caculatePro |
| --- | --- | --- | --- | --- |
| Bewertung | evaluation | X |  |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | historic evaluation | X |  |  |
| Vergleich | comparison | X |  |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | valuateExpert  valuateExpertPlusPartner |  | X |  |
| Kalkulation | repair |  |  | X |
| Glass-Kalkulation | glass |  |  | X |

Eingabedaten

SearchCriterionList - Suchkriterien, ein oder mehrere Suchbegriffe wie zum Beispiel: KFZ-Kennzeichen LicenseNumber oder Fahrgestellnummer Vin.  
Limit - Gibt die maximale Anzahl von Ergebnissen pro Abfrage an; Wert ist optional, Standardwert
ist 20. Der zulässige Bereich liegt zwischen 1 und 1000.  
Coverage - Datenausgabeumfang. Dieser Wert ist optional, der Standardwert lautet: COMPLETE

Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.

|  |  |
| --- | --- |
| Wert | Datenumfang |
| MARKETPLACEEXPORT | Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO). |
| EXTENDEDBYTRADING | Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO). |
| COMPLETE | Defaultwert; Standard Datenumfang für die Datenrückgabe |
| NOVALUATIONRESULT | Datenrückgabe ohne die Unterelemente Valuation und VAT |
| ENRICHED | Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen |
| BASE | Datenrückgabe ganz ohne Benennungen |
| SIMPLE | Bei diesem Wert entfallen zusätzlich bestimmte Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder, RegistratinData, Engine, Equipment oder TechInfo. |
| NONE | Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. |

Rückgabe

Im Erfolgsfall wird das Suchergebnis in Listenform zurückgegeben, ansonsten wird eine
Fehlermeldung ausgegeben. Die angezeigten Felder des Suchergebnisses orientieren sich
an der Felderliste der Vorgangsübersicht in der Anwendung, die Sortierung kann jedoch
unterschiedlich sein.

Funktionsbeschreibung

Die Suche können Sie mit unterschiedlichen Suchbegriffen durchführen. Wenn Sie das
Suchergebnis weiter eingrenzen möchten, können Sie mehrere Suchbegriffe kombinieren.
Die Suchkriterien wirken immer einschränkend, da diese durch den logischen Operator
UND verknüpft werden. Eine Suche muss mindestens einen der vordefinierten Suchbegriffe
enthalten. Zu einem Suchbegriff kann ein Wert, sowie eine untere und eine oberen Grenze
angegeben werden. Die Grenzwerte sind hierbei immer inklusive. Es existieren grundsätzlich
zwei unterschiedliche Arten von vordefinierten Suchbegriffen:

- Suchbegriffe, die nur konkrete Werte unterstützen.   
  Bei diesen Suchbegriffen wird nur der Wert berücksichtigt und die Angaben für die
  untere und die obere Grenze ignoriert.
- Suchbegriffe, die einen Wertebereich unterstützen.  
  Falls bei diesen Suchbegriffen der Wert angegeben ist, wird nur dieser berücksichtigt
  und die Angaben für die untere und die obere Grenze ignoriert. Falls kein Wert angegeben
  wurde, werden die Grenzwerte verwendet. Sollte die untere Grenze fehlen, dann werden
  alle Einträge bis zur oberen Grenze zurückgegeben. Sollte die obere Grenze fehlen,
  dann werden alle Einträge bis zur unteren Grenze zurückgegeben. Sind die Werte für
  die untere und die obere Grenze identisch, dann wird genau nach diesem Wert gesucht.
  Ist der untere Grenzwert größer als der obere, dann wird kein Ergebnis zurückgeliefert.

Mittels Limit begrenzen Sie die maximale Anzahl der Treffer. Falls Sie keine Vorgabe treffen wird
das Suchergebnis automatisch auf maximal 20 Treffer begrenzt.

Bitte verwenden Sie zur Aufbereitung der Suchbegriffe die Datenstruktur SearchDossierListNRequest. Sie können ein oder mehrere SearchCriterion-Unterelemente verwenden, jedes Unterelement kann bis zu fünf Elemente mit den Suchbegriffen
enthalten. Die Elemente von SearchCriterion sind bis auf useWildcard (Typ Boolean) alle vom Typ String und lauten wie folgt:

- Key - Bezeichnung des Suchbegriffs; erforderlich. Die Liste der möglichen Begriffe
  finden Sie weiter unten.
- Value - Konkreter Wert für die Suche; optional
- UpperLimit - Obere Grenze des Suchbereichs; optional
- LowerLimit - Untere Grenze des Suchbereichs; optional
- useWildcard- Suche mit Platzhalter; optional

Der konkrete Wert ist bei allen Suchbegriffen möglich. Suchbegriffe mit Wertebereich
können die Attribute LowerLimit und UpperLimit enthalten.

Beispiele

Suchbegriff mit konkretem Wert:

```
<SearchCriterion>
    <Key>Name</Key>
    <Value>My Dossier name</Value>
</SearchCriterion>
```

Suchbegriff mit Wertebereich:

```
<SearchCriterion>
     <Key>CreateDate</Key>
     <LowerLimit>2014-11-24</LowerLimit>
     <UpperLimit>2015-03-26</UpperLimit>
</SearchCriterion>
```

Suchbegriff mit Platzhalter:

```
<SearchCriterion>
    <Key>Name</Key>
    <Value>My Dossier*</Value>
    <useWildcard>true</useWildcard>
</SearchCriterion>
```

Übersicht der Suchbegriffe

| Suchbegriff | Datentyp | Art | Beschreibung | Werte / Beispiele | Suche mit Platzhalter möglich |
| --- | --- | --- | --- | --- | --- |
| DossierType | String | konkreter Wert | Nutzungskennzeichen;  Für SilverDAT 3 valuateFinance sind nur die Werte: evaluation, comparison und historic evaluation zulässig, wobei evaluation der Standardwert ist. Für SilverDAT 3 valuateExpert/PlusPartner ist nur valuateExpert beziehungsweise valuateExpertPlusPartner zulässig. Für SilverDAT calculatePro nur repair und glass zulässig. | evaluation = Bewertung  comparison = Vergleich  historic evaluation = Stichtagsbewertung  repair = Schadenskalkulation  glass = Glaskalkulation  valuateExpert = Stichtagsbewertung |  |
| Name | String | konkreter Wert | Bezeichnung des Vorgangs | beliebiger Text | X |
| ExternalId | String | konkreter Wert | Identifikation im Fremdsystem | beliebiger Text | X |
| CreateDate | Date | Bereich | Erstellungsdatum | 2014-11-24 |  |
| ChangeDate | Date | Bereich | Datum der letzten Änderung | 2015-03-26 |  |
| CreateUser | String | konkreter Wert | Benutzer, der den Vorgang erstellt hat | username |  |
| ChangeUser | String | konkreter Wert | Benutzer der letzten Änderung | otheruser |  |
| Country | String | konkreter Wert | Länderkennzeichen der Daten (ISO 3166 ALPHA-2) | DE |  |
| LicenseNumber | String | konkreter Wert | KFZ-Kennzeichen | S DAT 123 | X |
| Vin | String | konkreter Wert | Fahrzeugidentifikationsnummer (Fahrgestellnr.) | WDD2040071Axxxxxx | X |
| VehicleType | Integer | konkreter Wert | Fahrzeugart | 1 |  |
| Manufacturer | Integer | konkreter Wert | Hersteller-Schlüssel | 905 |  |
| MainModel | Integer | konkreter Wert | Haupttyp | 3 |  |
| SubModel | Integer | konkreter Wert | Untertyp | 2 |  |
| SubModelVariant | Integer | konkreter Wert | Untertypvariante | 43 |  |
| Container | String | konkreter Wert | Teil des Marktindex, zum DAT-€uropa-Code | DE00L |  |
| ConstructionTime | Integer | konkreter Wert | Bauzeit in DAT-Verschlüsselung | 4423 |  |
| InitialRegistration | Date | Bereich | Erstzulassungsdatum | 2006-10-10 |  |
| MileageEstimated | Integer | Bereich | Km-Stand geschätzt | 165000 |  |
| DeterminatedDate | Date | Bereich | Bewertungs-Stichtag (nur bei Stichtagsbewertungen) | 2015-01-02 |  |
| SalesPrice | Decimal | Bereich | Händler-Verkaufspreis netto (inkl. Ausstattungen) | 5620 |  |
| SalesPriceGross | Decimal | Bereich | Händler-Verkaufspreis brutto (inkl. Ausstattungen) | 5847 |  |
| orderNumber | String | konkreter Wert | Auftragsnummer | beliebiger Text | X |
| contractNumber | String | konkreter Wert | Vertragsnummer | beliebiger Text | X |
