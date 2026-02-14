---
title: "Integration der Oberfläche"
topic_id: "2305"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Verwalten der Fahrzeugbeschreibung > Fahrzeugbeschreibung holen > Mögliche Fehlercodes getVehicleColorUpholestery"
---

# Integration der Oberfläche

Das Produkt SilverDAT 3 valuateExpert/PlusPartner stellt Fremdanwendungen eine Schnittstelle zur Verfügung mit der sie die Oberfläche
der SilverDAT 3 valuateExpert/PlusPartner in eine eigene Anwendung einbinden können. Bitte beachten Sie, dass bei der Oberflächen-Integration
unserer Produkte mittels iFrame alle URLs die sich auf Produkte oder Ressourcen der DAT beziehen das HTTPS-Protokoll verwenden müssen.

Die Oberfläche der SilverDAT 3 valuateExpert/PlusPartner lässt sich auf zwei verschiedene Arten einbinden:

- Durch Integration in einen bestehenden Dialog (=Seite), der neben SilverDAT 3 valuateExpert/PlusPartner auch Inhalte und/oder Steuerelemente der Fremdanwendung beinhaltet.
- Durch Integration in einen neuen, leeren Dialog (=Seite)

Die Integration findet über eine bereitgestellte JavaScript-Klasse statt, die der
aktuellen Seite einen Inlineframe iframe mit der Oberfläche der SilverDAT 3 valuateExpert/PlusPartner hinzufügt. Beim Aufruf der Oberflächen-Schnittstelle müssen zusätzliche Parameter
übermittelt werden, Umfang und Inhalt der Angaben hängen von der gewählten Konstellation
ab. Mit diesen Parametern steuern Sie den Aufruf der SilverDAT 3 valuateExpert/PlusPartner und belegen die Datenfelder vor.

Abbildung : Beispiel für die Integration in eine herkömmliche HTML-Seite

Beim Aufruf der Oberflächen-Schnittstelle wird abhängig von den gewählten Vorgaben
die entsprechende Seite mit den zugehörigen Daten angezeigt. Ganz oben auf der Seite
finden Sie die Menüleiste mit den Steuerungselementen zur Navigation.

Abbildung : Beispiel für eine vollständig aufgeklappte Menüleiste

Die Menüleiste klappen Sie auf, indem Sie links oben auf den Pfeil  mit dem Prozessnamen klicken. Sie navigieren innerhalb des aktuellen Workflows, indem
Sie entweder auf einen der  Pfeile oder direkt auf eine Zielseite in der Workflow-Leiste klicken.  Sie wechseln zu einem anderen Prozess, indem Sie das entsprechende Piktogramm des
Prozesses in der vollständig aufgeklappten Menüleiste aktivieren. Zur LandingPage
gelangen Sie indem Sie auf den  Home-Button klicken. Sie speichern ihre Eingaben, indem Sie auf die Aktion  klicken. Zum Beenden der Anwendung klicken Sie auf den  Beenden-Button. Beim Verlassen über den Beenden-Button wird der Fremdanwendung der
gesamte Vorgang als Dossier VXS zur Verfügung gestellt. Die Fremdanwendung kann diese Daten anschließend verarbeiten,
die SilverDAT 3 valuateExpert/PlusPartner schließen und eigene Inhalte in der Seite zur Anzeige bringen oder die Seite komplett
verlassen.
