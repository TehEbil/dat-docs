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
| [MarketplaceAreaList](marketplaceare-25765.md) | List | Bereich MarketplaceAreaList enthält folgende Unterelemente |  |
| [MarketplaceManufacturerList](marketplaceman-25767.md) | List | Fabrikatenliste MarketplaceManufacturerList enthält folgende Unterelemente |  |
| [MarketplaceModelGroupList](marketplacemod-25769.md) | List | Modellgruppenliste MarketplaceModelGroupList enthält folgende Unterelemente |  |
| [MarketplaceModelList](marketplacemod-25771.md) | List | Modellliste und MarketplaceModelList enthält folgende Unterelemente |  |
| [MarketplaceVehicleSectionList](marketplaceveh-25773.md) | List | Fahrzeugbereichliste MarketplaceVehicleSectionList enthält folgende Unterelemente |  |
| [MarketplaceTypeLineList](marketplacetyp-25775.md) | List | Typzeile MarketplaceTypeLineList enthält folgende Unterelemente |  |
| [MarketplaceFuelConsumptionDataList](marketplacefue-25777.md) | List | Kraftstoffverbrauchswerteliste MarketplaceFuelConsumptionDataList enthält folgende Unterelemente |  |
| MarketplaceFuelAccordingEnVkVList | List | Kraftstoffliste nach EnVKV MarketplaceFuelAccordingEnVkVList enthält folgende Unterelemente |  |
| MarketplaceFuelAccordingEnVkVCust | String | Kraftstoff nach EnVKV für FHD/VXS |  |
| [MarketplaceColorInteriorFittingsList](marketplacecol-25781.md) | List | Innenausstattungsfarbenliste MarketplaceColorInteriorFittingsList enthält folgende Unterelemente |  |
| [AdvertisementFeatures](advertisementf-25783.md) | List | Börsenexport-Werbungsliste AdvertisementFeatures enthält folgende Unterelemente. |  |
| GeneralInspection | String | Hauptuntersuchung |  |
| GeneralInspectionNewFlag | Boolean | HU neu true=Hauptuntersuchung ist neu; false=Hauptuntersuchung ist nicht neu | true, false |
| WithFullServiceHistoryFlag | Boolean | Checkheft gepflegt | true, false |
| [MarketplaceAccidentalDamageList](marketplaceacc-25789.md) | List | Unfallschadenliste MarketplaceAccidentalDamageList enthält folgende Unterelemente |  |
| DescriptionAccidentalDamage | String | Unfallschadenbeschreibung |  |
| DealerCarFlag | Boolean | Händlerfahrzeug | true, false |
| [MarketplaceWarrantyList](marketplacewar-25791.md) | List | Garantieliste MarketplaceWarrantyList enthält folgende Unterelemente |  |
| EquipmentFormat | String | Ausstattungsformat | Gruppen Liste Fließtext |
| EquipmentSorting | String | Ausstattungssortierung |  |
| [MarketplaceEquipmentGroupListN](marketplaceequ-25793.md) | List | Börsenausstattungsliste und MarketplaceEquipmentGroupListN enthält folgende Unterelemente |  |
| IntroductionText | String | Einleitungstext Vorgang |  |
| FinalText | String | Schlusstext Vorgang |  |
| MPConfigIntroText | String | Einleitungstext Börsenkonfiguration |  |
| MPConfigFinalText | String | Schlusstext Börsenkonfiguration |  |
| NonSmokerCarFlag² | Boolean | Nichtraucherfahrzeug | true, false |
| MarketplaceProductionCountryVersion | String | Setzen der Landesversion des Fahrzeugs  Mit dem Parameter MarketplaceProductionCountryVersion kann die Länderversion des Fahrzeugs bestimmt werden.    |  | | --- | | Wert | | Deutsche Ausführung | | EU-Ausführung | | AT | | IT | | String |
| PeriodOfDelivery² | String | Auslieferungszeitraum | String |
| [PeriodOfDeliverySpecificList²](periodofdelive-25795.md) | List | Auslieferungszeitraum, börsenspezifisch festgelegt |  |
| PlannedDeliveryDateCustomer² | Date | Liefer-/Verfügbarkeitsdatum | YYYY-MM-DD |
| TaxiFlag² | Boolean | ehemals Taxi | true, false |
| E10SuitableFlag² | Boolean | geeigenet für Kraftstofftyp E10 | true, false |
| BiodieselSuitableFlag² | Boolean | geeigenet für Kraftstofftyp Biodiesel | true, false |
| VegetableOilSuitableFlag² | Boolean | geeigenet für Kraftstofftyp Pflanzenöl | true, false |
| AccessiblyDesignedFlag² | Boolean | Behindertengerecht | true, false |
| [MPConfigIntroTextList²](mpconfigintrot-25797.md) | List | Liste mit den Einleitungstexten der Börsenkonfigurationen |  |
| [MPConfigFinalTextList²](mpconfigfinalt-25799.md) | List | Liste mit den Schlusstexten der Börsenkonfigurationen |  |
| [MarketplaceEquipmentFlagList²](marketplaceequ-25801.md) | List | Liste mit den Angaben zu den börsenspezifischen Ausstattungen |  |
| [MpEquipmentFlagAttributesData](mpequipmentfla-25813.md)[²](qualitylabelsl-25803.md) | List | Liste mit den Angaben zu den börsenspezifischen Ausstattungsflags |  |
| [QualityLabelsList²](qualitylabelsl-25803.md) | List | Liste mit Qualitätssiegeln |  |
| [EnVKVAdditionals](envkvadditiona-25819.md) | List | Zusätzliche Werte nach ENVKV |  |

² Elemente können nicht über die API gesetzt werden, Zustand ist aber in der Response
enthalten.
