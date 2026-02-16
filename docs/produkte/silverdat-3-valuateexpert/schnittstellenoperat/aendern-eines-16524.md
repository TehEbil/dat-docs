---
title: "Aendern eines unvollstaendigen Aktenzeichens"
topic_id: "16524"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Unvollständiges Aktenzeichen > Verwalten von unvollstaendigen Aktenzeichen > Aendern eines unvollstaendigen Aktenzeichens"
---

# Aendern eines unvollstaendigen Aktenzeichens

Die Funktion changeDossierN unterstützt die Variante mit unvollständiger Fahrzeugidentifikation. In diesem Fall
ändern Sie den Vorgang, ohne das Fahrzeug vollständig zu definieren. Das unvollständige
Aktenzeichen ist an dem Wert incompleteValuation im Attribut type des Elements VXS zu erkennen.

Voraussetzungen

- Der zu ändernde Vorgang muss ein unvollständiges Aktenzeichen sein.
- Das Element Coverage muss gesetzt sein und den Wert NOVALUATIONRESULT oder NONE enthalten
- Um das unvollständige Aktenzeichen beizubehalten, darf der Request keine oder nur
  eine unvollständige Fahrzeugidentifikation enthalten.

Details

Beim unvollständigen Aktenzeichen müssen immer alle Parameter erneut übergeben werden.
Ein Hinzufügen zu bestehenden Werten ist in diesem Fall nicht möglich. Wird das Fahrzeug
vollständig definiert, wird es automatisch in ein normales Aktenzeichen umgewandelt.
Es ist danach nicht mehr möglich den Vorgang wieder in ein unvollständiges Aktenzeichen
umzuwandeln.

Eingabedaten

Es werden nur die nachfolgend beschriebenen Parameter unterstützt, alle anderen werden
ignoriert.

Rückgabe

Im Erfolgsfall wird der Vorgang als VXS zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben. Die Beschreibung
der Response-Elemente finden Sie im Kapitel VXS.
