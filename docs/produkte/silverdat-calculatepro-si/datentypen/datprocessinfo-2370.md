---
title: "datProcessInfo und DVNInfo (Veraltet!)"
topic_id: "2370"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Datentypen > datProcessInfo und DVNInfo (Veraltet!)"
---

# datProcessInfo und DVNInfo (Veraltet!)

Die datProccessInfo, DVNInfo oder DVN ist ein Container der kalkulationsrelevante Daten wie z. B. Arbeits- und Reparaturanweisungen,
Prozesse und ähnliches modelliert. Die Struktur des DVNInfo Objektes ist immer gleich, und hat eine Vielzahl an Attributen. Die Bedeutung der
Attribute wird über das "Method" Attribut gesteuert.

Generell muss die Gesamtheit der Attribute einer DVN eindeutig sein. Es ist Beispielsweise kein Fehler wenn z. B. zwei DVN mit der gleichen "processId" und "method" existieren, sich aber im "repaircode" unterscheiden.

Die Motivation hierbei ist, dass sich hierdurch die verschiedenen Methoden kombinieren
lassen. Ein Beispiel wäre hierfür ein Teil das einerseits ersetzt (repaircode "E") wird und andererseits aber zusätzlich Kosten für Aus- und Einbau (repaircode A) erzeugt.

"datProcessId" Attribut

Ein DVNInfo Objekt enthält immer eine "datProcessId" bzw. DVN. Die DVN dient dazu vordefinierte Teile, Arbeitsschritte und Prozesse eindeutig zu definieren.

"method" Attribut

Das "method" Attribut steuert die Art und Eigenschaften des DVN Objekts. Ob eine Eigenschaft ungenutzt, optional oder notwendig ist hängt jeweils
von diesem Attribut ab. Die verschiedenen Methoden sowie deren Eigenschaften sind
im folgenden näher beschrieben. Ist keine oder eine ungültige Methode definiert wird
auf "GRAPHICAL" zurückgegriffen. Insbesondere die Bedeutung der Reparatur Codes unterscheidet sich
in Kombination mit der Methode.

- GRAPHICAL

  Hierüber ist die graphische Teileauswahl nachgebildet.

  "repairCode" Attribut

  Das repairCode Attribut ist ähnlich einer Arbeitsanweisung. Je DVN Objekt kann immer nur ein repairCode definiert werden. Sind für ein Bauteil mehrere Reparaturanweisungen notwendig, so
  legt man für jeden Typ ein eigenes DVN Objekt an. Es ist somit kein Fehler, wenn mehrere DVN Objekte die gleiche datProcessId haben aber unterschiedliche repairCodes definieren.

  Es existieren die folgenden repairCodes. Ihre Bedeutung ist analog zu der der graphischen Teileauswahl. Ist kein oder ein
  ungültiger repairCode angegeben so wird "REPLACE (E)" als Fallback genutzt.

  |  |  |  |
  | --- | --- | --- |
  | REPAIRCODE | Kürzel | Bedeutung |
  | DIS\_MOUNTING | A | Aus- und Einbau |
  | UNDERBODY\_PROTECTION | B | Unterbodenschutz |
  | SPOT\_REPAIR | C | Spot Repair Lackierung |
  | DISASSEMBLY | D | Zerlegen |
  | REPLACE (default) | E | Ersetzen (default wenn kein Typ definiert wurde) |
  | ASSEMBLY | F | Montieren |
  | CUTTING | G | Schneiden |
  | DEAREATE | H | Entlüften |
  | OVERHAUL | I | Instandsetzen (mit Lack) |
  | CLEANING | J | Reinigen |
  | FIXING | / | Instandsetzen (ohne Lack) |
  | CAR\_BODY | K | abzugsfähige Kosten bei Rohbaukarosse |
  | LACQUER | L | Lackieren |
  | LACQUER\_DISMOUNTED | M | Montageteil demontiert lackieren |
  | ADDITIONAL\_COSTS | N | Nebenkosten |
  | BODY\_CAVITY\_PROTECTION | O | Hohlraumschutz |
  | VISUAL\_INSPECTION | P | Sichtprüfung (bzw. Polieren, wenn bei Karosserieteilen angegeben) |
  | REPLACE\_NO\_MATERIAL | Q | Ersetzen oder Erneuern - wie "E", aber nur Arbeitszeitberechnung, keine Materialkosten |
  | RISK | R | Risiko |
  | ADJUST | S | Einstellen |
  | TECHNICAL\_INSPECTION | T | technische Prüfung |
  | LACQUER\_NO\_AUTOMATICS | U | Lackieren ohne Lackierautomatik (nur bei der Typenhefterfassung - entspricht dem rot unterlegten "L" im Typenheft- wird intern vor der Kalkulation in "L" umgesetzt) |
  | MEASURING | V | Vermessen |
  | BALANCING | W | Wuchten |
  | EXPOSE | X | Freilegen (nur Arbeitslogik) |
  | COMPLETE | Y | Komplettieren (nur Arbeitslogik) |
  | DIS\_REASSEMBLE | Z | Zerlegen und Zusammenbauen |

  Attribute

  Der RepairCode definiert den Typ des DVNInfo Objektes und somit seine Attribute. Welche Attribute für welchen Typen gültig sind
  ist in der untenstehenden Tabelle dargestellt. Wird ein vom repairCode nicht unterstütztes Attribut gesetzt, so wird es stillschweigend ignoriert.

  Attribute sind bis auf wenige Ausnahmen optional. Wird ein Attribut weggelassen, so
  wird ein Standardwert angenommen.

  |  |  |  |  |
  | --- | --- | --- | --- |
  | Attribut | Kürzel | Bedeutung | Wertebereich |
  | price | E |  | Decimal |
  | isUsedPart | E |  | Boolean [true, false] |
  | difficultyAllowance | E, A |  | Decimal |
  | time | E, I, A, L, M, B, D, F, G, H, J, O, P, Q, S, T, U, V, W, X, Y, Z, /, N |  | Decimal [0-999999] |
  | lacquerLevel | E, I, / |  | Integer |
  | lacquerPercentage | E, I, L, M |  | Decimal |
  | noScratchTime | E, I |  | Integer |
  | discount | E, L, M, R |  | Decimal |
  | workLevel | E, I, A, / |  | Integer |
  | workType | E, I, A, / |  | Integer |
  | optimization | E, I, A, R, / |  |  |
  | preDamage | E, I, A, L, M, R, C, / | Teil hat einen Vorschaden | Boolean [true, false] |
  | location | I | Ortsangabe des Schadens  1 = vorn  2 = hinten  3 = oben  4 = unten  5 = mittig | Integer [1-5] |
  | countyLevelS | / |  |  |
  | countryLevelM | / |  |  |
  | coutnryLevelL | / |  |  |
  | price | /, N |  |  |
  | repairType | / |  |  |
  | countryLevelGlass | / |  |  |
  | amount | C, E, I, L, M, / | Anzahl der betroffenen Teile | Integer |
  | length | E, I, L, M, / | Die Länge des Ersatzteils bzw. des zu bearbeitenden Teils | Decimal |
  | width | E, I, L, M, / | Die Breite des Ersatzteils bzw. des zu bearbeitenden Teils. Zierleisten oder ähnliches die in Laufenden Metern abgerechnet werden, verfügen nur über eine Länge und keine Breite. | Decimal |
  | unit | E, I, L, M, / | Einheit, z.B. QM oder LFM ergibt sich aus der Fläche bzw der Länge des Bauteils. | String |
- MAINTENANCE

  Definiert Materialkosten bei der Wartungskalkulation. Die Wartungskalkulation ist
  durch das type Attribut verfeinert. Es gibt die folgenden Typen:

  |  |  |
  | --- | --- |
  | TYPE | Bedeutung |
  | LABOUR (default) | Arbeitsposition |
  | MATERIAL | Materialposition |
  | INTERVAL | Wartungsintervall |

  Attribute

  |  |  |  |  |
  | --- | --- | --- | --- |
  | Attribute | Typ | Bedeutung | Wert |
  | amount | Material |  | Decimal |
  | price | Material |  | Decimal |

  Beispiel für Material der Wartungskalkulation

  ```
  <!-- Maintenance -->
  <datProcessInfo method="MAINTENANCE" type="INTERVAL">
  <datProcessId>94030</datProcessId>
  </datProcessInfo>

  <!-- Zahnriemen der Motorsteuerung austauschen -->
  <datProcessInfo method="MAINTENANCE" type="LABOUR">
  <datProcessId>81715</datProcessId>
  </datProcessInfo>

  <!-- REP.-SATZ ZAHNRIEMEN -->
  <datProcessInfo method="MAINTENANCE" type="MATERIAL">
  <datProcessId>81715</datProcessId>
  <amount>2</amount>
  <price>130.90</price>
  </datProcessInfo>
  ```
- [DENTS](additional-ver-2377.md)
- MANUAL

  |  |  |  |
  | --- | --- | --- |
  | Attribute | Bedeutung | Wert |
  | price |  |  |
  | time |  |  |
  | amount |  |  |
  | laquerlevel |  |  |
  | processName |  |  |
  | partNumber |  |  |
  | WorkPositionNumber |  |  |
  | optimization |  |  |
  | preDamage | Teil hat einen Vorschaden. | Boolean [true | false] |
- ADDITIONAL

  |  |  |  |
  | --- | --- | --- |
  | Attribute | Bedeutung | Wert |
  | price |  |  |
  | time |  |  |
  | amount |  |  |
  | processName |  |  |
  | domusPart |  |  |

"suppressed" Attribut

Ist "suppressed" auf "true" gesetzt wird die DVNInfo bei der Kalkulation nicht berücksichtigt. Dies ermöglicht es verschiedene Variante
zu berechnen.

Beispiele

```
<!-- Reparieren -->
<datProcessInfo datProcessId="44210" method="GRAPHICAL" RepairCode="E">
</datProcessInfo>

<!-- Instandsetzen -->
<datProcessInfo datProcessId="44210" method="GRAPHICAL" RepairCode="/" />
</datProcessInfo>
```
