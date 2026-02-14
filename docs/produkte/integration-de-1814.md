---
title: "Integration der Oberfläche"
topic_id: "1814"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Oberflächen-Schnittstelle > Integration der Oberfläche"
---

# Integration der Oberfläche

Eine Fremdanwendung hat prinzipiell zwei Möglichkeiten, die Oberfläche der DAT €uropa-Code®
Fahrzeugauswahl einzubinden:

- Integration in einen bestehenden Dialog (=Seite), der neben der DAT €uropa-Code® Fahrzeugauswahl
  auch Inhalte und/oder Steuerelemente der Fremdanwendung beinhaltet.
- Integration in einen neuen, leeren Dialog (=Seite)

Bei der Einbindung können optionale Eingabewerte übermittelt werden, die von der DAT
€uropa-Code® Fahrzeugauswahl als „Benutzereingaben" übernommen und zur Anzeige bzw.
Vorauswahl gebracht werden.

Die Integration findet über eine von DAT bereitgestellt JavaScript-Klasse statt, welche
der aktuellen Seite einen iframe mit der Oberfläche der DAT €uropa-Code® Fahrzeugauswahl hinzufügt.

Abbildung : Beispiel für die Integration in eine herkömmliche HTML-Seite

Der Weiter-Button (Orange mit weißem Pfeil nach rechts) zeigt an, dass im eingestellten
Pageflow (Fahrzeugauswahl, Ausstattungsauswahl, Zusammenfassung und Technische Daten)
weitere Seiten folgen. Am Ende dieses Prozesses wird aus dem Weiter-Button ein Ende-Button
(Orange mit weißem Pfeil nach rechts gegen eine weiße senkrechte Linie). Beim Klick
auf den Ende-Button wird der Fremdanwendung das Ergebnis der Fahrzeugidentifikation
im DAT VXS-Format übermittelt. Die Fremdanwendung kann diese Daten anschließend verarbeiten,
die Fahrzeugauswahl schließen und eigene Inhalte in der Seite zur Anzeige bringen
oder die Seite komplett verlassen.
