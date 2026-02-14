---
title: "Definition abgerufen - abgeschlossen - versendet"
topic_id: "2094"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Grundlagenwissen > Definition abgerufen - abgeschlossen - versendet"
---

# Definition abgerufen - abgeschlossen - versendet

| Oberflächensymbol | Terminologie | Erklärung |
| --- | --- | --- |
|  | abgerufene Kalkulation | Hier handelt es sich um Kalkulationen, die über eine der Schnittstellen-Funktionen schon einmal abgerufen worden sind. Das Abrufen von Kalkulationen über eine Schnittstellen-Funktion ist - bislang - nur ein einziges Mal erlaubt. Da es sich hier um sensible Rechnungsdaten handelt, wurde dieser Service so eingerichtet. Es ist nicht über die Oberfläche erkennbar, welche Kalkulation schon über die Schnittstellen-Funktion abgerufen worden ist, da es für die Oberfläche nicht von Belang ist. Wird also die getNewContractNumbers() aufrufen und es werden keine Werte zurückgegeben, wurden alle angelegten Kalkulationen schon einmal abgerufen. |
|  | abgeschlossene Kalkulation | Dies sind Vorgänge, bei denen eine Kalkulation vorgenommen wurde. Dies sagt noch nichts darüber aus, ob sie auch schon versendet worden ist. Es sind aber Kalkulationen vorhanden. Im Gegensatz zu einem Vorgang, der einfach nur angelegt worden ist. Dieser muss noch keine Kalkulation enthalten. Abgeschlossene Kalkulationen können noch bearbeitet werden, dies ist erkennbar am entsprechenden Edit-Icon. |
|  | versendete Kalkulation | Diese Kalkulationen sind an die entsprechende Versicherung weitergeleitet worden und können nicht mehr bearbeitet werden. Allerdings können die Rechnungsanhänge heruntergeladen und angesehen werden. Da es sich bei den versendeten Kalkulationen nicht um Vorab-Kalkulationen, sondern Rechnungen handelt, ist dies eine sicherheitsrelevante, notwendige Maßnahme. Bei versendeten Kalkulationen entfällt das Edit-Icon und ein Icon für die Anhänge erscheint in der Spalte rechts daneben. |
