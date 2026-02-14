---
title: "datProcessInfo - Kindelement"
topic_id: "6706"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Datentypen > datProcessInfo - Kindelement"
---

# datProcessInfo - Kindelement

| Name/Elternelement | Kindelement | Beschreibung | Mögliche Werte | Datentyp |
| --- | --- | --- | --- | --- |
| datProcessInfo |  | Definiert den Reparaturprozess mit den folgenden Attributen: |  | datProcessInfo |
|  | method | Attribut; für Wartung oder Hagelschaden. | [GRAPHICAL](#expandblock-6706-d2e191635)  Hierüber ist die graphische Teileauswahl nachgebildet.  "repairCode" Attribut  Das repairCode Attribut ist ähnlich einer Arbeitsanweisung. Je DVN Objekt kann immer nur ein repairCode definiert werden. Sind für ein Bauteil mehrere Reparaturanweisungen notwendig, so legt man für jeden Typ ein eigenes DVN Objekt an. Es ist somit kein Fehler, wenn mehrere DVN Objekte die gleiche datProcessId haben aber unterschiedliche repairCodes definieren.    Es existieren die folgenden repairCodes. Ihre Bedeutung ist analog zu der der graphischen Teileauswahl. Ist kein oder ein ungültiger repairCode angegeben so wird "REPLACE (E)" als Fallback genutzt.  |  |  |  | | --- | --- | --- | | REPAIRCODE | Kürzel | Bedeutung | | DIS\_MOUNTING | A | Aus- und Einbau | | UNDERBODY\_PROTECTION | B | Unterbodenschutz | | SPOT\_REPAIR | C | Spot Repair Lackierung | | DISASSEMBLY | D | Zerlegen | | REPLACE (default) | E | Ersetzen (default wenn kein Typ definiert wurde) | | ASSEMBLY | F | Montieren | | CUTTING | G | Schneiden | | DEAREATE | H | Entlüften | | OVERHAUL | I | Instandsetzen (mit Lack) | | CLEANING | J | Reinigen | | FIXING | / | Instandsetzen (ohne Lack) | | CAR\_BODY | K | abzugsfähige Kosten bei Rohbaukarosse | | LACQUER | L | Lackieren | | LACQUER\_DISMOUNTED | M | Montageteil demontiert lackieren | | ADDITIONAL\_COSTS | N | Nebenkosten | | BODY\_CAVITY\_PROTECTION | O | Hohlraumschutz | | VISUAL\_INSPECTION | P | Sichtprüfung (bzw. Polieren, wenn bei Karosserieteilen angegeben) | | REPLACE\_NO\_MATERIAL | Q | Ersetzen oder Erneuern - wie "E", aber nur Arbeitszeitberechnung, keine Materialkosten | | RISK | R | Risiko | | ADJUST | S | Einstellen | | TECHNICAL\_INSPECTION | T | technische Prüfung | | LACQUER\_NO\_AUTOMATICS | U | Lackieren ohne Lackierautomatik (nur bei der Typenhefterfassung - entspricht dem rot unterlegten "L" im Typenheft- wird intern vor der Kalkulation in "L" umgesetzt) | | MEASURING | V | Vermessen | | BALANCING | W | Wuchten | | EXPOSE | X | Freilegen (nur Arbeitslogik) | | COMPLETE | Y | Komplettieren (nur Arbeitslogik) | | DIS\_REASSEMBLE | Z | Zerlegen und Zusammenbauen |  Attribute  Der RepairCode definiert den Typ des DVNInfo Objektes und somit seine Attribute. Welche Attribute für welchen Typen gültig sind ist in der untenstehenden Tabelle dargestellt. Wird ein vom repairCode nicht unterstütztes Attribut gesetzt, so wird es stillschweigend ignoriert.  Attribute sind bis auf wenige Ausnahmen optional. Wird ein Attribut weggelassen, so wird ein Standardwert angenommen.  |  |  |  |  | | --- | --- | --- | --- | | Attribut | Kürzel | Bedeutung | Wertebereich | | price | E |  | Decimal | | isUsedPart | E |  | Boolean [true, false] | | difficultyAllowance | E, A |  | Decimal | | time | E, I, A, L, M, B, D, F, G, H, J, O, P, Q, S, T, U, V, W, X, Y, Z, /, N |  | Decimal [0-999999] | | lacquerLevel | E, I, / |  | Integer | | lacquerPercentage | E, I, L, M |  | Decimal | | noScratchTime | E, I |  | Integer | | discount | E, L, M, R |  | Decimal | | workLevel | E, I, A, / |  | Integer | | workType | E, I, A, / |  | Integer | | optimization | E, I, A, R, / |  |  | | preDamage | E, I, A, L, M, R, C, / | Teil hat einen Vorschaden | Boolean [true, false] | | location | I | Ortsangabe des Schadens  1 = vorn  2 = hinten  3 = oben  4 = unten  5 = mittig | Integer [1-5] | | countyLevelS | / |  |  | | countryLevelM | / |  |  | | coutnryLevelL | / |  |  | | price | /, N |  |  | | repairType | / |  |  | | countryLevelGlass | / |  |  | | amount | C, E, I, L, M, / | Anzahl der betroffenen Teile | Integer | | length | E, I, L, M, / | Die Länge des Ersatzteils bzw. des zu bearbeitenden Teils | Decimal | | width | E, I, L, M, / | Die Breite des Ersatzteils bzw. des zu bearbeitenden Teils. Zierleisten oder ähnliches die in Laufenden Metern abgerechnet werden, verfügen nur über eine Länge und keine Breite. | Decimal | | unit | E, I, L, M, / | Einheit, z.B. QM oder LFM ergibt sich aus der Fläche bzw der Länge des Bauteils. | String |  [MAINTENANCE](#expandblock-6706-d2e191639)  Definiert Materialkosten bei der Wartungskalkulation. Die Wartungskalkulation ist durch das type Attribut verfeinert. Es gibt die folgenden Typen:  |  |  | | --- | --- | | TYPE | Bedeutung | | LABOUR (default) | Arbeitsposition | | MATERIAL | Materialposition | | INTERVAL | Wartungsintervall |  Attribute  |  |  |  |  | | --- | --- | --- | --- | | Attribute | Typ | Bedeutung | Wert | | amount | Material |  | Decimal | | price | Material |  | Decimal |  Beispiel für Material der Wartungskalkulation   ``` <!-- Maintenance --> <datProcessInfo method="MAINTENANCE" type="INTERVAL"> <datProcessId>94030</datProcessId> </datProcessInfo>  <!-- Zahnriemen der Motorsteuerung austauschen --> <datProcessInfo method="MAINTENANCE" type="LABOUR"> <datProcessId>81715</datProcessId> </datProcessInfo>  <!-- REP.-SATZ ZAHNRIEMEN --> <datProcessInfo method="MAINTENANCE" type="MATERIAL"> <datProcessId>81715</datProcessId> <amount>2</amount> <price>130.90</price> </datProcessInfo> ```  [DENTS](additional-ver-2377.md)  [MANUAL](#expandblock-6706-d2e191647)  |  |  |  | | --- | --- | --- | | Attribute | Bedeutung | Wert | | price |  |  | | time |  |  | | amount |  |  | | laquerlevel |  |  | | processName |  |  | | partNumber |  |  | | WorkPositionNumber |  |  | | optimization |  |  | | preDamage | Teil hat einen Vorschaden. | Boolean [true | false] |  [ADDITIONAL](#expandblock-6706-d2e191650)  |  |  |  | | --- | --- | --- | | Attribute | Bedeutung | Wert | | price |  |  | | time |  |  | | amount |  |  | | processName |  |  | | domusPart |  |  | | String, optional |
|  | type | Attribut; nur relevant für Wartungs- oder Hagelschadenberechnung | INTERVAL  LABOUR  MATERIAL | String, optional |
|  |  |  |  |  |
|  | additionLM |  | true/false | Boolean, optional |
|  | adhesiveMethod |  | true/false | Boolean, optional |
|  | adhesiveTechnologyScale |  | true/false | Boolean, optional |
|  | alloyLM |  | true/false | Boolean, optional |
|  | amount | Nur relevant für das Material der Wartungssberechnung |  | Decimal, optional |
|  | blockWageFlatPrice |  |  | Decimal, optional |
|  | bulgeArea |  |  | Integer, optional |
|  | bulgeAreaDifficultyFactor |  |  | Integer, optional |
|  | calculationMode |  |  | Integer,optional  calculationMode: „3" für Vordrücken/-ziehen  calculationMode: „1" für Drücken |
|  | control |  |  | String, optional |
|  | countLevelGlass |  |  | Integer, optional |
|  | countLevelL |  |  | Integer,optional |
|  | countLevelM |  |  | Integer,optional |
|  | countLevelS |  |  | Integer, optional |
|  | DMSFlag |  |  | String, optional |
|  | dentNumberLess |  |  | Decimal, optional |
|  | dentNumberMore |  |  | Decimal, optional |
|  | dentsCount | Anzahl Dellen |  | Integer, optional |
|  | dentsSize | Dellengröße (mm) |  | Integer, optional |
|  | difficultyAllowance | Erschwerniszuchlag |  | Decimal, optional |
|  | discount | Rabatt |  | Decimal, optional |
|  | domusPart |  | true/false | Boolean, optional |
|  | datProcessId | DVN |  | Long, pflicht |
|  | finishType |  |  | String, optional |
|  | grupoPlastico |  |  | String, optional |
|  | hasAluminium |  |  | Integer, optional |
|  | inputL |  |  | Decimal, optional |
|  | inputLP |  |  | Decimal, optional |
|  | inputSDE |  |  | Decimal, optional |
|  | inputSDI |  |  | Decimal, optional |
|  | inputSPD |  |  | Decimal, optional |
|  | isAdditionLM | Zuschlag LM-Teil | true/false | Boolean, optional |
|  | isFinishing | Finishing | true/false | Boolean, optional |
|  | isSetupTime | Rüstzeit einmalig | true/false | Boolean, optional |
|  | isUsedPart | Gebrauchtteil | true/false | Boolean, optional |
|  | lacquerLevel | Lackstufe |  | Integer, optional |
|  | lacquerPercentage |  |  | Decimal, optional |
|  | laquerDifficulty |  |  | Integer, optional |
|  | largeScale |  | true/false | Boolean, optional |
|  | length |  |  | Decimal, optional |
|  | location | Ortsangabe vom Schaden am Fahrzeug |  | Integer, optional |
|  | manual |  | true/false | Boolean, optional |
|  | noScratchTime |  |  | Decimal, optional |
|  | numDents20 |  |  | Integer, optional |
|  | numDents30 |  |  | Integer, optional |
|  | numDents45 |  |  | Integer, optional |
|  | optimization |  |  | Integer, optional |
|  | partNumber |  |  | String, optional |
|  | partPosition | Bauteillage | "senkrecht" | "waagrecht" | String, optional |
|  | piezasOP |  |  | String, optional |
|  | piezasPO |  |  | String, optional |
|  | preDamage | Vorschaden | true/false | Boolean, optional |
|  | prePressTime | Arbeitszeit Vordrücken |  | Decimal, optional |
|  | price | Pauschale, nur relevant für das Material der Wartungssberechnung |  | Decimal, optional |
|  | processName |  |  | String, optional |
|  | repairCode | Nur relevant für das Material der Wartungssberechnung |  | String, optional |
|  | repairType |  |  | String, optional |
|  | setupTime |  |  | Integer, optional |
|  | suppressed | Die datProcessIds, die mit dem Element <suppressed>true</suppressed> werden bei der Berechnungszeit ausgelassen. | true/false | Boolean, optional |
|  | time | Arbeitszeit (STD) |  | Decimal, optional |
|  | unit |  |  | String, optional |
|  | wearAdditional |  |  | Decimal, optional |
|  | wearAge |  |  | Integer, optional |
|  | wearGroup |  |  | String, optional |
|  | wearMileage |  |  | Integer, optional |
|  | width |  |  | Decimal, optional |
|  | workCompleted |  | true/false | Boolean, optional |
|  | workLevel |  |  | Integer, optional |
|  | workPositionNumber |  |  | String, optional |
|  | workTime20 |  |  | Decimal, optional |
|  | workTime30 |  |  | Decimal, optional |
|  | workTime45 |  |  | Decimal, optional |
|  | workType |  |  | Integer, optional |
|  | worktime |  |  | Decimal, optional |
