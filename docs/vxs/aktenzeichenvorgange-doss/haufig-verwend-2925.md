---
title: "Häufig verwendete Attribute"
topic_id: "2925"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Häufig verwendete Attribute"
---

# Häufig verwendete Attribute

Für spätere Verwendungszwecke sind die Attribute „nil" und „overwrite" definiert.

Das Attribut „nil" erlaubt nicht belegte Felder (NULL in der Datenbank). Bei exportierten
Daten werden diese üblicherweise komplett weggelassen, um die Übersichtlichkeit zu
verbessern.

<ns:TextFeld nil="true"></ns:TextFeld> oder <ns:TextFeld nil="true" /> definiert somit, dass TextFeld nicht belegt ist, während <ns:TextFeld /> bzw. <ns:TextFeld></ns:TextFeld> einen Leerstring definiert.

Für Datentypen, die normalerweise keine leeren Inhalte erlauben, wie z.B. dateTime
oder decimal, wurden im xsd-Schema entsprechende Erweiterungen verwendet, so dass
auch <ns:DatumsFeld nil="true" /> möglich ist. Zudem werden bei diesen Datentypen auch ohne nil="true" leere Inhalte als „unbelegt" interpretiert.

Das Attribut „overwrite" ist für das Aktualisieren einzelner Felder bei vorhandenen Daten gedacht. Ist das
Attribut „false", wird das Feld in der Datenbank nicht verändert. Bis auf weiteres ist dies jedoch
nicht möglich, vorerst ist nur der Import vollständiger Aktenzeichen bzw. Vorgänge
geplant.
