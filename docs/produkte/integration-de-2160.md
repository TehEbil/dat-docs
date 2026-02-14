---
title: "Integration der Oberfläche"
topic_id: "2160"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Integration der Oberfläche"
---

# Integration der Oberfläche

Eine Fremdanwendung hat prinzipiell zwei Möglichkeiten die Oberfläche der SilverDAT
calculatePro einzubinden:

- Integration in einen bestehenden Dialog (=Seite), der neben SilverDAT calculatePro
  auch Inhalte und/oder Steuerelemente der Fremdanwendung beinhaltet.
- Integration in einen neuen, leeren Dialog (=Seite)

Die Integration findet über eine von DAT bereitgestellte JavaScript-Klasse statt,
die der aktuellen Seite einen iframe mit der Oberfläche der SilverDAT calculatePro
hinzufügt.

Abbildung : Beispiel für die Integration in eine herkömmliche HTML-Seite

Sobald der Benutzer die Fahrzeugauswahl abgeschlossen hat, wird der "Weiter" (Orange
mit weißem Pfeil nach rechts) freigeschaltet. Bei Klick auf diesen Button wird in
die grafische Teileauswahl gewechselt, von der der Benutzer wiederum nach abgeschlossener
Definition des Schadensumfangs in das Kalkulationsergebnis geleitet wird. Bei Klick
auf den Weiter-Button im Kalkulationsergebnis werden der Fremdanwendung die Identifikationsdaten
(DAT €uropa-Code, ggfs. Marktindex und Bauzeit) des gewählten Fahrzeugs übermittelt.
Die Fremdanwendung kann dann über die entsprechende Webserviceoperation das Kalkulationsergebnis
im Hintergrund abrufen, die Oberfläche der SilverDAT calculatePro schließen und eigene
Inhalte in der Seite zur Anzeige bringen oder die aktuelle Seite komplett verlassen
oder sogar das Browserfenster schließen.
