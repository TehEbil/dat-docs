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

- [aufbereitung-d-2393](aufbereitung-d-2393.md)
- [aufbereitung-d-2397](aufbereitung-d-2397.md)
- [aufruf-der-sil-2395](aufruf-der-sil-2395.md)
- [aufrufbeispiel-2504](aufrufbeispiel-2504.md)
- [aufrufziele-2503](aufrufziele-2503.md)
- [callback-metho-2399](callback-metho-2399.md)
- [callback-metho-2402](callback-metho-2402.md)
- [html-grundgeru-2502](html-grundgeru-2502.md)
- [komplettbeispi-2505](komplettbeispi-2505.md)
- [notwendige-sch-2501](notwendige-sch-2501.md)
