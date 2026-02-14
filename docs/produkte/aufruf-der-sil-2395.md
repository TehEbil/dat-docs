---
title: "Aufruf der SilverDAT calculatePro / calculateExpert Oberfläche"
topic_id: "2395"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Integration der Oberfläche > Aufruf der SilverDAT calculatePro / calculateExpert Oberfläche"
---

# Aufruf der SilverDAT calculatePro / calculateExpert Oberfläche

|  |  |
| --- | --- |
|  | Bitte lesen Sie in jedem Fall die Kapitel [Aufbereitung der Authentifizierungsinformationen](#showid/2397 "Aufbereitung der Authentifizierungsinformationen"), [Callback-Methode für die Verarbeitung eines abgeschlossenen Vorgangs](#showid/2399 "Callback-Methode für die Verarbeitung eines abgeschlossenen Vorgangs") und [Callback-Methode für Fehlerbehandlungen](#showid/2402 "Callback-Methode für Fehlerbehandlungen"), bevor Sie mit diesem Topic fortfahren. |
| Tipp |

Zum Aufruf von SilverDAT calculatePro über Schnittstelle werden benötigt:

- Basis-URL: https://www.dat.de/VehicleRepairOnline
- Zieladresse

Das globale sphinx-Objekt stellt für den Aufruf eine Eigenschaft und zwei Methoden zur Verfügung. Zuerst
muss die Eigenschaft host gesetzt, dann die Fahrzeugauswahl über die Methode init initialisiert und schließlich über die Methode execute zur Anzeige und Ausführung gebracht werden.

| Methode bzw. Property | Typ | Bedeutung |
| --- | --- | --- |
| sphinx.host | Eigenschaft | Basis-URL der DAT €uropa-Code Fahrzeugauswahl |
| sphinx.servletmapping | Eigenschaft | "external" |
| sphinx.init | Methode | Initialisierung der Fahrzeugauswahl mit den Parametern (s. Tabelle unten "Aufrufparameter"):  Zieladresse  ID der Zielseite  Name der DOM-Node unter der der iFrame für SilverDAT calculatePro erzeugt werden soll (bei Übergabe von null wird der iFrame direkt unter body erzeugt  Name der CSS-Klasse mit CSS-Eigenschaften für den zu erzeugenden iFrame, bspw. modelIFrame  null oder Adresse (URL) eines eigenen CSS-Stylesheets mit weiterführenden CSS-Eigenschaften  Callback-Methode zur Entgegennahme der Benachrichtigung über Abschluss des Vorgangs in SilverDAT calculatePro |
| sphinx.firstPage | Eigenschaft | Steuerung der bearbeitbaren Masken. Sperrt alle vorhergehenden Masken. Bearbeitet werden können nur alle nachfolgenden Masken. Diese Eigenschaft ist optional. Wird sie nicht explizit gesetzt, kann der User auf alle Masken zugreifen.  Mögliche Werte sind:  model - Maske Fahrzeugauswahl  graphicSelectionPage - Maske graphische Teileauswahl  activityRelated - Maske Vorgangsbezogene Daten  calculationResult - Maske Kalkulationsergebnis  printAndSend - Maske Drucken und senden |
| sphinx.lastPage | Eigenschaft | Steuerung der Ausstiegsmaske. Verhindert damit das Springen in darauf folgende Masken, da alle nachfolgenden Masken gesperrt sind. Bearbeitet werden können nur die bis dahin freigegebenen Masken. Diese Eigenschaft ist optional. Wird sie nicht explizit gesetzt, kann der User auf alle Masken zugreifen.  Mögliche Werte sind:  calculationResult - Maske Kalkulationsergebnis  printAndSend - Maske Druck und Versand  graphicSelectionPage - Maske graphische Teileauswahl |
| sphinx.execute | Methode | Anzeige bzw. Ausführung der Oberfläche mit den Parametern: Authentifizierungsdaten vom Typ DatLoginInformation null oder XML-String mit einer Vorgangsnummer und Callback-Methode für Fehlerbehandlungen |

Nachfolgend sehen Sie eine Abbildung der calculatePro Oberfläche mit der Dropdown-Liste
der aufrufbaren Masken. Masken, die für den User gesperrt sind, sind ausgegraut (z.B.
'Drucken und senden').
