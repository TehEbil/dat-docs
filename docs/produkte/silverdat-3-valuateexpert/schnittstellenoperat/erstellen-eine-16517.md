---
title: "Erstellen eines neuen unvollstaendigen Aktenzeichens"
topic_id: "16517"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Unvollständiges Aktenzeichen > Verwalten von unvollstaendigen Aktenzeichen > Erstellen eines neuen unvollstaendigen Aktenzeichens"
---

# Erstellen eines neuen unvollstaendigen Aktenzeichens

Die Funktion createDossierN unterstützt die Variante mit unvollständiger Fahrzeugidentifikation. Bei dieser Variante
erstellen Sie einen neuen Vorgang in der Anwendung, ohne vorher das Fahrzeug eindeutig
zu identifizieren.

Voraussetzungen:

- Das Element Coverage muss gesetzt sein und den Wert NOVALUATIONRESULT oder NONE enthalten.
- Der Request darf keine oder nur eine unvollständige Fahrzeugidentifikation enthalten.

Arbeitsweise

1. Der Vorgang kann mit fehlenden Fahrzeugdaten angelegt werden.
2. Der Vorgang wird angelegt und gespeichert.
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
