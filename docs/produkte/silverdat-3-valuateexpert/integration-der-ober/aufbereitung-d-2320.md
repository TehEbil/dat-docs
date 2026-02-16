---
title: "Aufbereitung der Eingabeparameter"
topic_id: "2320"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Integration der Oberfläche > Aufruf der Methoden von SilverDAT 3 valuateExpert Oberflächeintegration > Aufbereitung der Eingabeparameter"
---

# Aufbereitung der Eingabeparameter

Alle benötigten Vorgaben für den Aufruf der Oberflächen-Schnittstelle der SilverDAT 3 valuateExpert/PlusPartner setzen Sie mit den valuateNGExternal Objektfunktionen. Bitte beachten Sie, dass die nachfolgend beschriebenen Parameter
aufgrund der jeweiligen Berechtigungen und Systemeinstellungen eingeschränkt oder
auch nicht verfügbar sein können.

Der Client benötigt für die Kommunikation mit der aufrufenden Anwendung den Endpunkt
ihrer Server-Anwendung. Bitte geben Sie den entsprechenden Endpunkt mit der Methode
setExternalUrl an. Der verwendete Inlineframe iframe benötigt einen Namen, damit man diesen in JavaScript referenzieren kann, bitte setzen Sie den Namen des iframe mit der Methode setIframeName. Um mit SilverDAT 3 valuateExpert/PlusPartner arbeiten zu können, muss man sich zuerst anmelden. Sie können sich entweder mit einer
gültigen SessionID des Authentication-Services oder mittels der JSON Web Token Authentifikation anmelden.
Die Anmeldung mittels JSON Web Token erfolgt entsprechend der Anmeldung bei den Soap-Funktionen
zweistufig mittels der JSON Web Token Authentifikation. Im ersten Schritt erstellen
Sie das Token mittels der Funktion JSON.stringify und im zweiten Schritt melden Sie sich mittels der Funktion sphinx.credentials an. Das DAT-AuthorizationToken hat eine Gültigkeit von 30 Minuten. Die Beschreibung
hierzu finden Sie unter [Aufbereitung der Authentifizierungsinformationen](aufbereitung-d-2322.md). Ein einfaches Beispiel zur Übergabe des Tokens sieht wie folgt aus:

```
            valuateNGExternal.setToken(token)
            valuateNGExternal.setProductVariant( "valuateNG.expert" );
```

Für den Aufruf muss man noch den gewünschten Zielmarkt einstellen, diesen setzen Sie
mit der Methode setCountry, zum Beispiel "DE". Ebenfalls muss noch die Oberflächensprache - das Sprachkürzel (Language) mit der Methode setLocale eingestellt werden. Diese Vorgabe verhält sich entsprechend der Sprachumschaltung
in der Oberfläche. Mit der Methode setStartPage bestimmen Sie das Aufrufziel. Diese Angabe ist der wichtigste Parameter zur Steuerung
der Oberflächen-Schnittstelle, je nach Vorgabe sind unterschiedliche Aktionen und
Seitenaufrufe möglich. Bitte beachten Sie hierbei die umfangreichen Abhängigkeiten,
die zugehörige Beschreibung finden Sie unter Aufrufziele. Die möglichen Aufrufziele sind unter anderem abhängig von der PageList, den VXS Vorgangsdaten beziehungsweise der eindeutigen Vorgangskennung DossierId, der Fahrzeugart und den Einstellungen der Berechtigungen der betreffenden Benutzergruppe in der Systemkonfiguration.
Damit sind die Mindestanforderungen für einen einfachen Aufruf erfüllt.

Wenn Sie einen bestehenden Vorgang öffnen möchten, dann müssen Sie den Vorgang mit
der Methode setDossierId definieren. In diesem Fall muss der Wert für Dossier leer bleiben. Wenn Sie beim Aufruf direkt in eine bestimmte Bearbeitungsseite springen
möchten, aber die zugehörigen Daten erst mit dem Aufruf importieren möchten, dann
müssen Sie diese mit der Methode setDossier angeben. Der Wert für DossierId muss in diesem Falle leer bleiben.

Ein einfaches Beispiel für setDossierId sieht wie folgt aus:

```
                valuateNGExternal.setDossierId( "99999" );
                valuateNGExternal.setDossier( "" );
                valuateNGExternal.setStartPage( "valuation.contractOpening" );
```

Ein einfaches Beispiel für setDossier sieht wie folgt aus:

```
valuateNGExternal.setDossier( "<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<ns2:Dossiers xmlns:ns2="http://www.dat.de/vxs" source="SD3" type="completeEvaluation">
   <ns2:Dossier>
      <ns2:Name>Dossier import sample</ns2:Name>
      <ns2:Country>DE</ns2:Country>
        <ns2:Language>DE_de</ns2:Language>
        <ns2:Vehicle>
            <ns2:VehicleIdentNumber>12345678901234567</ns2:VehicleIdentNumber>
            <ns2:DatECode>012850950160006</ns2:DatECode>
            <ns2:Container>DE004</ns2:Container>
            <ns2:ConstructionTime>5123</ns2:ConstructionTime>
            <ns2:InitialRegistration>2012-08-12+02:00</ns2:InitialRegistration>
            <ns2:MileageEstimated>43000</ns2:MileageEstimated>
            <ns2:MileageOdometer>43000</ns2:MileageOdometer>
            <ns2:Country>DE</ns2:Country>
            <ns2:Equipment>
                <ns2:SpecialEquipment>
                    <ns2:EquipmentPosition>
                        <ns2:DatEquipmentId>14200</ns2:DatEquipmentId>
                    </ns2:EquipmentPosition>
                    <ns2:EquipmentPosition>
                        <ns2:DatEquipmentId>16007</ns2:DatEquipmentId>
                    </ns2:EquipmentPosition>
                    <ns2:EquipmentPosition>
                        <ns2:DatEquipmentId>4900</ns2:DatEquipmentId>
                    </ns2:EquipmentPosition>
                    <ns2:EquipmentPosition>
                        <ns2:DatEquipmentId>2392</ns2:DatEquipmentId>
                    </ns2:EquipmentPosition>
                </ns2:SpecialEquipment>
            </ns2:Equipment>
        </ns2:Vehicle>
   </ns2:Dossier>
</ns2:Dossiers>" );
```

Falls Sie beim Aufruf der Oberflächen-Schnittstelle, die für den Benutzer zugänglichen
Seiten einschränken möchten, dann können Sie dies mit der Methode SetPageList vorgeben. Die gewünschten Seiten tragen Sie als kommaseparierte Liste ein. Bitte
beachten Sie bei Verwendung der Seitenliste, die in [Aufruf der Oberfläche](aufruf-der-met-2318.md) beschriebenen Bedingungen.

Ein einfaches Beispiel für SetPageList sieht wie folgt aus:

```
                valuateNGExternal.setLocale( "de_DE" );
                valuateNGExternal.setCountry( "DE" );
                valuateNGExternal.setDossierId( "99999" );
                valuateNGExternal.setStartPage( "valuation.condition" );
                valuateNGExternal.setPageList( "valuation.contractOpening,valuation.equipment,valuation.condition" );
```

Mit der Methode setWorkflow bestimmen Sie, ob der Anwender zu weiteren Seiten des aktuellen Prozesses navigieren
kann. Bitte beachten Sie, dass hierfür die Fahrzeugart VehicleType gesetzt werden muss. Falls Sie dies nicht zulassen möchten, dann setzen Sie Workflow auf "false". Mit der Methode setProcesses bestimmen Sie, ob der Anwender den Prozess wechseln darf. Diese Konfiguration ist
nur zulässig, wenn auch die Berechtigung für Workflow und Save gegeben sind. Bitte beachten Sie, dass nur die Prozesse verwendet werden können,
die in der Systemkonfiguration freigegeben sind. Mit der Methode setSave bestimmen Sie, ob die Änderungen im System gespeichert werden. Dies ist Pflicht,
falls Processes mit true angegeben ist.

Ein einfaches Beispiel hierfür sieht wie folgt aus:

```
                valuateNGExternal.setLocale( "de_DE" );
                valuateNGExternal.setCountry( "DE" );
                valuateNGExternal.setDossierId( "99999" );
                valuateNGExternal.setDossier( "" );
                valuateNGExternal.setStartPage( "valuation.model" );
                valuateNGExternal.setPageList( "" );
                valuateNGExternal.setWorkflow( "true" );
                valuateNGExternal.setProcesses( "true" );
                valuateNGExternal.setSave( "true" );
```

Mit der Methode setReadOnly bestimmen Sie, ob der Vorgang im Lesemode geöffnet wird. Bitte beachten Sie, dass
diese Aktion ist nur beim Aufruf eines bestehenden Vorgangs zulässig ist. Es wird
nur die vorgegebene Aufrufseite angezeigt. Die Eigenschaften setWorkflow, setProcesses und setSave müssen auf false gesetzt sein.

```
                valuateNGExternal.setDossierId( "99999" );
                valuateNGExternal.setDossier( "" );
                valuateNGExternal.setStartPage( "valuation.historyValuation" );
                valuateNGExternal.setPageList( "" );
                valuateNGExternal.setReadOnly("true");
                valuateNGExternal.setWorkflow( "false" );
                valuateNGExternal.setProcesses( "false" );
                valuateNGExternal.setSave( "false" );
```

Mit den Methoden setVehicleIdentNumber, setVehicleIdentNumberRequest, setInitialRegistration, setMileageEstimated,
setKbaNumber, setDatECode, setContainer und setConstructionTime belegen Sie entsprechenden Eingabefelder der Modell-Maske vor und führen die VIN-Abfrage
durch. Diese Funktionen sind nur in Kombination mit dem Aufrufziel valuation.create zulässig.

Ein einfaches Beispiel hierfür sieht wie folgt aus:

```
                valuateNGExternal.setVehicleIdentNumber("WAUDEXTESTSTUB001");
                valuateNGExternal.setVehicleIdentNumberRequest("true");
                valuateNGExternal.setInitialRegistration("2008-12-18");
                valuateNGExternal.setMileageEstimated("145000");
                valuateNGExternal.setKbaNumber("0588/ADU");
                valuateNGExternal.setDatECode("010600370430004");
                valuateNGExternal.setContainer("DE001");
                valuateNGExternal.setConstructionTime("4495");
```

Mit der Methode setFlapVisible blenden Sie die seitlichen Flaps der Benutzeroberfläche aus.

Ein einfaches Beispiel sieht wie folgt aus:

```
valuateNGExternal.setFlapVisible("false");
```

Mit der Methode execute rufen Sie Oberfläche der SilverDAT 3 valuateExpert/PlusPartner mit allen angegebenen Parametern auf.

Ein einfaches Beispiel sieht wie folgt aus:

```
valuateNGExternal.setOnLoginSuccess(valuateNGExternal.execute);
valuateNGExternal.login();
```
