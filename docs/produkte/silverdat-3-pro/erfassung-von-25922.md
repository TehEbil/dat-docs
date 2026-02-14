---
title: "Erfassung von Neufahrzeugen, Tageszulassungen und Vorführfahrzeugen"
topic_id: "25922"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Erfassung von Neufahrzeugen, Tageszulassungen und Vorführfahrzeugen"
---

# Erfassung von Neufahrzeugen, Tageszulassungen und Vorführfahrzeugen

Innerhalb der Fahrzeugbewertung ist es möglich Vorgänge für Neufahrzeuge, Tageszulassungen
und Vorführfahrzeuge zu erfassen.

Generell werden hierzu die vorhandenen Services und Methoden zum [Verwalten von Vorgängen](verwalten-von-15172.md) verwendet und um die entsprechenden Parameter ergänzt.

Die Art des Vorgangs kann nach Anlage nur begrenzt geändert werden. Es gelten folgende
Regeln:

- Die Umwandlung eines Gebrauchtfahrzeug-Vorgangs in eine andere Vorgangsart ist nicht
  möglich
- Die Umwandlung eines Neufahrzeug-Vorgangs ist nur in einen Tageszulassung-Vorgang
  oder Vorführfahrzeug-Vorgang möglich. Eine Umwandlung in einen Gebrauchtfahrzeug-Vorgang
  ist nicht möglich.
- Die Umwandlung eines Tageszulassung-Vorgangs ist nur in Vorführfahrzeug-Vorgang möglich.
  Eine Umwandlung in einen Gebrauchtfahrzeug- oder Neufahrzeug-Vorgang ist nicht möglich.
- Die Umwandlung eines Vorführfahrzeug-Vorgangs ist nur in einen Tageszulassung-Vorgang
  möglich. Eine Umwandlung in einen Gebrauchtfahrzeug- oder Neufahrzeug-Vorgang ist
  nicht möglich.
- Im Status Verkauft ist generell keine Umwandlung mehr möglich.

Folgendes gilt für Neufahrzeuge:

- Für den Parameter VatType unter VAT kann nur der Wert regular angegeben werden. Differenzbesteuerung ist nicht zulässig.
- Der Parameter InitialRegistration unter Vehicle kann nicht angegeben werden.
- Der Parameter Mileage unter Vehicle ist optional.
- Der Parameter InstallDate unter EquipmentPosition kann nicht angegeben werden.
- Folgende Parameter unter Tires werden nicht angeboten

  - TireOriginalPrice
  - TreadDepthLeftOuterPerc
  - TreadDepthRightOuterPerc
  - TreadDepthLeftOuterMm
  - TreadDepthRightOuterMm
  - TreadDepthLeftInnerPerc
  - TreadDepthRightInnerPerc
  - TreadDepthLeftInnerMm
  - TreadDepthRightInnerMm
  - DefaultTiresPrice
- Folgende Parameter unter Condition können nicht angegeben werden

  - IncreaseInValue
  - TiresMountedValue
  - TiresUnmountedValue
  - NumberOfOwnersN
  - OwnerCorrectionPerc
  - ConditionCorrectionFactorPerc
  - ConditionCorrectionFactorDescription
  - RepairCosts
  - RepairCostsInTradeMargin
  - NexGeneralInspection
  - LastServiceDate
  - NextServiceDate
  - LastServiceMileage
  - NextServiceMileage
- Folgende Parameter unter Valuation werden nicht angeboten:

  - ReferenceMileage
  - MileageCorr
  - InitialRegsitrationCorr
  - BasePrice
  - BasePrice2
  - ValuationCorrection
  - BasePrice3
  - DefaultTiresPrice
  - ConditionCorrectionPerc
  - SalesPrice
  - SalesPriceGross
  - SalesPriceRounded
  - SalesPriceGrossRounded
  - Margin
  - MarginGross
  - MarginRounded
  - MarginGrossRounded
  - PurchasePrice
  - PurchasePriceGross
  - PurchasePriceRounded
  - PurchasePriceGrossRounded
  - PrognosisDate
  - SalesPricePrognosis
  - SalesPricePrognosisGross
  - MarginPrognosis
  - MarginPrognosisGross
  - PurchasePricePrognosis
  - PurchasePricePrognosisGross
  - ObsoletePrognosis
  - PrognosisMileageDat
  - ExtendedMileageCorrection
- Der Aufruf der webScan-Funktionalität ist nicht möglich.
- Der Node PriceCalculation unter TradingAcitvity wird nicht in der Response zurückgegeben.
- Der Node Purchase unter TradingActivity wird wird nicht in der Response zurückgegeben.

Folgendes gilt für Tageszulassungen:

- Der Aufruf der webScan-Funktionalität ist nicht möglich.
- Der Node PriceCalculation unter TradingAcitvity wird nicht in der Response zurückgegeben.

Folgendes gilt für Vorführfahrzeuge:

- Der Aufruf der webScan-Funktionalität ist nicht möglich.
- Der Node PriceCalculation unter TradingAcitvity wird nicht in der Response zurückgegeben.
