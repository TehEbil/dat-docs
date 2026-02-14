---
title: "CalculationProtocol"
topic_id: "16543"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > CalculationProtocol"
---

# CalculationProtocol

Verfügbare Elemente

| Element | Typ | Beschreibung |
| --- | --- | --- |
| [ProtocolHints](protocolhints-16549.md) | complexType, optional,  [ProtocolHint](protocolhints-16549.md) | Unter diesem Knoten werden Hinweistexte ausgegeben |
| InvalidPositionsProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Ungültige Positionen / fehlende Verbauungsbedingungen |
| PartsWithoutWorkProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Enthält die Ersatzteile ohne Arbeit (Stufe = 0) |
| UnspecificPositionsProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Serienübergreifende Verbauungsbedingungen |
| SuppressedPositionsProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Vom Benutzer unterdrückte Positionen |
| MissingLacquerInformationProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Fehlende Lackdaten |
| ImplausiblePositionsProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Unplausible Positionen |
| MissingInputProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Fehlende Angaben wie z.B. Preis oder Arbeitszeit |
| PredamagePositionsProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Positionen mit (100%) Vorschaden |
| SetupTimeRelevantPositionsProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Positionen, die zur Vorbereitungszeit führten |
| WithoutUsedPriceProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Austausch-Ersatzteile ohne Preisvorgabe |
| WithoutManufacturerPriceProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | „Normale" Ersatzteile ohne Preisvorgabe |
| WithLacquerBlendingProtocol | complexType, optional, [ProtocolEntries](protocolentrie-16556.md) | Lack-Positionen mit Beilackierung |
| PartsOfOtherPositionProtocol | complexType, optional, [ProtocolEntriesWithRemoval](protocolentrie-16558.md) | Abgemagerte Eingabepositionen |
| PartsOfCombinationPositionProtocol | complexType, optional, [ProtocolEntriesWithRemoval](protocolentrie-16558.md) | Zu Kombination zusammengefasst |
| RemovedByCompositePositionProtocol | complexType, optional, [ProtocolEntriesWithRemoval](protocolentrie-16558.md) | Durch Verbundarbeit abgemagert |
| RemovedRepairTypesProtocol | complexType, optional, [ProtocolEntriesWithRemoval](protocolentrie-16558.md) | Arbeitsart (RC) ist in anderer Position enthalten |
| DentPositionsProtocol | complexType, optional, [DentPositionsProtocolEntries](dentpositionsp-16560.md) | Hinweise zum Hagelschaden |
| PositionsWithMeasuresProtocol | complexType, optional, [PositionsWithMeasuresEntry](positionswithm-16562.md) | Teile mit Maßangaben |
| PriceCorrectionsProtocol | complexType, optional, [PriceCorrectionsProtocolEntries](pricecorrectio-16564.md) | Preiskorrekturen |
