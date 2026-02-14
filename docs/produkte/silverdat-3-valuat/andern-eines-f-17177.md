---
title: "Ändern eines freien Aktenzeichens"
topic_id: "17177"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Freies Aktenzeichen > Verwalten von freien Aktenzeichen > Ändern eines freien Aktenzeichens"
---

# Ändern eines freien Aktenzeichens

Mit der Funktion changeDossierN ändern Sie ein bestehendes freies Aktenzeichen. Das freie Aktenzeichen kann dann über
den Parameter IsDiesengagedN mit dem Wert true in der Response erkannt werden. Dieser befindet sich unter dem Body Element Vehicle.

Ebenso kann mit der Funktion changeDossierN ein normales Aktenzeichen in ein freies Aktenzeichen umgewandelt werden. Dazu setzen
Sie den Parameter IsDisengaged auf true.

Momentan stehen die Datenländer Bulgarien, China, Deutschland, Frankreich, Griechenland,
Italien, Niederlande, Österreich, Rumänien, Schweiz, Slowakei, Spanien, Tschechische
Republik, Türkei und Ungarn für die Bewertung zur Verfügung. Derzeit können Sie als
Sprache bulgarisch, chinesisch, deutsch, englisch, französisch, griechisch, italienisch,
niederländisch, polnisch, rumänisch, russisch, slowakisch, spanisch, tschechisch,
türkisch und ungarisch auswählen. Bitte beachten Sie, dass gegenwärtig nur bestimmte
Kombinationen aus Datenland und Sprache möglich sind.

Der Nutzer kann die Zuordnung der Ausstattungen frei wählen.

Der Nutzer kann beliebige verfügbare, sowie frei definierte Fahrzeugtypen, Herstellertypen,
Serien- oder Sonderausstattung hinzufügen.

Es findet weder eine Prüfung noch eine Korrektur durch die Ausstattungslogik statt.

Bei der Umwandlung zum freien Aktenzeichen werden (falls bereits im Aktenzeichen bei
der Umwandlung vorhanden) folgende Daten in das freie Aktenzeichen übernommen und
nach einer Änderung der Fahrzeugidentifikation im freien Aktenzeichen nicht mehr automatisch
erneuert beziehungsweise aktualisiert:

- Fahrzeugidentifikation (nur Bezeichnungen)
- Halterdaten
- Listenneupreis
- Basiswert
- Wertbeeinflussende Faktoren
- Vorhanden Serien-/Sonderausstattungen inklusive Abwertung jedoch ohne Neupreis
- Vorhandene Zusatzausstattungen inklusive Neupreis und Abwertung
- Zustandsabhängige Daten
- Instandsetzungskosten

Arbeitsweise

1. Das Fahrzeug kann frei definiert werden.
2. Das Fahrzeug wird entsprechend den Benutzervorgaben bewertet und die Änderungen werden
   gespeichert.
3. Die Vorgangsdaten werden als VXS Datenstruktur zurückgegeben.

Eingabedaten

Es werden nur die nachfolgend beschriebenen Parameter unterstützt, alle anderen werden
ignoriert.

Für die Parameter wurden folgende Namespace-Definitionen festgelegt:

xmlns:dos="http://sphinx.dat.de/services/Dossier1N

xmlns:vxs="http://www.dat.de/vxs"

Rückgabe

Im Erfolgsfall wird der Vorgang als VXS zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben. Die Beschreibung
der Response-Elemente finden Sie im Kapitel VXS.
