---
title: "Daten für den Zugang anlegen"
topic_id: "12134"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Status umbuchen > Daten für den Zugang anlegen"
---

# Daten für den Zugang anlegen

Mit der Funktion setAdmissionData legen Sie Zugangsdaten zu einem bestehenden Vorgang an.

Hinweis: Nachdem Sie die Zugangsdaten angelegt haben, können Sie den Status des Dossiers mit
der Funktion changeContractStatus nach Bestand ändern.

Parameter setAdmissionData

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ContractID | Long | Eindeutige Vorgangserkennung (DossierId) | numerisch | X |
| BuyerId | Integer | ID des Käufers(erhält man durch die Methode [getPossibleContactPersons](#expandblock-12134-d2e717426)Response unter dem Parameter id)  ``` <S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">    <S:Body>       <ns3:getPossibleContactPersonsResponse xmlns:ns3="http://www.dat.eu/myClaim/soap/v2/MyClaimExternalService">          <PossibleContactPersons>             <firstName>Max</firstName>             <id>2781</id>             <name>34, Mustermann</name>             <salutation>titleMr</salutation>             <surname>34</surname>          </PossibleContactPersons>       </ns3:getPossibleContactPersonsResponse>    </S:Body> </S:Envelope> ``` | numerisch | X |
| VehicleGroup | String | Fahrzeuggruppe;  Hinweis: Die Werte für die Fahrzeuggruppen legen Sie in den Stammdaten an und holen diese mit [getVehicleGroupList](#expandblock-12134-d2e717456). Der Reponseparameter VehicleGroup muss eingegeben werden.  Bitte beachten Sie, dass die Fahrzeuggruppe, die im Parameter ValidVehicleTypes angegeben ist, mit der Fahrzeugart des Dossiers übereinstimmen muss.  Parameter getVehicleGroupListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupListResponse | vehicleGroupListResponse | Enthält die VehicleGroupList als Unterelement |  |  Element vxs:VehicleGroupListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupList | vehicleGroupList | Enthält 0 bis n Positionen VehicleGroupItem als Unterelemente |  |  Element vxs:VehicleGroupList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupItem | vehicleGroupItem | Enthält die Fahrzeuggruppendetails |  |  Element vxs:VehicleGroupItem  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | Designation | String | Bezeichnung von Fahrzeuggruppen |  | | UniqueCode | String | Eindeutiger Code |  | | ValidVehicleTypes | String | Fahrzeugarten |  | | VehicleGroup | Integer | Eindeutige Nummerierung der Fahrzeuggruppen. | numerisch | |  | X |
| AcceptanceDate | Date | Hereinnahmedatum | Format[YYYY-MM-DD] | X |
| AcceptanceDetails | String | Hereinnahmedetails;  Hinweis: Die Werte für die Hereinnahmedetails legen Sie in den Stammdaten an und holen diese mit [getAcceptanceDetailsList](#expandblock-12134-d2e717508). Der Reponseparameter AcceptanceDetails muss eingegeben werden  Parameter getAcceptanceDetailsListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | AcceptanceDetailsListResponse | acceeptanceDetailsListResponse | Enthält die vxs:AcceptanceDetailsList als Unterelement |  |  Element vxs:AcceptanceDetailsListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | AcceptanceDetailsList | acceptanceDetailsList | Enthält 0 bis n Positionen vxs:AcceptanceDetailsItem als Unterelemente |  |  Element vxs:AcceptanceDetailsList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | AcceptanceDetailsItem | acceptanceDetailsIte | Enthält die Hereinnahmedetails |  |  Element vxs:AcceptanceDetailsItem  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | Designation | String | Bezeichnung von Hereinnahmedetails |  | | UniqueCode | String | Eindeutiger Code |  | | ValidVehicleTypes | String | Fahrzeugarten |  | | AcceptanceDetails | Integer | Eindeutige Nummerierung der Hereinnahmedetails | numerisch | |  |  |
| DeregistrationDate | Date | Abmeldedatum | Format[YYYY-MM-DD] |  |
| ResidualWarrantyType | String | Restgarantieart |  |  |
| ResidualWarrantyUntil | Date | Restgarantie bis | Format[YYYY-MM-DD] |  |
| ResidualWarrantyValueNet | Decimal | Restgarantiewert (EUR) Netto Werden ResidualWarrantyValueNet und ResidualWarrantyValueGross angegeben, wird ResidualWarrantyValueNet verwendet. |  |  |
| ResidualWarrantyValueGross | Decimal | Restgarantiewert (EUR) Brutto Werden ResidualWarrantyValueNet und ResidualWarrantyValueGross angegeben, wird ResidualWarrantyValueNet verwendet. |  |  |
| PaymentAgreements | String | Zahlungsvereinbarungen |  |  |
| OtherAgreements | String | Sonstige Vereinbarungen |  |  |
| ProvisionOn | Date | Bereitstellung am | Format[YYYY-MM-DD] |  |
| AdmissionDate | Date | Ankaufsdatum | Format[YYYY-MM-DD] | X |
| AdmissionPriceNet | Decimal | Einkaufspreis (EUR) Netto Werden AdmissionPriceNet und AdmissionPriceGross angegeben, wird AdmissionPriceNet verwendet. |  | bedingt (AdmissionPriceNet oder AdmissionPriceGross muss angegeben sein) |
| AdmissionPriceGross | Decimal | Einkaufspreis (EUR) Brutto Werden AdmissionPriceNet und AdmissionPriceGross angegeben, wird AdmissionPriceNet verwendet. |  | bedingt (AdmissionPriceNet oder AdmissionPriceGross muss angegeben sein) |
| MileageOdometer | Integer | Laufleistung entsprechend der Tachoanzeige bei der Hereinnahme des Fahrzeugs (km) |  |  |
| MileageVehicle | Integer | Fahrzeug Laufleistung (km) |  | X |
| Location | String | Standort des Fahrzeugs |  |  |
