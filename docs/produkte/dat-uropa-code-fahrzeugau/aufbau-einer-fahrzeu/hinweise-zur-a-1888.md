---
title: "Hinweise zur Abfrage des Haupt- und Untertyps"
topic_id: "1888"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Aufbau einer Fahrzeugauswahl > Fahrzeugauswahl: Der Basistyp > Hinweise zur Abfrage des Haupt- und Untertyps"
---

# Hinweise zur Abfrage des Haupt- und Untertyps

Bitte lesen Sie die Kapitel ab [Fahrzeugauswahl: Der Basistyp](fahrzeugauswah-1885.md), bevor Sie hier weiterlesen. Beachten Sie vor allem die Hinweise zu den Abfragen.

Setzen Sie Filter, wo immer es Ihnen angeboten wird

Bitte nutzen Sie auch bei der Abfrage nach Haupt- und Untertyp die Filtermöglichkeit,
wie im Unterkapitel [Hinweise zur Abfrage von Fahrzeugart und Hersteller](hinweise-zur-a-1887.md) beschrieben.

Nutzen Sie die Bauzeiteinschränkung, wann immer es möglich ist

Sie sollten spätestens mit der Abfrage nach dem Haupttyp beginnen, und zwar über die
Schnittstellenfunktion getBaseModels, die Bauzeiteinschränkung regelmäßig in Ihre Abfragen einzubeziehen.

Wenn Sie also das Erstzulassungsdatum noch nicht abgefragt haben, sollten Sie dies
spätestens jetzt erledigen. Das Erstzulassungsdatum benutzen Sie, um es mit der Schnittstellenfunktion
date2constructionTime in die vierstellige DAT-Notation, die Bauzeit, umzuwandeln.

Mit dem Ergebnis der Umwandlung befüllen Sie zukünftig den Parameter <constructionTimeTo> Ihrer Abfragen. Dies bedeutet, dass Ihnen nur Daten zurückgegeben werden, für die,
bis zum Zeitpunkt des übergebenen Erstzulassungsdatums, Fahrzeuge im Datenbestand
existieren.

Eine Bauzeiteinschränkung ab Haupttyp bzw. Untertyp macht unter folgenden Prämissen
Sinn:

- Sie möchten dem Nutzer die Auswahl erleichtern, indem Sie nur Haupt- oder Untertypen
  eines Herstellers ausgeben, die für die spätere Verwendung (Bewertung, Schadenskalkulation)
  geeignet sind. Haupt- oder Untertypen, die zu einem bestimmten Zeitpunkt noch gar
  nicht oder nicht mehr existieren, werden dadurch erst gar nicht angezeigt.
