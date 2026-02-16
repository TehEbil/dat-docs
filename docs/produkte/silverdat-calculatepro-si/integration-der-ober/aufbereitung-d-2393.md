---
title: "Aufbereitung der Eingabeparameter"
topic_id: "2393"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Integration der Oberfläche > Aufbereitung der Eingabeparameter"
---

# Aufbereitung der Eingabeparameter

Parameter

Derzeit stehen die folgenden Eingabeparameter zur Verfügung:

- az

  Dieser Parameter ist optional. Er kann entweder eine gültige Vorgangsnummer (contractID) wie beispielsweise via Anlage eines neuen Vorgangs beinhalten oder komplett fehlen. Sollte der Parameter fehlen oder leer gelassen werden,
  betrachtet SilverDAT calculatePro den Aufruf als Neuanlage eines Vorgangs.
- defaultReadyhandler

  Dieser Parameter ist optional. Mögliche Werte sind die booleschen Werte:

  - true - Der Button führt die bislang bekannten Aktionen durch (Default)
  - false - der Button ist sichtbar, ein Klick bewirkt allerdings keine Aktion

  Erfolgt der Aufruf über die Oberflächenschnittstelle der calculatePro, befindet sich
  auf der Kalkulationsergebnisseite bzw. auf der Seite, die durch den Parameter "[Aufruf der SilverDAT calculatePro Oberfläche](aufruf-der-sil-2395.md)" zur letzten Seite deklariert worden ist, ein "Abschließen"-Button, der beim Klick
  der übergeordneten Anwendung über URL-Änderung mitteilt, dass der Prozess durchlaufen
  ist.

  Das führt manchmal zu Problemen, weil die eingebettete HTML-Seite lokal liegt und
  vom Browser aus im Regelfall keine lokale Seite geöffnet werden darf.

  Die Lösung des Problems liegt darin, sich einen Event auf den Button zu registrieren
  und mit dem Parameter zu steuern, ob die Default-Aktion (URL-Änderung) durchgeführt
  wird oder nicht.
- urlReadyHandler

  Dies ist eine Callback-URL, die aufgerufen wird, wenn der Anwender einen Abschließen-Button
  in der Anwendung betätigt. Dieses values-Objekt kann genutzt werden, wenn es bei der Verwendung von <Frame>-Tags zu Problemen beim Auslesen des ready-Objektes kommt. Wird es gesetzt, hängt die Anwendung ein Konstrukt, wie z.B. "?ready=xxx&cid=yyy" an die URL.
- productVariant

  Ruft das Product calculateExpert auf.
- tires

  Dieser Parameter ist optional. Mögliche Werte sind die booleschen Werte:

  - true - Der "Reifendialog" Button erscheint wie gehabt in den Masken der Ausstattungen
    und grafischen Teileauswahl.
  - false - Der "Reifendialog" verschwindet Button in den Masken der Ausstattungen und grafischen
    Teileauswahl, sodass eine Bearbeitung dieses Dialogs nicht mehr möglich ist.
- displayHeader

  Dieser Parameter ist optional. Mögliche Werte sind die booleschen Werte:

  - true - Header aktivieren
  - false - Header deaktivieren
- showProcessMenu

  Dieser Parameter ist optional. Mögliche Werte sind die booleschen Werte:

  - true - Menü aktivieren
  - false - Menü deaktivieren
- hidePrintIcon

  Dieser Parameter ist optional. Mögliche Werte sind die booleschen Werte:

  - true - Der Drucksymbol in der grafischen Teileauswahl und Kalkulationsergebnisseite aktivieren.
  - false - Der Drucksymbol in der grafischen Teileauswahl und Kalkulationsergebnisseite deaktivieren.
- activityRelatedDataBtnActive

  - true - Der "Vorgangsbezogene Daten"-Symbol in der Werkzeugleiste der grafischen Teileauswahl
    aktivieren.
  - false - Der "Vorgangsbezogene Daten"-Symbol in der Werkzeugleiste der grafischen Teileauswahl
    deaktivieren.
- imageGalleryVisible

  Dieser Parameter ist optional. Mögliche Werte sind die booleschen Werte:

  - true - Die Bildergalerie in der grafischen Teileauswahl aktivieren.
  - false - Die Bildergalerie in der grafischen Teileauswahl deaktivieren.
- hideContractCreation

  Der Parameter ist optional und steuert die Sichtbarkeit der Schaltflächen ("Neuen
  Vorgang anlegen", "Vorgabedaten", "Vorgang duplizieren", "Vorgänge importieren") in
  der Vorgangsübersicht. Mögliche Werte sind die booleschen Werte:

  - true - Die Schaltflächen werden sichtbar sein
  - false - Die Schaltflächen werden nicht mehr sichtbar sein (Default)
- FasttrackWorkflow

  Der Parameter ist optional und steuert die Sichtbarkeit der FastTrack in der graphische
  Teileauswahl. Mögliche Werte sind die booleschen Werte:

  - true: Die FastTrack-Ansicht erscheint in der grafischen Teileauswahl (Default)
  - false: Die Zonengrafik wird in der grafischen Teileauswahl erscheinen. Die FastTrack-Ansicht
    wird nicht mehr vorhanden sein.

Umsetzungsbeispiel

Die Eingabeparameter werden als Property eines JavaScript-Objekts aufbereitet und
mittels einer Hilfsmethode aus dem globalen sphinx-Objekt in XML gewandelt:

```
<script type="text/javascript" language="JavaScript">
  function load(){
    var values = new Object();
//contractID, either a valid contractId or empty
    values.az = 4766;
//onClick event handler on calculationResult page
    values.defaultReadyHandler = false;
```

```
// if [values.defaultReadyHandler=true], the application will add a construct like 
// '?ready=xxxx&cid=yyyy' to the given URL
// and will call it as a signal for the ready state
  values.urlReadyHandler = 'https://gold.dat.de/callback.php';
//create XML data from values
    var inputXml = sphinx.getDAFXml(values);
  }
</script>
```
