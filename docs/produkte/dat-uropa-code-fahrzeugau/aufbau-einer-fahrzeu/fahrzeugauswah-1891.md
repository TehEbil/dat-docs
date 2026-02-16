---
title: "Fahrzeugauswahl: Die Typvariante"
topic_id: "1891"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Aufbau einer Fahrzeugauswahl > Fahrzeugauswahl: Die Typvariante"
---

# Fahrzeugauswahl: Die Typvariante

Bitte lesen Sie die Kapitel ab [Fahrzeugauswahl: Der Basistyp](fahrzeugauswah-1885.md), bevor Sie hier weiterlesen. Beachten Sie vor allem die Hinweise zu den Abfragen.

Beispiel eines DAT €uropa-Code®, mit 9-stelligem Marktindex und Bauzeit in DAT-Notation  
(der DAT-Schlüssel zur Typvariante ist blau dargestellt).

Die klassifizierende Ausstattung und ihre Bedeutung

Die Typvariante verschlüsselt die verbauten, klassifizierenden Ausstattungen eines
Fahrzeugs. Um den Schlüssel zu erhalten, müssen Sie alle klassifizierenden Ausstattungen
eines Fahrzeugs abfragen.

Eine klassifizierende Ausstattung im Sinne der DAT ist eine Ausstattung, die es ermöglicht,
ein Fahrzeug technisch eindeutig zu identifizieren. Da diese Ausstattungen über 85%
des Fahrzeuges ausmachen, wird im DAT-Umfeld - nach der A-B-C Analyse - von den A-AV
gesprochen.

| Klassifizierungsgruppe | Gruppen-Nr. | Pkw | Geländefahrzeug | Transporter | Kraftrad | Lkw |
| --- | --- | --- | --- | --- | --- | --- |
| Motor | 1 | X | X | X | X | X |
| Karosserie | 2 | X | X | X | X |  |
| Bauart | 7 |  |  |  |  | X |
| Getriebe | 11 | X | X | X |  |  |
| Radstand | 3 |  | X | X |  | X |
| Antriebsart | 4 |  | X | X |  |  |
| Anzahl Achsen | 9 |  |  |  |  | X |
| Fahrerhaus | 5 |  |  |  |  | X |
| Tonnage | 6 |  |  |  |  | X |
| Federungsart | 8 |  |  |  |  | X |
| Ausstattungslinie (optional) | 10 | X | X | X | X | X |

Die 1. Spalte gibt die Ausstattung wieder, die als klassifizierende Ausstattung gewertet
wird.   
Die 2. Spalte gibt den Schlüssel wieder, der bei der DAT für diese klassifizierende
Ausstattung benutzt wird.  
Die 3. - 7. Spalte gibt wieder, welche Fahrzeugart im DAT-System mit welcher klassifizierenden
Ausstattung verwendet wird.

Laut der oben angezeigten Matrix benötigt ein Pkw also die folgenden klassifizierenden
Ausstattungen (A-AVs), um technisch eindeutig identifiziert werden zu können:

1. Motor
2. Karosserie
3. Getriebe und
4. Ausstattungslinie (allerdings nur optional, da nicht jeder Hersteller Ausstattungslinien
   verwendet)

Bei der Abfrage der klassifizierenden Ausstattung eines Fahrzeugs muss - analog zur
Abfrage des Basistyps - alle bereits gewählten Ausstattungen an die nächste Abfrage
übermittelt werden. Hier ein Programmier-Beispiel:

```
...
KeyIntValueStringPair[] result = getSdoClient().getEngineOptions(getDatCustomerNo(), 
   getDatLogin(), getDatPassword(), vehicleType, manufacturer, baseModel, subModel,
    availableOptions);
...
```

Damit Sie alle notwendigen klassifizierenden Ausstattungen dynamisch - angepasst an
die jeweils gesuchte Fahrzeugart, den Hersteller und Haupt- und Untertyp - erhalten,
benutzen Sie bitte die Schnittstellenfunktion getClassificationGroups Ihrer jeweils genutzten SilverDAT Anwendung. Diese Schnittstellenfunktion gibt Ihnen
alle Gruppennummern (s. Matrix oben, 2. Spalte) wieder, die zwingend benötigt werden,
um das Fahrzeug technisch zu identifizieren.

Übergeben Sie zu wenig oder die falsche klassifizierende Ausstattungen, um ein Fahrzeug
zu identifizieren, erhalten Sie falsche Ergebnisse zurück.

Bitte lesen Sie weitere Informationen zur Schnittstellenfunktion getClassificationGroups im

Kompendium > SilverDAT Produkte > DAT Europa-Code® Fahrzeugauswahl > Fahrzeugauswahl
- Funktionen > getClassificationGroups

Kaskadierende klassifizierende Ausstattung in einer Beispiel-Anwendung

Und auch für die Abfrage der klassifizierenden Ausstattung gilt:

1. Nutzen Sie die Bauzeiteinschränkung, wann immer es möglich ist
2. Setzen Sie den Filter <restriction> verwendungsgenau
