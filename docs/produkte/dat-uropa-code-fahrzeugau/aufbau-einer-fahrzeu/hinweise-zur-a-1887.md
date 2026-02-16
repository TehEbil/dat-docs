---
title: "Hinweise zur Abfrage von Fahrzeugart und Hersteller"
topic_id: "1887"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Aufbau einer Fahrzeugauswahl > Fahrzeugauswahl: Der Basistyp > Hinweise zur Abfrage von Fahrzeugart und Hersteller"
---

# Hinweise zur Abfrage von Fahrzeugart und Hersteller

Es gibt zwei Möglichkeiten, die Fahrzeugauswahl benutzerfreundlich aufzubauen. Diese
sind abhängig vom Klientel, das Ihre Fahrzeugauswahl zukünftig bedienen wird:

1. Ihre zukünftigen Nutzer sind normale Nutzer, die nicht aus dem Automotive-Bereich
   stammen, z.B. Privatpersonen:  
     
   Um den Fehlerquotienten bei der durchzuführenden Fahrzeugauswahl zu senken, und die
   Auswahl der einzelnen Basistyp-Komponenten auf ein Minimum einzuschränken, empfiehlt
   es sich, schon zu einem sehr frühen Zeitpunkt, das Erstzulassungsdatum des Fahrzeugs
   abzufragen und in den nachfolgenden Abfragen zu verwenden.  
     
   Das abgefragte Erstzulassungsdatum wird mithilfe der Schnittstellenfunktion date2constructionTime in eine vierstellige DAT-Notation gewandelt, mit der Sie alle nachfolgenden Abfragen
   filtern können. Lesen Sie bitte im   
   Kompendium > SilverDAT Produkte > [Ihre genutzte Anwendung] > [Schnittstellenbeschreibungen]
   > date2constructionTime  
   alles zum Aufruf und zur Behandlung dieser Schnittstellenfunktion inklusive einer
   Beispiel-Notation.
2. Ihre zukünftigen Nutzer sind Personen aus dem Automotive-Bereich, z.B. Werkstattmeister,
   Kfz-Händler, Autoversicherer:  
     
   Entsprechende Kfz-Erfahrung vorausgesetzt, können Sie zu diesem Zeitpunkt auf eine
   Abfrage des Erstzulassungsdatums verzichten und direkt mit der Abfrage von Fahrzeugart
   und Hersteller beginnen. Es sei denn, Sie möchten Ihren Nutzern die Auswahl so weit
   wie möglich vorfiltern:   
     
   Das abgefragte Erstzulassungsdatum wird mithilfe der Schnittstellenfunktion date2constructionTime in eine vierstellige DAT-Notation gewandelt, die Bauzeit, mit der Sie alle nachfolgenden
   Abfragen filtern können. Lesen Sie bitte im   
   Kompendium > SilverDAT Produkte > [Ihre genutzte Anwendung] > [Schnittstellenbeschreibungen]  
   alles zum Aufruf und zur Behandlung dieser Schnittstellenfunktion inklusive einer
   Beispiel-Notation.

Oldtimer (Fahrzeuge > 20 Jahre),Youngtimer (Liebhaberfahrzeuge, die aber noch keinen
Oldtimerstatus besitzen) und Neufahrzeuge können nicht bewertet werden. Bei der Abfrage
des Erstzulassungsdatums sollten Sie dies gleich berücksichtigen und dem Nutzer einen
entsprechenden Hinweis ausgeben.

Bei der Abfrage nach der Fahrzeugart halten Sie sich bitte an die Informationen im
  
Kompendium > SilverDAT Produkte > DAT Europa-Code® Fahrzeugauswahl > Fahrzeugauswahl
- Funktionen > getVehicleTypes

Setzen Sie Filter, wo immer es Ihnen angeboten wird

Unsere neuen SilverDAT Produkte (valuateFinance, CalculatePro, CalculationAudit, DAT €uropa-Code Fahrzeugauswahl) bieten einen weiteren Filter an, den Sie unbedingt abfragegenau nutzen sollten:
den Parameter <restriction>.

Mit diesem Filter können Sie die zurückgegebene Datenmenge auf ihre endgültige Verwendung
einschränken("ALL", "REPAIR", "APPRAISAL"). Es ist möglich, nur Fahrzeuge, die für eine Fahrzeuginstandsetzung geeignet sind
("REPAIR"), oder nur bewertungsfähige Fahrzeuge ("APPRAISAL") oder alle Fahrzeuge ohne Einschränkung ("ALL") auszugeben. Wenn Sie den Filter nicht verwendungsgenau festlegen, kann das dazu
führen, dass ein Fahrzeug, das Sie bewerten möchten, eine Fehlermeldung ausgibt, weil
es nicht für die Bewertung geeignet ist. Dies können Sie durch die Verwendung des
Filters vermeiden.

Setzen Sie die Bauzeiteinschränkung, wann immer es Ihnen ermöglicht wird

Schon bei der Abfrage des Herstellers mit der Schnittstellenfunktion getManufacturers können Sie die Bauzeiteinschränkung nutzen, indem Sie das Erstzulassungsdatum, das
Sie in DAT-Notation umgewandelt haben, als Wert in den Parameter <constructionTimeTo> einsetzen.

Dies bedeutet, dass Ihnen nur Hersteller ausgegeben werden, für die, bis zum Zeitpunkt
des übergebenen Erstzulassungsdatums, Fahrzeuge im Datenbestand existieren. Eine Bauzeiteinschränkung
ab Hersteller macht unter folgenden Prämissen Sinn:

- Es ist wahrscheinlich, dass Ihre Nutzer Old- oder Youngtimer oder Neufahrzeuge abfragen
  werden; betrifft vor allem deren Bewertung
- Sie haben das Erstzulassungsdatum nicht schon zu Anfang abgefragt und Ihren Nutzer
  noch nicht darauf aufmerksam gemacht, dass die vorgenannten Fahrzeuge nicht bewertet
  werden können.
- Sie möchten dem Nutzer die Auswahl erleichtern, indem Sie nur Hersteller ausgeben,
  die für die spätere Verwendung (Bewertung, Schadenskalkulation) geeignet sind. Hersteller,
  die zu einem bestimmten Zeitpunkt noch keine Fahrzeuge auf dem Markt hatten oder auch
  nicht mehr auf dem Markt hatten, werden erst gar nicht angezeigt.
