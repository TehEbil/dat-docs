---
title: "Fahrzeugauswahl: Der Basistyp"
topic_id: "1885"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Aufbau einer Fahrzeugauswahl > Fahrzeugauswahl: Der Basistyp"
---

# Fahrzeugauswahl: Der Basistyp

Die Schnittstellenfunktionen der Fahrzeugauswahl bauen aufeinander auf, d.h. die zurückgegebenen
Ergebnisse werden bei einer Abfrage übermittelt, um den DAT €uropa-Code® zu erhalten.
Sie nehmen also den zurückgegebenen Fahrzeugart-Schlüssel, um eine Liste der Hersteller
für diese Fahrzeugart anzufordern. Danach nehmen Sie den Fahrzeugart-Schlüssel und
den ausgewählten Hersteller-Schlüssel, um eine Liste der Haupttypen anzufordern usw.

Für den sogenannten Basiscode, bestehend aus Fahrzeugart, Hersteller, Haupt- sowie
Untertyp (s. Beispielgrafik), ist das sehr einfach.

Nach Auswahl des Untertyps wird die Kaskade komplexer, da die Ausstattungen der nun
folgenden Typvariante von der Fahrzeugart abhängig sind.

Lesen Sie in den nachfolgenden Kapiteln, wie Sie bei der Abfrage des Basistyps vorgehen
können und was Sie beachten sollten.
