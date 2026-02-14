---
title: "Änderungsnachweis"
topic_id: "2689"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Änderungsnachweis"
---

# Änderungsnachweis

Mit der jeweils aktuellsten Fassung verlieren alle früheren Versionen ihre Gültigkeit.

|  |  |  |
| --- | --- | --- |
| Version | Date | Change |
| 2.0 | 21.03.2024 | Erweiterung setCustomTag für die Zuweisung weiterer Rollen. |
| 1.9 | 10.10.2023 | Neuen Funktion deleteContract zum Löschen von Aufträgen. |
| 1.8 | 24.05.2023 | Neue Filter in folderTypes zum Abrufen von geteilten Aufträgen in listContracts()  Erweiterte Beschreibung im Thema für createOrUpdateContractN() zur Anzeige des Fahrzeugbuchsymbols bei der Übertragung eines Fahrzeugs. |
| 1.7 | 03.04.2023 | - Erweiterung der Funktion listContracts mit der Möglichkeit zur Filterung der Vorgangsliste nach Hersteller, Haupttyp und   Untertyp. - Verbesserung der Lesbarkeit durch Gruppierung der Fahrzeugfilter in einem neuen vehicleInfo-Element. - Erweiterung der Funktion saveAddressBook für die Übergabe des Erstzulassungsdatums. |
| 1.6 | 03.02.2023 | Erweiterung der Funktion uploadAttachmentByFolderID, uploadAttachmentByIdentification und listAttachmentsOfContract Response zum Zuweisen und Abrufen von Anhangsattributen.  Verbesserung der Dokumentation für uploadAttachmentByFolderID und uploadAttachmentByIdentification |
| 1.5 | 03.11.2022 | Erweiterter Fullscreen Modus für die Oberflächenintegration zur größeren Darstellung des Arbeitsbereichs.  Weitere Infos im Kapitel [Direktes Aufrufen von myClaim über POST-Schnittstelle](#showid/2797 "Direktes Aufrufen von myClaim über POST-Schnittstelle"). |
| 1.4 | 11.03.2022 | Datenabruf in länderspezifischer Sprache  Oberflächenintegration Direktsprung in einem bestimmten Bereich innerhalb eines Vorgangs für die SilverDAT 3  Suchfilter Erweiterung der Funktion listContract  Erweiterung der Funktion changeContractStatus zum Ändern des Status über Status Identifikation und Type |
| 1.3 | 18.10.2021 | Eine neue Funktion createOrUpdateContractN die den gleichen Funktionsumfang enthält wie createOrUpdateContract, jedoch mit der Erweiterung um einen neuen optionalen Parameter der ausschließlich im Zusammenhang mit dem Aktualisieren / Überschreiben des Dossiers zu verwenden ist. |
| 1.2 | 12.05.2021 | - Neue Capabilities Crash, Charging Session, ADAS sowie zugehörige Datenpunkte und neue Datentypen  - Neue Datenpunkte für charging, dashboard\_lights, diagnostics, engine, hood, lights, maintenance, trips, trunk, usage, vehicle\_information und vehicle\_location  - Abgesetzt: ignition.accessories\_status ignition.status mit Ersatz ignition.state    Weitere detailliertere Informationen können dem offiziellen [High-Mobility-Change-Log](https://github.com/highmobility/auto-api/blob/master/changelogs/L13_changelog.md "Changelog L13") entnommen werden.    Darüber hinaus steht [ein neues SDK](https://docs.high-mobility.com/guides/getting-started/fleet/ "Getting Started Fleet") speziell für flottenbezogene Telematikanwendungen bereit. |
| 1.1 | 19.01.2021 | Die API wurde mit neuen Datenpunkten und Möglichkeiten ausgestattet. Umfasst sind u.a.:  - Transformation des Einheitstyps des Rückgabewerts (z.B.: Laufleistung in Meilen oder Kilometer)  - Separierung der statischen Fahrzeugdaten in eigene Entität (früher Vehicle Status)  - Verfügbarkeitsinformationen für einzelne Datenpunkte (z.B. Update-Rate)    Ein detaillierter Change-Log kann [hier](https://www.github.com/highmobility/auto-api/blob/master/changelogs/L12_changelog.md "HIGH MOBILITY Changelog L12") entnommen werden. |
| 1 | 15.01.2021 | Aufnahme der AUTO API von HIGH MOBILITY in das Kompendium |
