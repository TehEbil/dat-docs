---
title: "Optionale Aufbereitung möglicher Eingabeparameter"
topic_id: "1856"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Oberflächen-Schnittstelle > Integration der Oberfläche > Optionale Aufbereitung möglicher Eingabeparameter"
---

# Optionale Aufbereitung möglicher Eingabeparameter

Mögliche Eingabeparameter sind:

- displayHeader - Über diesen Schalter (true / false) wird die Darstellung der DAT-Kopfzeile ein-
  bzw. ausgeschaltet.

- Restriction - Ein Filter der darüber entscheidet, welche Fahrzeuge in der Fahrzeugauswahl berücksichtigt
  werden. Die Möglichkeiten sind:

  - ALL (default) = Identifizierbar, nicht notwendigerweise auch für Bewertung oder Schadenskalkulation
    geeignet
  - REPAIR = In der Schadenskalkulation verwendbar
  - APPRAISAL = In der Gebrauchtwagenbewertung verwendbar
  - GLASS = In den Anwendungen der Glaskalkulation verwendbar

- noRestrictionInp - Über diesen Schalter (true / false) wird das Auswahl-Element für die Restriction
  ein- bzw. ausgeschaltet.

- CountryCode - Dieser Parameter wählt den Zielmarkt (Land) und entspricht dem datCountryIndicator
  aus den Schnittstellenfunktionen. Allerdings mit dem Unterschied, dass dieser nach
  ISO 3166 ALPHA-2 codiert ist, während der CountryCode der Notierung der Kfz-Nationalitätszeichen
  folgt. Beispielsweise für Österreich der CountryCode "A".

- DatECode - Der DAT €uropa-Code®, 15-stellig, in der Form:

  Fahrzeugart + Hersteller + Haupttyp + Untertyp + Untertypvariante

  Alternativ kann der DAT €uropa-Code® auch gesplittet mit seinen einzelnen Elementen
  übergeben werden. Siehe dazu die nachfolgenden Eingabeparameter VehicleType, Manufacturer, BaseModel, SubModel und SubModelVariant.

- VehicleType - Angabe der Fahrzeugart (numerisch, 2 Stellen)
- Manufacturer - Angabe des Herstellers, bzw. der Marke (numerisch, 3 Stellen)
- BaseModel - Angabe des Haupttyps (numerisch, 3 Stellen)
- SubModel - Angabe des Untertyps (numerisch, 3 Stellen)
- SubModelVariant - Angabe der Untertypvariante (numerisch, 4 Stellen)

- Container - Der Marktindex (DAT-Container) bestehend aus 5 Zeichen, z. Bsp. DE004

- VehicleIdentNumber - Fahrzeugidentifikationsnummer, 17 Zeichen, bspw. WP0AA298X8U760141

- KbaCode - KBA-Schlüssel, 8 Zeichen, z. Bsp. 3436/ACP

- natCode - Nur für Österreich! Angabe des österreichischen-Nationalcodes (NatCode), z. Bsp.
  162288

- licencePlate - Nur für Italien und die Schweiz! Amtliches Kennzeichen für die Kennzeichenabfrage.
- baseNumber - Nur für die Schweiz! Angabe der Stammnummer, bspw. 136.936.153r
- typeNoteNumber - Nur für die Schweiz! Angabe der Typenscheinnummer, bspw. 1LC582

- InitialRegistration - Erstzulassung in Millisekunden seit dem 1.1.1970, bspw. 1185962400000

- mileage - Laufleistung in km

- equFilter - Ein Filter, der den Umfang der Ausstattungen bestimmt, die angezeigt werden. Die
  Möglichkeiten sind:

  - ALL (default) = Alle Ausstattungen werden angezeigt
  - GENERAL = Allgemeine Ausstattungen werden angezeigt
  - EXTERIOR = Ausstattungen im Bereich "Außen" werden angezeigt
  - INTERIOR = Ausstattungen im Bereich "Innen" werden angezeigt
  - CHASSIS = Ausstattungen im Bereich Fahrwerk werden angezeigt
  - AGGREGATE = Ausstattungen im Bereich Aggregat werden angezeigt
  - GLASS = Ausstattungen im Bereich Glas werden angezeigt
- equDatNr - Angabe einer Liste von fahrzeugspezifischen DAT-Ausstattungs-Nummern, jeweils mit
  Komma getrennt. Die Zuordnung (Sonder / Serie) geschieht automatisch.  
  ACHTUNG: Für die Übergabe von Ausstattungen muss zusätzlich der Parameter InitialRegistration (Erstzulassung) gesetzt sein.
- equAdd - Angabe einer Liste von Zusatzausstattungen, jeweils mit Komma getrennt, z. Bsp.
  Zusatzscheinwerfer, Standheizung
- withSaveAsEvent - Über diesen Schalter (true / false) kann eingestellt werden ob an Ende des Pageflows
  die getätigte Fahrzeugidentifikation in der Datenbank gespeichert werden soll. Als
  Referenz wird die DossierId verwendet. Diese wird dann im zurückgelieferten VXS angegeben.
- eventName - Name des Speichern-Events. Wenn kein eigenes Event definiert werden soll, muss
  hier 'from external' angegeben werden.
- az - Dieser Parameter entspricht der DossierId, die eindeutige Referenz eines Vorgangs
  (in unserem Fall eine Fahrzeugidentifikation). Bei einer Übergabe dieses Parameters
  wird, sofern vorhanden, der entsprechende Vorgang aus der Datenbank geladen und in
  die Oberfläche übertragen.
- withoutVinQueryButton - Über diesen Schalter (true / false) wird der Button zur Ausführung der VIN-Abfrage
  ein- bzw. ausgeblendet.

Alle Eingabeparameter sind optional.

Die möglichen Eingabeparameter werden als Propterties eines JavaScript-Objekts aufbereitet
und mittels einer Hilfsmethode aus dem globalen sphinx-Objekt in XML umgewandelt:

```
<script type="text/javascript" language="JavaScript">
  function load(){
    var values = new Object();

    // do not show DAT header
    values.displayHeader = false;

    // vehicle filter restriction, one of ALL, REPAIR, APPRAISAL or GLASS, default = ALL
    values.Restriction = 'REPAIR';
    // prohibit the change of Restriction (if true the Restriction selection is hidden)
    values.noRestrictionInp = false;

    // Country code for the target market (international licence plate country code, 3 chars)
    // corresponds to the datCountryIndicator (Values: 'D', 'A', 'CH', 'I', 'E', 'F', ...)
    values.CountryCode = 'I';

    // DAT Europa Code
    values.DatECode = '019050850010006';
    // or splitted DAT Europa Code
    // values.VehicleType = 1;
    // values.Manufacturer = 905;
    // values.BaseModel = 85;
    // values.SubModel = 1;
    // values.SubModelVariant = 6;

    // Marktindex
    values.Container = 'DE004';

    // VehicleIdentification Number
    values.VehicleIdentNumber = 'WP0AA298X8U760141';
    // KBA
    values.KbaCode = '3436/ACP';
    // NatCode (for Austria only)
    values.natCode = '162288';
    // Licence plate (for Italy and Switzerland only)
    values.licencePlate = 'BE 12345';
    // Base number (for Switzerland only)
    values.baseNumber = '136.936.153';
    // Type note number (for Switzerland only)
    values.typeNoteNumber = '1LC582';

    // if available vehicle initial registration date in milliseconds since 1/1/1970
    values.InitialRegistration = 1185962400000;
    // vehicle mileage
    values.mileage = 15000;

    // equipment filter, one of ALL, GENERAL, EXTERIOR, INTERIOR, CHASSIS, AGGREGATE or GLASS (default = ALL)
    values.equFilter = 'ALL';
    // comma separated list of dat standard/orptional equipment numbers (eg. '23605,73606')
    values.equDatNr = '';
    // comma separated list of additional equipments (eg. 'auxiliary heating, auxiliary lights')
    values.equAdd = '';

    //create XML data from values
    var inputXml = sphinx.getDAFXml(values);

    . . .

  }
</script>
```
