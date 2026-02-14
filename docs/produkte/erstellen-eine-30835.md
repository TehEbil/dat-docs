---
title: "Erstellen eines freien Aktenzeichens im Speicher"
topic_id: "30835"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Freies Aktenzeichen > Verwalten von freien Aktenzeichen > Erstellen eines freien Aktenzeichens im Speicher"
---

# Erstellen eines freien Aktenzeichens im Speicher

###### Erstellen eines freien Aktenzeichens im Speicher Mit der Funktion doValuationInMemoryN erstellen Sie eine neue Bewertung für ein freies Aktenzeichen im Speicher, indem Sie den Parameter IsDisengagedN auf true setzen. Der Parameter IsDisengagedN befindet sich unter dem Body Element Vehicle. Der Nutzer kann die Zuordnung der Ausstattungen frei wählen. Der Nutzer kann beliebige verfügbare, sowie frei definierte Fahrzeugtypen, Herstellertypen, Serien- oder Sonderausstattung hinzufügen. Es findet weder eine Prüfung noch eine Korrektur durch die Ausstattungslogik statt. Arbeitsweise 1. Das Fahrzeug kann frei definiert werden. 2. Das Fahrzeug wird entsprechend den Benutzervorgaben bewertet 3. Die Vorgangsdaten werden als VXS Datenstruktur zurückgegeben. Eingabedaten Es werden nur die nachfolgend beschriebenen Parameter unterstützt, alle anderen werden ignoriert. Für die Parameter wurden folgende Namespace-Definitionen festgelegt: xmlns:val="http://www.dat.eu/myClaim/soap/v2/ValuationServiceN" xmlns:vxs="http://www.dat.de/vxs" Rückgabe Im Erfolgsfall wird der Vorgang als VXS zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben. Die Beschreibung der Response-Elemente finden Sie im Kapitel VXS.
