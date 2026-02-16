---
title: "Aufruf der Oberfläche"
topic_id: "2240"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Integration der Oberfläche > Aufruf der Oberfläche"
---

# Aufruf der Oberfläche

Die nachfolgenden Angaben werden zum Aufruf der SilverDAT 3 valuateFinance über die Schnittstelle grundsätzlich benötigt:

Basis-URL: https://www.datgroup.com/FinanceLine

- Host-URL - Endpunkt der externen Anwendung, die SilverDAT 3 valuateFinance einbindet
- Bezeichnung des Inlineframes
- Anmeldeinformationen

Alle weiteren Angaben müssen je nach Aktionstyp unterschiedlich gesetzt werden.

Zur Vorgabe und Verarbeitung stellt das globale sphinx-Objekt die für den Aufruf und
die Kommunikation nötigen Eigenschaften und Methoden zur Verfügung. Die grundsätzlichen
Eigenschaften müssen immer, die restlichen je nach Bedarf gesetzt werden, weitere
Details finden Sie unter Aufbereitung der Eingabeparameter.

Als erstes werden die Angaben für die URL der SilverDAT 3 valuateFinance und für den Namen beziehungsweise der ID des Inlineframe iframe benötigt. Diese setzen Sie mit der Funktion sphinx.setProductUrl beziehungsweise mit sphinx.setIframeName. Als nächstes muss die Host-URL ihrer Anwendung angegeben werden, die Sie mit der
Funktion sphinx.hostUrl festlegen. Die Anmeldedaten geben Sie mit der Funktion sphinx.credentials an. Die zugehörigen Parameter sind unter [Aufbereitung der Authentifizierungsinformationen](aufbereitung-d-2244.md) nachfolgend genauer beschrieben. Mittels der Eigenschaft sphinx.params setzen Sie die spezifischen Vorgaben für SilverDAT 3 valuateFinance wie zum Beispiel: Land, Sprache und Aktion. Die Beschreibung dieser Parameter folgt.
Bitte verwenden Sie zur Fehlerbehandlung bei der Anmeldung die Funktion sphinx.onLoginFailure. Mit der Funktion sphinx.onFinished führen Sie die Aktionen nach einer abgeschlossenen Bewertung durch. Mit der Funktion
sphinx.exportDossier exportieren Sie die VXS-Daten der aktuellen Bewertung und mit sphinx.afterExportDossier steuern Sie die Weiterverarbeitung nach dem Export. Mittels der Methode sendDossierRequest erfolgt die Ausführung und Anzeige der Aktion.

Übersicht der benötigten Funktionen und Parameter

| Funktion/Eigenschaft | Bedeutung |
| --- | --- |
| sphinx.setProductUrl | Basis-URL der SilverDAT 3 valuateFinance |
| sphinx.hostUrl | Host-URL der aufrufenden Anwendung, die SilverDAT 3 valuateFinance einbindet |
| sphinx.setIframeName | Name beziehungsweise ID des Inlineframe iframe |
| sphinx.credentials | Anmeldeinformation; Die Beschreibung der Parameter finden Sie unter [Aufbereitung der Authentifizierungsinformationen](aufbereitung-d-2244.md). |
| sphinx.params | Setzen der spezifischen Einstellungen für SilverDAT 3 valuateFinance:    datCountryIndicator - Landesflag für den Zielmarkt; ISO 3166 ALPHA-2  locale - Sprachkürzel (Language)  action - Aktionstyp  dossierid - Eindeutige Vorgangskennung entsprechend [Verwalten von Vorgängen](../../allgemeine-services/verwalten-von-vorgan/funktionsumfan-15005.md)  type - Typ des anzulegenden Vorgangs  vxs - VXS-Vorgangsdaten; Pflicht für Aktion importDossier  page - [Aufrufziel](aufrufziele-2246.md) (Seite)  workflow - boolean; Berechtigung zum Navigieren innerhalb des Vorgangs  save - boolean; Berechtigung zum Speichern des Vorgangs |
| sphinx.onLoginFailure | Fehlerbehandlung bei der Anmeldung. |
| sphinx.onFinished | Diese Funktion wird nach dem Betätigen des Beenden-Buttons aufgerufen. |
| sphinx.exportDossier | Exportieren der VXS-Daten der aktuellen Bewertung. |
| sphinx.afterExportDossier | Steuerung der Weiterverarbeitung nach dem Export der VXS-Daten. |
| sphinx.sendDossierRequest | Aufruf der SilverDAT 3 valuateFinance Oberfläche mit den vorgegebenen Parametern. |
