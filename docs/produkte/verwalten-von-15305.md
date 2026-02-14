---
title: "Verwalten von freien Aktenzeichen"
topic_id: "15305"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Freies Aktenzeichen > Verwalten von freien Aktenzeichen"
---

# Verwalten von freien Aktenzeichen

Das freie Aktenzeichen ermöglicht Ihnen Fahrzeuge über die DAT-Schnittstellen zu bewerten,
für die die DAT keine Bewertungsdaten anbietet. In diesem Fall stellt die Anwendung
die verfügbaren Grunddaten zur Verfügung. Um eine manuelle Bewertung zu erstellen
müssen Sie noch die Grunddaten entsprechend ergänzen. Hierfür müssen Sie die fehlenden
Daten über die Schnittstelle übergeben.

Anlage eines freien Aktenzeichens

Bei der Anlage eines freien Aktenzeichens können Sie grundsätzlich zwischen zwei verschiedenen
Abläufen wählen:

1. Sie bewerten zuerst ein vergleichbares Fahrzeug mit der Funktion createDossierN und schalten mit der Funktion changeDossierN auf das freie Aktenzeichen um.

2. Sie legen direkt ein freies Aktenzeichen mit createDossierN an.

Kennzeichen Freies Aktenzeichen

Sie legen ein freies Aktenzeichen an, indem Sie das Element isDisengagedN auf true setzen.

Mode-Umschaltung zum freien Aktenzeichen

Die Umwandlung eines Vorgangs in ein freies Aktenzeichen ist unumkehrbar. Falls dies
mittels changeDossierN versucht wird, wird eine Fehlermeldung zurückgegeben.

Modellmaske

Der nachfolgende Screenshot zeigt die Modellmaske eines Vorgangs der mittels der Funktion
createDossierN im Mode Freies Aktenzeichen angelegt wurde. In diesem Fall wird zur Anlage eines Vorgangs
kein DAT €uropa-Code® benötigt. Die Beschreibungsfelder der Fahrzeugauswahl können hierbei mit eigenen
Werten überschrieben werden. Die Laufleistung können Sie in Kilometer, Meilen oder
Arbeitsstunden angeben.
