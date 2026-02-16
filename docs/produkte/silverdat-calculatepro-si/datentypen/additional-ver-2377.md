---
title: "ADDITIONAL (Veraltet!)"
topic_id: "2377"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Datentypen > datProcessInfo und DVNInfo (Veraltet!) > ADDITIONAL (Veraltet!)"
---

# ADDITIONAL (Veraltet!)

##### DENTS (Veraltet!)

Die Methode "DENTS" führt eine Hagelschadenkalkulation durch.

Die Schnittstelle ist sehr ähnlich zum Hagelschadendialog aufgebaut. Grundsätzlich
gibt es drei sich gegenseitig ausschließenden Berechnungsmodi, dem „Drücken“, dem
„Erneuern“ und dem „Vordrücken und Lackieren“ (BVAT) oder Vorziehen und Lackieren (Deutsche Kommission für Lack und Karosserieinstandsssetzung)

Der Berechnungsmodus wird über den Parameter „calculationMode“ gesteuert. Die Bedeutung der verschieden Modi wird im Folgenden näher erklärt.

Für Hagelschäden werden spezielle Reparaturprozesse verwendet, mit deren Hilfe ist
es möglich die zusätzlichen Felder der Methode „Drücken" und „Vordrücken und Lackieren"
oder "Vorziehen und Lackieren" zu setzen. Als Methode <method/> muss bei Hagelschäden immer „DENTS“ angegeben werden. Fehlt die Methode, dann wird der Standardreparaturprozess „GRAPHICAL“ genutzt und hagelspezifische Informationen nicht berücksichtigt was zu massive Abweichungen
beim Ergebnis führt.

Die Eingabefelder sind über einen hagelschadenspezifischen Reparaturprozess vorbelegbar.
Dementsprechend muss als Methode immer „DENTS“ angegeben werden. Fehlt die Methode dann wird „GRAPHICAL“ angenommen, welche hagelspezifische Informationen ignoriert und auf andere Stundensätze
zurückgreift. Dadurch treten erhebliche Abweichungen beim Ergebnis auf.

Bei Hagelprozessen die aus mehreren Reparaturprozessen bestehen (z.B. I und L sowie E) muss der calculationMode für eine DVN konsistent sein.

Es können zeitgleich die Eigenschaften/Felder für „Hagelschaden drücken" und „Vordrücken
und Lackieren" oder "Vorziehen und Lackieren" gesetzt werden, die entsprechenden Eigenschaften/Felder
sind kollisionsfrei. Die Berechnung wählt anhand des calculationMode und die zugehörigen Felder aus.

Hagelschaden Drücken

Dieser Modus (calculationMode=1) entspricht dem Berechnungsmodus "Drücken" je nach Auswahl der Hagelschadenmethode
BVAT oder Deutsche Kommission für Lack und Karosserieinstandsssetzung.

Das Prozess wird über einen „I“ und einen „L“ mit Lackstufe 0 für lackschadenfreie Hagelpositionen abgebildet.

Die Typ (1) Eigenschaft definiert das Berechnungsmodelle z. B. „BVAT“.

|  |  |
| --- | --- |
| Type | Bedeutung |
| GERMAN\_COMMISION | Deutsche Kommission für Lack und Karosserieinstandsetzung |
| BVAT | Hagelschaden-Zentrum (Bundesverband Ausbeultechnik, BVAT) |

Im Screenshot ist der Dialog für BVAT dargestellt, und wird im Folgenden näher erklärt.

Aus der „Anzahl der Dellen" (2), der „Bauteillage" (3) und der „Dellengröße" (4) wird
die "Vorgabe-Zeit" (12) gemäß BVAT vorgaben errechnet. Wird bei der "Arbeitszeit (ohne Zuschläge)" (11) eine Zeit manuell
angegeben so wird immer die manuelle Zeit bevorzugt. Die "Zeit Vordrücken (mit Zuschlägen)"
wird nicht mehr berücksichtigt. Ist ein Pauschalwert gewünscht, so muss die Auswahl
"Lohnkosten pauschal" im Dropdown-Menü "Zeitangabe/Pauschale" (10) angegeben werden.
Die Arbeitszeit wird somit ignoriert.

Die Felder (5) – (9) steuern die Zuschläge.

|  |  |  |
| --- | --- | --- |
| Feld in der Oberfläche | Property des RepairProcess | Wertebereich |
| Typ (1) | <type/> | String  [BVAT | GERMAN\_COMMISION] |
| Anzahl der Dellen (2) | <dentsCount/> | Integer |
| Bauteillage (3) | <partPosition/> | String  [S | W bei BVAT] |
| Dellengröße (4) | <dentsSize/> | Integer |
| Zuschlag LM-Teil (5) | <isAdditionLM/> | Boolean [true | false] |
| Zuschlag Klebetechnik 30% (6) | <adhesiveMethod> | Boolean [true | false] |
| Rüstzeit einmalig (8) | <isSetupTime/> | Boolean [true | false] |
| Finisharbeit pro Bauteil (9) | <isFinishing/> | Boolean [true | false] |
| Arbeitszeit (ohne Zuschläge) (11) | <time/> | Decimal |
| Pauschale (EUR) (10) | <price/> | Float |

Bitte beachten Sie, dass ein Aufsummieren der einzelnen Arbeitszeit-Eingaben der Hagelpositionen
falsch wäre.

Beispiel: Eine Hagelposition nach dem Berechnungsmodus "Dellen-Drücken" als alleinige
Position mit 10 Dellen dauert nach der deutschen Kommission bspw. 2,9 Stunden, eine zweite Hagelposition mit 15 Dellen dauert vielleicht 3,5 Stunden.

Die einzelnen Angaben betragen 2,9 Std. und 3,5 Std. (time). Die gesamte Arbeitszeit fürs Dellen drücken wird wahrscheinlich eher 4,5 Std. (geschätzt) nicht 6,4 Std. (2,9 + 3,5 = 6,4) betragen.

Dies liegt daran, dass die Vorbereitungszeiten oder vergleichbares bereits mit eingerechnet
sind, was dazu führen kann, dass sich der Aufwand pro Delle reduziert.

Hagelschaden Vordrücken / Vorziehen und Lackieren

Dieser Modus (calculationMode=3) entspricht dem Berechnungsmodus Vordrücken / Vorziehen und Lackieren.

Dellen werden hier über den Parameter „I“ ausgesteuert. Aus der „Angabe der Dellen" <dentsSize> wird eine Zeit berechnet. Die Berechnete Zeit kann im Feld „Arbeitszeit vordrücken"
überschrieben werden <time/>.

Die Lackberechnung wird über den Reparatur Prozess „L“ vorgegeben und steuert die Lackstufe (1) (<lacquerLevel>). Der „L“ Prozess muss in diesem Modus für eine Berechnung immer existieren, kennt außer der
Lackstufe jedoch keine anderen Parameter.

Erneuern

In diesem Modus (calculationMode=2) wird ein Komplettaustausch mit dem ReparaturCode „E“ berechnet. Die Lackstufe wird über den „L“ Prozess definiert.

Auch hier sollte als Methode „DENTS“ spezifiziert werden. Der ReparaturCode „E“ in Kombination mit „DENTS“ verfügt über die gleichen Parameter wie ein „I“ mit der Methode „DENTS“. Dadurch wird es möglich im Dialog „Erneuern" vorzuselektieren, und gleichzeitig
die Felder von „Drücken" sowie „Vordrücken / Vorziehen und Lackieren" vorbelegen.
Diese zusätzlichen Informationen werden gespeichert aber nicht bei der Berechnung
berücksichtigt.

Als alternative Berechnung kann auch mit einem normalen „E“ verwendet werden, hier gehen jedoch beim Umschalten des calculationMode die Delleninformationen verloren.

Weitere Teile

Die Oberfläche bietet die Möglichkeit Hagelschäden für Teile die dem DAT System unbekannt
sind (ohne eine passende DVN) zu erfassen. Diese Funktion wird in der über „manuelle Position" definiert.

Da weder für ein solches Teil weder die Ersatzeilkosten noch die Lackierzeiten im
DAT System hinterlegt sind, ist nur die Methode „Drücken" also calculationMode="1" gültig.

Von der Schnittstelle gesehen verhält sich ein solches Teil wie fast identisch wie
im Falle „Hagelschaden drücken".

Der Reparaturprozess ist ein „I“ mit der Methode „DENTS“, die DVN ist in diesem Fall „0" und manual ist auf „true“ gesetzt.

Länder Spezifische Abweichungen.

Für Österreich und die Schweiz sind zusätzliche Informationen für einen „I“ Prozess notwendig. In Österreich kommen sogenannte Dellengruppen zum Einsatz.

|  |  |
| --- | --- |
| Austria |  |
| numDents20 |  |
| numDents30 |  |
| numDents45 |  |
| workTime20 |  |
| workTime30 |  |
| workTime45 |  |
| hasAluminium |  |
| Switzerland |  |
| Worktime |  |
| DentsNumbeLess |  |
| DentsNumberMore |  |
| AdditionalLM |  |
| WorkCompleted |  |
| SetupTime |  |
| BlockWageFlatPrice |  |
| AlloyLM |  |
| LargeScale |  |
| AdhesiveTechnologyScale |  |
