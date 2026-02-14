---
title: "Responsebeschreibung getBatteryValuationParams"
topic_id: "26378"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Fahrzeugbewertung von Elektroautos > Fahrzeugbewertung von Elektroautos > Moeglichkeit der Bewertung für Elektroautos erfragen > Responsebeschreibung getBatteryValuationParams"
---

# Responsebeschreibung getBatteryValuationParams

###### Responsebeschreibung getBatteryValuationParams Parameter response | Parameter | Datentyp | Beschreibung | | --- | --- | --- | | DatECode | String | DAT €uropa-Code® | | Container | String | Marktindex | | ConstructionTime | Integer | Bauzeit | | MileageEstimated | Integer | Kilometerangabe | | InitialRegistration | Date | Erstzulassung | | Country | String | Datenland, für das die Möglichkeit der erweiterten Bewertung für Elektrofahrzeuge abgefragt wird. | | Language | String | Sprache | | BatteryValuationPossible | Boolean | gibt an, ob die erweiterte Bewertung von Elektrofahrzeugen vollumfänglich möglich ist. | | UserBatteryStateOfHealthPossible | Boolean | gibt an, ob ein Benutzerwert für BatteryStateOfHealth angegeben werden kann. | | UserBatteryCorrPossible | Boolean | gibt an, ob ein Benutzerwert für BatteryCorr angegeben werden kann. | | BatteryParameters | batteryParameters | enthält Unterelemente mit weiteren Batterieparametern | Parameter BatteryParameters | Parameter | Datentyp | Beschreibung | | --- | --- | --- | | ReplacementEffort | Decimal | Wiederbeschaffungswert der Fahrzeugbatterie in Netto | | ReplacementEffortGross | Decimal | Wiederbeschaffungswert der Fahrzeugbatterie in Brutto | | Distance | Double | Reichweite | | BatteryStateOfHealth | Decimal | DAT-Wert für den Ist-State of Health der Fahrzeugbatterie |
