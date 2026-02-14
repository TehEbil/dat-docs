---
title: "Anlegen und ändern eines unvollständigen Aktenzeichens mit der Oberflächenintegration"
topic_id: "15497"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Integration der Oberfläche > Aufruf der Methoden von SilverDAT 3 valuateExpert Oberflächeintegration > Anlegen und ändern eines unvollständigen Aktenzeichens mit der Oberflächenintegration"
---

# Anlegen und ändern eines unvollständigen Aktenzeichens mit der Oberflächenintegration

Bei einem unvollständigem Aktenzeichen handelt es sich um einen Vorgang, der kein
vollständig identifiziertes Fahrzeug für die Bewertung beinhaltet.

Hinweis:Falls Sie die VIN-Abfrage durchführen und nicht regulär zurückspringen zur
Schnittstellenanwendung, sei es weil die Verbindung abreißt oder Sie den Vorgang abbrechen,
bleibt das Aktenzeichen erhalten.

Folgende Parameter müssen nicht angegeben werden: DatEcode, Container, ConstrutionTime, Mileage, InitialRegistration und Country unter dem Body Vehicle.

Im unvollständigen Aktenzeichen können auch Zustandsparameter übergeben werden. z.B.
NumberOfOwnersN, AccidentDamage. Siehe Kapitel [Condition](#showid/1750 "Zustand (Condition)").

Rückgabe

Ein Vorgang, der kein vollständiges Fahrzeug beinhaltet.

Beispiel

```
                valuateNGExternal.setLocale( "de_DE" );
                valuateNGExternal.setCountry( "DE" );
                valuateNGExternal.setDossierId( "721243" );
                valuateNGExternal.setDossier( "" );
                valuateNGExternal.setStartPage( "valuation.model" );
                valuateNGExternal.setPageList( "" );
                valuateNGExternal.setDatGroupHeader( "true" );
                valuateNGExternal.setWorkflow( "true" );
                valuateNGExternal.setProcesses( "true" );
                valuateNGExternal.setSave( "true" );
                valuateNGExternal.setMode( "" );
                valuateNGExternal.setFlapVisible("false");
```
