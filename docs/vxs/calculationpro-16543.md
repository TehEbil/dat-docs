---
title: "CalculationProtocol"
topic_id: "16543"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > CalculationProtocol"
---

# CalculationProtocol

Verfügbare Elemente

| Element | Typ | Beschreibung |
| --- | --- | --- |
| [ProtocolHints](#showid/16549 "ProtocolHints") | complexType, optional,  [ProtocolHint](#showid/16549 "ProtocolHints") | Unter diesem Knoten werden Hinweistexte ausgegeben |
| InvalidPositionsProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Ungültige Positionen / fehlende Verbauungsbedingungen |
| PartsWithoutWorkProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Enthält die Ersatzteile ohne Arbeit (Stufe = 0) |
| UnspecificPositionsProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Serienübergreifende Verbauungsbedingungen |
| SuppressedPositionsProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Vom Benutzer unterdrückte Positionen |
| MissingLacquerInformationProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Fehlende Lackdaten |
| ImplausiblePositionsProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Unplausible Positionen |
| MissingInputProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Fehlende Angaben wie z.B. Preis oder Arbeitszeit |
| PredamagePositionsProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Positionen mit (100%) Vorschaden |
| SetupTimeRelevantPositionsProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Positionen, die zur Vorbereitungszeit führten |
| WithoutUsedPriceProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Austausch-Ersatzteile ohne Preisvorgabe |
| WithoutManufacturerPriceProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | „Normale" Ersatzteile ohne Preisvorgabe |
| WithLacquerBlendingProtocol | complexType, optional, [ProtocolEntries](#showid/16556 "ProtocolEntries") | Lack-Positionen mit Beilackierung |
| PartsOfOtherPositionProtocol | complexType, optional, [ProtocolEntriesWithRemoval](#showid/16558 "ProtocolEntriesWithRemoval") | Abgemagerte Eingabepositionen |
| PartsOfCombinationPositionProtocol | complexType, optional, [ProtocolEntriesWithRemoval](#showid/16558 "ProtocolEntriesWithRemoval") | Zu Kombination zusammengefasst |
| RemovedByCompositePositionProtocol | complexType, optional, [ProtocolEntriesWithRemoval](#showid/16558 "ProtocolEntriesWithRemoval") | Durch Verbundarbeit abgemagert |
| RemovedRepairTypesProtocol | complexType, optional, [ProtocolEntriesWithRemoval](#showid/16558 "ProtocolEntriesWithRemoval") | Arbeitsart (RC) ist in anderer Position enthalten |
| DentPositionsProtocol | complexType, optional, [DentPositionsProtocolEntries](#showid/16560 "DentPositionsProtocolEntry") | Hinweise zum Hagelschaden |
| PositionsWithMeasuresProtocol | complexType, optional, [PositionsWithMeasuresEntry](#showid/16562 "PositionsWithMeasuresEntry") | Teile mit Maßangaben |
| PriceCorrectionsProtocol | complexType, optional, [PriceCorrectionsProtocolEntries](#showid/16564 "PriceCorrectionsProtocolEntry") | Preiskorrekturen |
