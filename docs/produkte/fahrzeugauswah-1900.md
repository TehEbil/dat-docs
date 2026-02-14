---
title: "Fahrzeugauswahl Marktindex"
topic_id: "1900"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Aufbau einer Fahrzeugauswahl > Fahrzeugauswahl Marktindex"
---

# Fahrzeugauswahl Marktindex

Der Marktindex beinhaltet die Sammlung kaufmännischer Betrachtungen eines anhand des
DAT €uropa-Code® technisch eindeutig identifizierten Fahrzeuges.

Der Marktindex besteht aus der Landeskennung (Länderkennzeichen ISO-3166-1-Char2)
und einer Sammlung möglicher kaufmännischer Preisfindungsvarianten, die als charakterisierende
Ausstattungen abgebildet sind, in Abhängigkeit zum DAT €uropa-Code®.

Aufbau eines DAT €uropa-Code®, mit Marktindex bestehend aus Container und Bauzeit  
(der Container ist orange dargestellt).

Mit der Funktion getPriceFocusCases kann der Marktindex zu einem DAT €uropa-Code® ermittelt werden.

Auch für die Abfrage nach dem Marktindex gilt:

1. Nutzen Sie die Bauzeiteinschränkung, wann immer es möglich ist
2. Setzen Sie den Filter <restriction> verwendungsgenau

Programmier-Beispiel:

```
...
List<KeyStringValueStringPair> content = WtkTypeConverter
    .keyStringValueStringPairs2List(
            sdoClient.getPriceFocusCases(
        getDatCustomerNo(), getDatLogin(), getDatPassword(), datECode), 
                "Bitte auswählen");
    containerListBtn.setEnabled(true);
    containerListBtn.setListData(content);
...
```
