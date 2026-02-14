---
title: "Aufbereitung der Eingabeparameter"
topic_id: "15257"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Integration der Oberfläche > Aufruf der Oberfläche > Aufbereitung der Eingabeparameter"
---

# Aufbereitung der Eingabeparameter

Alle Vorgaben für den Aufruf der Oberflächen-Schnittstelle der SilverDAT 3 valuateFinance setzen Sie mit den Eigenschaften und Funktionen des sphinx Objekts. Bitte beachten Sie, dass die nachfolgend beschriebenen Optionen aufgrund
der jeweiligen Berechtigungen oder Systemeinstellungen eingeschränkt oder nicht vorhanden
sein können. Bitte geben Sie die Basis-URL der SilverDAT 3 valuateFinance mit der Funktion sphinx.setProductUrl an. Für die Kommunikation mit der aufrufenden Anwendung benötigt der Client den Endpunkt
ihrer Server-Anwendung. Bitte geben Sie den entsprechenden Endpunkt mit der Funktion
sphinx.hostUrl an. Der verwendete Inlineframe iframe benötigt einen Namen, damit man diesen in JavaScript referenzieren kann, bitte setzen
Sie den Namen des iframe mit der Funktion sphinx.setIframeName. Um mit SilverDAT 3 valuateFinance arbeiten zu können, muss man sich anmelden, bitte setzen Sie die Anmeldedaten mit
der Funktion sphinx.credentials. Die Beschreibung hierzu finden Sie unter [Aufbereitung der Authentifizierungsinformationen](aufbereitung-d-2244.md).

Ein einfaches Beispiel zum Generieren des JSON Web Tokens sieht wie folgt aus:

```
            payload: JSON.stringify( {
                action: "generateToken",
                customerNumber: "9999999",
                user: "myLogin",
                password: "password"
                interfacePartnerNumber : "9999999",
                interfacePartnerSignature : "jA0EAwMCJ..."
                } )
```

Ein einfaches Beispiel zur Übergabe des Tokens sieht wie folgt aus:

```
            sphinx.credentials = {
                token: token
            };
```

Mit der Eigenschaft sphinx.params stellen Sie die spezifischen Vorgaben der SilverDAT 3 valuateFinance ein. Über den Parameter action steuern Sie den Aktionstyp. Die Oberflächen-Schnittstelle der SilverDAT 3 valuateFinance kann grundsätzlich in vier verschiedenen Aktionytypen action aufgerufen werden.

Übersicht der Aktionen

| Aktion | Beschreibung | Abhängigkeit zu |
| --- | --- | --- |
| showEventList | Anzeigen der Vorgangsübersicht |  |
| createDossier | Neuen Vorgang anlegen | Nur für die Vorgangsarten type: evaluation, historical evaluation und compare zulässig |
| changeDossier | Bestehenden Vorgang ändern | Vorgangskennung dossierid,  [Aufrufziel](aufrufziele-2246.md) page Nur für die Vorgangsarten type: evaluation, historical evaluation und compare zulässig |
| importDossier | Vorgang importieren und anzeigen | Vorgangsdaten vxs  [Aufrufziel](aufrufziele-2246.md) page Nur für die Vorgangsarten type: evaluation, historical evaluation und compare zulässig |

Übersicht der Übergabeparameter

| Parameter | Beschreibung | Abhängigkeit zu | Pflicht |
| --- | --- | --- | --- |
| datCountryIndicator | Mit dem Parameter datCountryIndicator stellen Sie den gewünschten Zielmarkt, zum Beispiel "DE" ein | kbaNumber nationalCodeAustria | X |
| locale | Mit dem Parameter locale wählen Sie das Sprachkürzel (Language) aus, zum Beispiel "de\_DE" |  | X |
| action | Über den Parameter action steuern Sie den Arbeitsmodus. |  | X |
| dossierid | Den Wert für die Vorgangskennung dossierid benötigen Sie, wenn Sie einen bestehenden Vorgang öffnen möchten | Nur für Aktionstyp changeDossier zulässig | Pflicht für Aktionstyp changeDossier |
| type | Den Vorgangstyp type benötigen Sie, wenn Sie einen Vorgang neu anlegen möchten. Die folgenden Vorgangstypen sind möglich: evaluation - Bewertung historical evaluation - stichtagsbezogene Bewertung compare - Vergleich | Nur für Aktionstyp createDossier zulässig | Pflicht für Aktionstyp createDossier |
| vxs | Die Vorgangsdaten vxs benötigen Sie, wenn Sie einen neuen Vorgang importieren möchten. | Nur für Aktionstyp importDossier zulässig | Pflicht für Aktionstyp importDossier |
| page | Das Aufrufziel page legt die aufzurufende Seite der SilverDAT 3 valuateFinance Oberfläche fest. Die möglichen Aufrufziele sind vom Aktionstyp action, dem Typ des anzulegenden Vorgangs DossierType, der Fahrzeugart VehicleType und der Bewertungsart ValuationType abhängig.  Bei der Aktion createDossier wird unabhängig von der Vorgabe in page die Modelseite model page aufgerufen, falls das Fahrzeug nicht vollständig identifiziert wurde. | Nur für die Aktionstypen:  createDossier, changeDossier und importDossier | Pflicht für die Aktionstypen: createDossier, changeDossier und importDossier |
| pageList | Falls Sie beim Aufruf der Oberflächen-Schnittstelle die für den Benutzer zugänglichen Seiten einschränken möchten, dann können Sie dies mit dem Paramter pageList vorgeben. Die gewünschten Seiten tragen Sie als kommaseparierte Liste ein. Bitte beachten Sie bei Verwendung der Seitenliste die in Aufruf der Oberfläche beschriebenen Bedingungen. Bei der Aktion createDossier muss bei Verwendung der Seitenliste die Modelseite model page enthalten sein. Keine Vorgabe bedeutet, dass alle möglichen Seiten auch zugänglich sind.  Beispiel: model selection,equipment selection,evaluation | Der Wert von [Aufrufziel](aufrufziele-2246.md) page muss in pageList enthalten sein Nur zulässig, falls workflow=true ist Nur für die Aktionstypen: createDossier, importDossier und changeDossier zulässig |  |
| vehicleIdentNumber | Mit dem Wert von vehicleIdentNumber belegen Sie das Eingabefeld VIN der Modell-Maske vor. Format: String Beispiel: WAUDEXTESTSTUB001 | Nur für Aktionstyp createDossier zulässig |  |
| vehicleIdentNumberRequest | Falls Sie den Parameter vehicleIdentNumberRequest=true setzen lösen Sie die VIN-Abfrage aus. Der Parameter vehicleIdentNumber muss in diesem Fall korrekt vorbelegt sein. Format: boolean | VIN vehicleIdentNumber Nur für Aktionstyp createDossier zulässig |  |
| name | Mit dem Wert von name belegen Sie das Eingabefeld Vorgangsname der Auftragseröffnungsmaske vor. Format: String |  |  |
| initialRegistration | Mit dem Wert von initialRegistration belegen Sie das Eingabefeld Erstzulassung der Modell-Maske vor. Format: JJJJ-MM-DD Beispiel: 2020-07-10 | Nur für Aktionstyp createDossier zulässig |  |
| mileageEstimated | Mit dem Wert von mileageEstimated belegen Sie das Eingabefeld Laufleistung der Modell-Maske vor. Format: Zahl, Beispiel: 90000 | Nur für Aktionstyp createDossier zulässig |  |
| kbaNumber | Mit dem Wert von kbaNumber belegen Sie das Eingabefeld KBA der Modell-Maske vor. Format: HSN/TSN,  Beispiel: 0588/AHZ | Nur für Datenland DE zulässig. Nur für Aktionstyp createDossier zulässig |  |
| nationalCodeAustria | Mit dem Wert von nationalCodeAustria belegen Sie das Eingabefeld Nationaler Code (A7) der Modell-Maske vor. Beispiel: 162288 | Nur für Datenland AT zulässig Nur für Aktionstyp createDossier zulässig |  |
| datECode | Mit dem Wert von datECode belegen Sie das Eingabefeld DAT €uropa-Code® der Modell-Maske vor. Beispiel: 010600370430004 | Nur für Aktionstyp createDossier zulässig |  |
| container | Mit dem Wert von container belegen Sie das Eingabefeld Marktindex der Modell-Maske vor.  Beispiel: DE003 | Nur für Aktionstyp createDossier zulässig |  |
| constructionTime | Mit dem Wert von constructionTime belegen Sie das Eingabefeld Bauzeit der Modell-Maske vor.  Beispiel: 5050 | Nur bei Aktionstyp createDossier zulässig |  |
| workflow | Wenn Sie den Parameter workflow mit true vorbelegen, dann darf der Anwender durch die Anwendung navigieren, falls Sie false setzen, dann darf er die vorgegebene Seite nicht verlassen.  Defaultwert = true | pageList |  |
| save | Mit dem Parameter save bestimmen Sie, ob der Anwender den Vorgang speichern darf true, oder aber nicht verändern kann false.  Defaultwert = true |  |  |
| readOnly | Mit dem Parameter readOnly bestimmen Sie, ob der Vorgang im Lesemodus geöffnet wird.  Diese Aktion ist nur beim Aufruf eines bestehenden Vorgangs zulässig. Es wird nur die vorgegebene Aufrufseite page angezeigt. Die Eigenschaften workflow und save müssen auf false gesetzt sein. Defaultwert = false | page save workflow |  |

Ein einfaches Beispiel sieht wie folgt aus:

```
            sphinx.params = {
                datCountryIndicator : "DE",
                locale : "de_DE",
                action : "createDossier",
                dossierid : "",
                type : "evaluation",
                vxs : "",
                page : "model selection",
                pageList : "model selection,equipment selection,evaluation",
                vehicleIdentNumber : "WAUDEXTESTSTUB001",
                vehicleIdentNumberRequest : "false",
                initialRegistration : "2008-12-18",
                mileageEstimated : "184000",
                kbaNumber : "0588/ADU",
                nationalCodeAustria : "",
                datECode : "010600370430004",
                container : "DE001",
                constructionTime : "4495",
                workflow : "true",
                save : "true"
            };
```

Nachfolgend noch ein Beispiel für den Parameter readOnly:

```
                sphinx.params = {
                datCountryIndicator : "DE",
                locale : "de_DE",
                action : "changeDossier",
                dossierid : "12345678",
                page : "evaluation",
                readOnly : "true",
                workflow : "false",
                save : "false"
            };
```

Nachfolgend noch ein Beispiel für den Parameter nationalcode:

```
                sphinx.params = {
                datCountryIndicator : "AT",
                locale : "de_AT",
                action : "createDossier",
                dossierid : "",
                type : "evaluation",
                vxs : "",
                page : "model selection",
                pageList : "model selection,equipment selection,evaluation",
                initialRegistration : "2008-12-18",
                mileageEstimated : "184000",
                nationalCodeAustria : "181429",
                datECode : "010600370430004",
                container : "AT003",
                constructionTime : "5045",
                workflow : "true",
                save : "true"
            };
```

Mit der Funktion sendDossierRequest rufen Sie Oberfläche der SilverDAT 3 valuateFinance mit den vorgegebenen Parametern auf. Ein einfaches Beispiel sieht wie folgt aus:

```
sphinx.sendDossierRequest();
```

Ein einfaches VXS-Beispiel für importDossier sieht wie folgt aus:

```
vxs : "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"yes\"?>
<ns2:Dossiers xmlns:ns2=\"http://www.dat.de/vxs\" source=\"SD3\" type=\"completeEvaluation\">
    <ns2:Dossier>
        <ns2:Name>POST import sample</ns2:Name>
        <ns2:UUID>48251edb-a4c6-4ad9-8cd8-59488a5df51f</ns2:UUID>
        <ns2:DossierId>47337</ns2:DossierId>
        <ns2:IdSD3Network>47337</ns2:IdSD3Network>
        <ns2:Country>DE</ns2:Country>
        <ns2:Language>DE_de</ns2:Language>
        <ns2:DataVersion>1</ns2:DataVersion>
        <ns2:DatCustomerId>1000000</ns2:DatCustomerId>
        <ns2:DossierType>evaluation</ns2:DossierType>
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
                <ns2:DatEquipmentValue>277.32</ns2:DatEquipmentValue>
                <ns2:DatEquipmentValueGross>330.01</ns2:DatEquipmentValueGross>
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
        <ns2:VAT>
            <ns2:VatType>difference</ns2:VatType>
            <ns2:VatAtConstructionTime origin=\"dat\">19</ns2:VatAtConstructionTime>
            <ns2:BaseVatAtConstructionTime origin=\"dat\">19</ns2:BaseVatAtConstructionTime>
            <ns2:AddOnTaxApplication>before vat</ns2:AddOnTaxApplication>
            <ns2:VatAtValuationTime origin=\"dat\">19</ns2:VatAtValuationTime>
        </ns2:VAT>
        <ns2:Valuation>
        </ns2:Valuation>
    </ns2:Dossier>
</ns2:Dossiers>"
```
