---
title: "VXS Beispiel"
topic_id: "14080"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > VXS Beispiel"
---

# VXS Beispiel

VXS Beispiel:

```
<vxs:ProcedureRelatedParameters>
    <vxs:ProcedureRelatedParameter attribute="vatRate" factor="CalculationFactor" type="Double">19.0</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="referenceSetName" factor="CalculationFactor" type="String">Standardverrechnungssatz (Default)</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="biwOptimizationMode" factor="CalculationFactor" type="BiwOptimizationMode">AUTOMATIC</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="showLongWorkStrings" factor="CalculationFactor" type="Boolean">true</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="selectedLacquerMethod" factor="CalculationFactor" type="LacquerMethod">EURO_LACQUER</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="timeUnit" factor="CalculationFactor" type="TimeUnitSystem">AW</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="CalculationFactor" type="Integer">12</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="dataCurrency" factor="CalculationFactor" type="String">EUR</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="increaseDecrease" factor="SparePartFactor" type="Double">1.0</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="surchargeInProtocolOly" factor="SparePartFactor" type="Boolean">true</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="smallSparePartCalculationModel" factor="SparePartFactor" type="SmallPartsCalculationModel">PERCENT_OF_PARTS</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="priceDate" factor="SparePartFactor" type="Date">2019-02-01</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="priceSource" factor="SparePartFactor" type="PriceSource">DAT</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="smallSparePartPercentOfPart" factor="SparePartFactor" type="Double">2.0</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="dentWage" factor="LabourCostFactor" mode="PER_TIME_SYSTEM" type="Price">7.5</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="mechanicWage1" factor="LabourCostFactor" mode="PER_TIME_SYSTEM" type="Price">8.3333</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="electricWage1" factor="LabourCostFactor" mode="PER_TIME_SYSTEM" type="Price">8.3333</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="timeUnit" factor="LabourCostFactor" type="TimeUnitSystem">AW</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="LabourCostFactor" type="Integer">12</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="bodyWage1" factor="LabourCostFactor" mode="PER_TIME_SYSTEM" type="Price">8.3333</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="materialPriceCategoryName" factor="EuroLacquerFactor" type="String">Perleffekt (2-Schicht)</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="materialMode" factor="EuroLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="type" factor="EuroLacquerFactor" type="String">30</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="wage" factor="EuroLacquerFactor" mode="PER_TIME_SYSTEM" type="Price">8.3333</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="materialIndex" factor="EuroLacquerFactor" type="Double">100.0</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="wageMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="calculationType" factor="EuroLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="disposalCostPercent" factor="EuroLacquerFactor" type="Double">0.0</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="timeUnit" factor="EuroLacquerFactor" type="TimeUnitSystem">AW</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="EuroLacquerFactor" type="Integer">12</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="materialMode" factor="ManufacturerLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="type" factor="ManufacturerLacquerFactor" type="String">17</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="materialFlatRatePercent" factor="ManufacturerLacquerFactor" type="Double">60.0</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="wage" factor="ManufacturerLacquerFactor" mode="PER_TIME_SYSTEM" type="Price">8.333333333333332</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="typeSaved" factor="ManufacturerLacquerFactor" type="Boolean">true</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="wageMode" factor="ManufacturerLacquerFactor" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="ManufacturerLacquerFactor" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="calculationType" factor="ManufacturerLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="timeUnit" factor="ManufacturerLacquerFactor" type="TimeUnitSystem">AW</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="ManufacturerLacquerFactor" type="Integer">12</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="fourLayerLacquerMode" factor="AztLacquerFactor" type="AztLacquerMode">WET_IN_WET</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="materialMode" factor="AztLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="type" factor="AztLacquerFactor" type="String">17</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="wage" factor="AztLacquerFactor" mode="PER_HOUR" type="Price">99.0</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="materialIndex" factor="AztLacquerFactor" type="Double">60.0</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="aztDataset" factor="AztLacquerFactor" type="Integer">1</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="wageMode" factor="AztLacquerFactor" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="AztLacquerFactor" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="calculationType" factor="AztLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="disposalCostPercent" factor="AztLacquerFactor" type="Double">0.0</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="timeUnit" factor="AztLacquerFactor" type="TimeUnitSystem">HOUR</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="threeLayerLacquerMode" factor="AztLacquerFactor" type="AztLacquerMode">WET_IN_WET</vxs:ProcedureRelatedParameter>
    <vxs:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="AztLacquerFactor" type="Integer">1</vxs:ProcedureRelatedParameter>
</vxs:ProcedureRelatedParameters>
```
