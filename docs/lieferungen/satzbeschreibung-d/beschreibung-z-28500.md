---
title: "Beschreibung Zusatzelement 1b"
topic_id: "28500"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 1b"
---

# Beschreibung Zusatzelement 1b

Bauzeiten und Ausstattungsvarianten

Das Zusatzelement 1b liefert die Serien- und Sonderausstattung zu einem DAT €uropa-Code®
sowie Angaben zum Bauzeitraum der DAT €uropa-Codes®.

Außerdem gibt es eine Datei mit der Beschreibung des Marktindex, einer Erweiterung,
die es erlaubt, ein Fahrzeug noch präziser hinsichtlich bewertungsrelevanter Information
auszuwählen.

Diese Informationen bilden die maßgebliche Voraussetzung für alle weiterführenden
Maßnahmen zur Datenverarbeitung, wie zum Beispiel für eine korrekte Zuordnung der
Ergebnisse der DAT-Marktbeobachtung (Gebrauchtfahrzeugwerte und Restwertprognosen).

Pro DAT €uropa-Code® - AV - AV-Zeitpunkt-Ab wird jeweils ein Datensatz für die verfügbaren
Serien- und möglichen Sonderausstattungen mit dem jeweiligen Bauzeitpunkt (AV-Zeitpunkt-Ab)
ausgegeben.

An klassifizierten Ausstattungsvarianten werden zunächst nur die beim DAT €uropa-Code®
direkt gespeicherten ausgegeben. Für alle anderen Ausstattungen besteht eine Möglichkeit
der Ansteuerung. Die NICHTWENN / NUR-WENN-Umfasst-Logik wird dabei nicht weiter ausgewertet.

Sollte diese erforderlich sein, kann die DAT auf Wunsch eine Webapplikation zur Verfügung
stellen, welche eine entsprechende Logikprüfung ermöglicht.

Der Name der XML-Root-Elements lautet „zusatz1b" und der Name eines Satz-Elements
lautet „zusatz1b\_s".

Damit Informationen, die von den Ausstattungsvarianten (AV) abhängig sind, nicht immer
redundant wiederholt werden müssen , gibt es zusätzlich eine AV-Stammdatendatei.

Der Name des entsprechenden XML-Root-Elements lautet „zusatz1b\_av" und der Name eines
Satz-Elements lautet „zusatz1b\_av\_s". Zusatz1b\_av enthält alle AV pro Haupttyp und
zusatz1b\_av\_s enthält alle AV pro Hersteller.

Achtung: Sowohl in zusatz1b\_av als auch in zusatz1b\_av\_s befinden sich nur kalkulierbare
Ausstattungen!  
Nur im Typenheft enthaltene Ausstattungen werden ausgegeben.  
Gesperrte Sonderausstattungen (HTBU\_KZ\_SONDER = 'X' AND HTBU\_KZ\_PR\_STEU = '0') werden
nicht ausgegeben.

Bei den Informationen zum Bauzeitraum wird ein Satz pro DAT €uropa-Code® ausgegeben.
Der Beginn eines Bauzeitraumes wird über die Eckbauzeit-Von des Untertyps und den
jeweils ältesten Eintrag der einzelnen AVs des DAT €uropa-Codes® im Typkatalog (Datenstrang
der zum jeweiligen Modell verfügbaren Serien- und Sonderausstattungen) ermittelt.
Das Ende eines Bauzeitraums ist das Ende des jüngsten Jahres aus Baujahr-Bis unter
den zugeordneten DAT-Untertypen.

Der Name der XML-Root-Elements lautet „zusatz1b\_bz" und der Name eines Satz-Elements
lautet „zusatz1b\_bz\_s".

Bei den Marktindizes wird pro DAT €uropa-Code®-Marktindex ein Satz ausgegeben.

Der Name des XML-Root-Elements ist „zusatz1b\_con", der Name eines Satz-Elements „zusatz1b\_con\_s".
