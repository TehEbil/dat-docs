---
title: "Derivat-Ereignisse"
topic_id: "27919"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Datenstrukturen > Fahrzeugspezifikationen > Derivat-Ereignisse"
---

# Derivat-Ereignisse

Der events-Abschnitt eines Derivats hat die folgenden Eigenschaften:

| Name der Eigenschaft | Typ | Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| usability | String | gültige Verwendbarkeitskennungen | Gibt den Grad der Vervollständigung der Daten des Derivats in der neuesten Version an | ja |
| usabilityModified | Datum |  | Datum, an dem die usability-Eigenschaft zuletzt geändert wurde | ja |
| derivativeIntroduced | Datum |  | Datum, an dem das Derivat auf den Markt kam | ja |
| derivativeChanged | Datum |  | Datum, an dem das Derivat zuletzt auf dem Markt geändert wurde | ja |
| derivativeChangeType | String | gültige Derivat-Änderungskennungen | Art der Marktänderung | ja |

Die usability-Eigenschaft kann einen der folgenden Werte annehmen:

- "pricesOnly": Bedeutet, dass für die neueste Version des Derivats nur die Grunddaten und die
  preisbezogenen Daten eingegeben wurden.
- "pricesAndEquipment": Bedeutet, dass die Grunddaten, die preisbezogenen Daten und die wichtigsten Fahrzeugspezifikationen
  für die neueste Version des Derivats eingegeben wurden.
- "complete": Bedeutet, dass die Grunddaten, die preisbezogenen Daten, alle verfügbaren Fahrzeugspezifikationen
  und die Ausstattungspositionen für die neueste Version des Derivats eingegeben wurden.

Die derivateChangeType-Eigenschaft kann einen der folgenden Werte annehmen:

- "newModel": Bedeutet, dass das Derivat zu einem neuen Modell oder einer neuen Modellgeneration
  gehört, die gerade auf den Markt gekommen ist.
- "facelift": Bedeutet, dass das Derivat zur Facelift-Version eines bestehenden Modells gehört,
  das bereits auf dem Markt ist.
- "newVersion": Bedeutet, dass das Derivat eine neue Kombination aus Motor, Getriebe und Serienausstattungslevel
  hat, aber zu einem bereits bestehenden Modell gehört.
- "specChange": Bedeutet, dass das Derivat bereits existierte, es aber Änderungen in der Serienausstattung
  gab.
- "optionChange": Bedeutet, dass das Derivat bereits existierte und die Serienausstattung unverändert
  ist, es aber Änderungen in der Sonderausstattung gab.
- "priceChange": Bedeutet, dass das Derivat und seine Ausstattung unverändert sind, sich aber der
  Preis des Derivats geändert hat.
- "taxChange": Gleich wie "priceChange", außer dass die Preisänderung auf Änderungen der Besteuerung durch staatliche Behörden
  zurückzuführen ist.
