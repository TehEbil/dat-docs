---
title: "Börsenaufbereitung (MarketplacePreparation)"
topic_id: "12661"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Weitere Handelsdaten (TradingAdditional) > Börsenaufbereitung (MarketplacePreparation)"
---

# Börsenaufbereitung (MarketplacePreparation)

Element vxs:MarketplacePreparation

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| VehicleNumber | String | Fahrzeugnummer |  |
| ExportFlag | Boolean | Exportieren | true, false |
| MarketplaceVehicleType | String | Fahrzeugtyp Börse |  |
| [MarketplaceAreaList](#showid/25765 "MarketplaceAreaList") | List | Bereich MarketplaceAreaList enthält folgende Unterelemente |  |
| [MarketplaceManufacturerList](#showid/25767 "MarketplaceManufacturerList") | List | Fabrikatenliste MarketplaceManufacturerList enthält folgende Unterelemente |  |
| [MarketplaceModelGroupList](#showid/25769 "MarketplaceModelGroupList") | List | Modellgruppenliste MarketplaceModelGroupList enthält folgende Unterelemente |  |
| [MarketplaceModelList](#showid/25771 "MarketplaceModelList") | List | Modellliste und MarketplaceModelList enthält folgende Unterelemente |  |
| [MarketplaceVehicleSectionList](#showid/25773 "MarketplaceVehicleSectionList") | List | Fahrzeugbereichliste MarketplaceVehicleSectionList enthält folgende Unterelemente |  |
| [MarketplaceTypeLineList](#showid/25775 "MarketplaceTypeLineList") | List | Typzeile MarketplaceTypeLineList enthält folgende Unterelemente |  |
| [MarketplaceFuelConsumptionDataList](#showid/25777 "MarketplaceFuelConsumptionDataList") | List | Kraftstoffverbrauchswerteliste MarketplaceFuelConsumptionDataList enthält folgende Unterelemente |  |
| MarketplaceFuelAccordingEnVkVList | List | Kraftstoffliste nach EnVKV MarketplaceFuelAccordingEnVkVList enthält folgende Unterelemente |  |
| MarketplaceFuelAccordingEnVkVCust | String | Kraftstoff nach EnVKV für FHD/VXS |  |
| [MarketplaceColorInteriorFittingsList](#showid/25781 "MarketplaceColorInteriorFittingsList") | List | Innenausstattungsfarbenliste MarketplaceColorInteriorFittingsList enthält folgende Unterelemente |  |
| [AdvertisementFeatures](#showid/25783 "AdvertisementFeatures") | List | Börsenexport-Werbungsliste AdvertisementFeatures enthält folgende Unterelemente. |  |
| GeneralInspection | String | Hauptuntersuchung |  |
| GeneralInspectionNewFlag | Boolean | HU neu true=Hauptuntersuchung ist neu; false=Hauptuntersuchung ist nicht neu | true, false |
| WithFullServiceHistoryFlag | Boolean | Checkheft gepflegt | true, false |
| [MarketplaceAccidentalDamageList](#showid/25789 "MarketplaceAccidentalDamageList") | List | Unfallschadenliste MarketplaceAccidentalDamageList enthält folgende Unterelemente |  |
| DescriptionAccidentalDamage | String | Unfallschadenbeschreibung |  |
| DealerCarFlag | Boolean | Händlerfahrzeug | true, false |
| [MarketplaceWarrantyList](#showid/25791 "MarketplaceWarrantyList") | List | Garantieliste MarketplaceWarrantyList enthält folgende Unterelemente |  |
| EquipmentFormat | String | Ausstattungsformat | Gruppen Liste Fließtext |
| EquipmentSorting | String | Ausstattungssortierung |  |
| [MarketplaceEquipmentGroupListN](#showid/25793 "MarketplaceEquipmentGroupListN") | List | Börsenausstattungsliste und MarketplaceEquipmentGroupListN enthält folgende Unterelemente |  |
| IntroductionText | String | Einleitungstext Vorgang |  |
| FinalText | String | Schlusstext Vorgang |  |
| MPConfigIntroText | String | Einleitungstext Börsenkonfiguration |  |
| MPConfigFinalText | String | Schlusstext Börsenkonfiguration |  |
| NonSmokerCarFlag² | Boolean | Nichtraucherfahrzeug | true, false |
| MarketplaceProductionCountryVersion | String | Setzen der [Landesversion](#expandblock-12661-d2e733583) des Fahrzeugs  Mit dem Parameter MarketplaceProductionCountryVersion kann die Länderversion des Fahrzeugs bestimmt werden.    |  | | --- | | Wert | | Deutsche Ausführung | | EU-Ausführung | | AT | | IT | | String |
| PeriodOfDelivery² | String | Auslieferungszeitraum | String |
| [PeriodOfDeliverySpecificList²](#showid/25795 "PeriodOfDeliverySpecificList") | List | Auslieferungszeitraum, börsenspezifisch festgelegt |  |
| PlannedDeliveryDateCustomer² | Date | Liefer-/Verfügbarkeitsdatum | YYYY-MM-DD |
| TaxiFlag² | Boolean | ehemals Taxi | true, false |
| E10SuitableFlag² | Boolean | geeigenet für Kraftstofftyp E10 | true, false |
| BiodieselSuitableFlag² | Boolean | geeigenet für Kraftstofftyp Biodiesel | true, false |
| VegetableOilSuitableFlag² | Boolean | geeigenet für Kraftstofftyp Pflanzenöl | true, false |
| AccessiblyDesignedFlag² | Boolean | Behindertengerecht | true, false |
| [MPConfigIntroTextList²](#showid/25797 "MPConfigIntroTextList") | List | Liste mit den Einleitungstexten der Börsenkonfigurationen |  |
| [MPConfigFinalTextList²](#showid/25799 "MPConfigFinalTextList") | List | Liste mit den Schlusstexten der Börsenkonfigurationen |  |
| [MarketplaceEquipmentFlagList²](#showid/25801 "MarketplaceEquipmentFlagList") | List | Liste mit den Angaben zu den börsenspezifischen Ausstattungen |  |
| [MpEquipmentFlagAttributesData](#showid/25813 "MpEquipmentFlagAttributesData")[²](#showid/25803 "QualityLabelsList") | List | Liste mit den Angaben zu den börsenspezifischen Ausstattungsflags |  |
| [QualityLabelsList²](#showid/25803 "QualityLabelsList") | List | Liste mit Qualitätssiegeln |  |
| [EnVKVAdditionals](#showid/25819 "EnVKVAdditionals") | List | Zusätzliche Werte nach ENVKV |  |

² Elemente können nicht über die API gesetzt werden, Zustand ist aber in der Response
enthalten.
