---
title: "Integration der Oberfläche"
topic_id: "26036"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Integration der Oberfläche"
---

# Integration der Oberfläche

Das Produkt SilverDAT 3 Mietwagenspiegel stellt Fremdanwendungen eine Schnittstelle zur Verfügung mit der sie die Oberfläche
des Produkts SilverDAT 3 Mietwagenspiegel in eine eigene Anwendung einbinden können. Bitte beachten Sie, dass bei der Oberflächen-Integration
unserer Produkte mittels iFrame alle URLs die sich auf Produkte oder Ressourcen der DAT beziehen das HTTPS-Protokoll verwenden müssen.

Die Oberfläche des Produkts SilverDAT 3 Mietwagenspiegel lässt sich auf zwei verschiedene Arten einbinden:

- Durch Integration in einen bestehenden Dialog (=Seite), der neben SilverDAT 3 Mietwagenspiegel auch Inhalte und/oder Steuerelemente der Fremdanwendung beinhaltet.
- Durch Integration in einen neuen, leeren Dialog (=Seite)

Die Integration findet über eine bereitgestellte JavaScript-Klasse statt, die der
aktuellen Seite einen Inlineframe iframe mit der Oberfläche des Produkts SilverDAT 3 Mietwagenspiegel hinzufügt. Beim Aufruf der Oberflächen-Schnittstelle müssen zusätzliche Parameter
übermittelt werden, Umfang und Inhalt der Angaben hängen von der gewählten Konstellation
ab. Mit diesen Parametern steuern Sie den Aufruf des Produkts SilverDAT 3 Mietwagenspiegel.

Abbildung : Beispiel für die Integration in eine herkömmliche HTML-Seite

Beim Aufruf der Oberflächen-Schnittstelle wird abhängig von den gewählten Vorgaben
die entsprechende Seite mit den zugehörigen Daten angezeigt. Ganz oben auf der Seite
finden Sie die Menüleiste mit den Steuerungselementen zur Navigation.

Abbildung : Beispiel für eine vollständig aufgeklappte Menüleiste

Die Menüleiste klappen Sie auf, indem Sie links oben auf den Pfeil mit dem Prozessnamen
klicken. Sie navigieren innerhalb des aktuellen Workflows, indem Sie entweder auf
einen der Pfeile oder direkt auf eine Zielseite in der Workflow-Leiste klicken.
