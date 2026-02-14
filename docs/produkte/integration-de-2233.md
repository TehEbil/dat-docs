---
title: "Integration der Oberfläche"
topic_id: "2233"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Integration der Oberfläche"
---

# Integration der Oberfläche

Das Produkt SilverDAT 3 valuateFinance stellt Fremdanwendungen eine Schnittstelle zur Verfügung mit der sie die Oberfläche
der SilverDAT 3 valuateFinance in eine eigene Anwendung einbinden können. Die Integration funktioniert nur mit https.

Die Oberfläche der SilverDAT 3 valuateFinance lässt sich auf zwei verschiedene Arten einbinden:

- Durch Integration in einen bestehenden Dialog (=Seite), der neben SilverDAT 3 valuateFinance auch Inhalte und/oder Steuerelemente der Fremdanwendung beinhaltet.
- Durch Integration in einen neuen, leeren Dialog (=Seite)

Beim Aufruf der Oberflächen-Schnittstelle müssen zusätzliche Parameter übermittelt
werden. Die benötigten Parameter sind von der gewählten Aktion abhängig, diese werden
von der SilverDAT 3 valuateFinance als Voreinstellungen übernommen und zur Anzeige bzw. Vorauswahl gebracht.

Die Integration findet über eine bereitgestellte JavaScript-Klasse statt, die der
aktuellen Seite einen Inlineframe iframe mit der Oberfläche der SilverDAT 3 valuateFinance hinzufügt.

Abbildung: Beispiel für die Integration in eine herkömmliche HTML-Seite

Beim Aufruf der Oberflächen-Schnittstelle wird abhängig von den gewählten Vorgaben
die entsprechende Seite mit den zugehörigen Daten angezeigt. Beim Verlassen über den
Zurück-Button wird der Fremdanwendung der gesamte Vorgang als Dossier VXS zur Verfügung gestellt. Die Fremdanwendung kann diese Daten anschließend verarbeiten,
die SilverDAT 3 valuateFinance schließen und eigene Inhalte in der Seite zur Anzeige bringen oder die Seite komplett
verlassen.
