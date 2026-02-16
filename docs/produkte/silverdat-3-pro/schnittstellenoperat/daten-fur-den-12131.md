---
title: "Daten für den Ankauf anlegen"
topic_id: "12131"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Status umbuchen > Daten für den Ankauf anlegen"
---

# Daten für den Ankauf anlegen

Mit der Funktion setPurchaseData legen Sie Ankaufsdaten zu einem bestehenden Vorgang an.

Hinweis: Nachdem Sie die Ankaufsdaten angelegt haben, können Sie den Status des Dossiers mit
der Funktion changeContractStatus nach Disponiert ändern.

Parameter setPurchaseData

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ContractID | Long | Eindeutige Vorgangserkennung (DossierId) | numerisch | X |
| BuyerId | Integer | ID des Käufers (erhält man durch die Methode getPossibleContactPersonsResponse unter dem Parameter id)  ``` <S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">    <S:Body>       <ns3:getPossibleContactPersonsResponse xmlns:ns3="http://www.dat.eu/myClaim/soap/v2/MyClaimExternalService">          <PossibleContactPersons>             <firstName>Max</firstName>             <id>2781</id>             <name>34, Mustermann</name>             <salutation>titleMr</salutation>             <surname>34</surname>          </PossibleContactPersons>       </ns3:getPossibleContactPersonsResponse>    </S:Body> </S:Envelope> ``` | numerisch | X |
| VehicleGroup | String | Fahrzeuggruppe; Hinweis: Die Werte für die Fahrzeuggruppen legen Sie in den Stammdaten an und holen diese mit getVehicleGroupList. Der Reponseparameter VehicleGroup muss eingegeben werden.  Bitte beachten Sie, dass die Fahrzeuggruppe, die im Parameter ValidVehicleTypes angegeben ist, mit der Fahrzeugart des Dossiers übereinstimmen muss.  Parameter getVehicleGroupListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupListResponse | vehicleGroupListResponse | Enthält die VehicleGroupList als Unterelement |  |  Element vxs:VehicleGroupListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupList | vehicleGroupList | Enthält 0 bis n Positionen VehicleGroupItem als Unterelemente |  |  Element vxs:VehicleGroupList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupItem | vehicleGroupItem | Enthält die Fahrzeuggruppendetails |  |  Element vxs:VehicleGroupItem  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | Designation | String | Bezeichnung von Fahrzeuggruppen |  | | UniqueCode | String | Eindeutiger Code |  | | ValidVehicleTypes | String | Fahrzeugarten |  | | VehicleGroup | Integer | Eindeutige Nummerierung der Fahrzeuggruppen. | numerisch | |  | X |
| AcceptanceDate | Date | Geplantes Hereinnahmedatum | Format[YYYY-MM-DD] | X |
| AcceptanceDetails | String | Hereinnahmedetails;  Hinweis: Die Werte für die Hereinnahmedetails legen Sie in den Stammdaten an und holen diese mit getAcceptanceDetailsList. Der Reponseparameter AcceptanceDetails muss eingegeben werden  Parameter getAcceptanceDetailsListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | AcceptanceDetailsListResponse | acceeptanceDetailsListResponse | Enthält die vxs:AcceptanceDetailsList als Unterelement |  |  Element vxs:AcceptanceDetailsListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | AcceptanceDetailsList | acceptanceDetailsList | Enthält 0 bis n Positionen vxs:AcceptanceDetailsItem als Unterelemente |  |  Element vxs:AcceptanceDetailsList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | AcceptanceDetailsItem | acceptanceDetailsIte | Enthält die Hereinnahmedetails |  |  Element vxs:AcceptanceDetailsItem  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | Designation | String | Bezeichnung von Hereinnahmedetails |  | | UniqueCode | String | Eindeutiger Code |  | | ValidVehicleTypes | String | Fahrzeugarten |  | | AcceptanceDetails | Integer | Eindeutige Nummerierung der Hereinnahmedetails | numerisch | |  | X |
| DeregistrationDate | Date | Abmeldedatum | Format[YYYY-MM-DD] |  |
| ResidualWarrantyType | String | Restgarantieart |  |  |
| ResidualWarrantyUntil | Date | Restgarantie bis | Format[YYYY-MM-DD] |  |
| ResidualWarrantyValueNet | Decimal | Restgarantiewert (EUR) Netto Werden ResidualWarrantyValueNet und ResidualWarrantyValueGross angegeben, wird ResidualWarrantyValueNet verwendet. |  |  |
| ResidualWarrantyValueGross | Decimal | Restgarantiewert (EUR) Brutto Werden ResidualWarrantyValueNet und ResidualWarrantyValueGross angegeben, wird ResidualWarrantyValueNet verwendet. |  |  |
| PaymentAgreements | String | Zahlungsvereinbarungen |  |  |
| OtherAgreements | String | Sonstige Vereinbarungen |  |  |
| ProvisionOn | Date | Bereitstellung am | Format[YYYY-MM-DD] |  |
| PurchaseDate | Date | Ankaufsdatum | Format[YYYY-MM-DD] | X |
| PurchasePriceNet | Decimal | Einkaufspreis (EUR) Netto Werden PurchasePriceNet und PurchasePriceGross angegeben, wird PurchasePriceNet verwendet. |  | bedingt (PurchasePriceNet oder PurchasePriceGross muss angegeben sein) |
| PurchasePriceGross | Decimal | Einkaufspreis (EUR) Brutto Werden PurchasePriceNet und PurchasePriceGross angegeben, wird PurchasePriceNet verwendet. |  | bedingt (PurchasePriceNet oder PurchasePriceGross muss angegeben sein) |
| MileageExpected | Integer | Voraussichtliche Laufleistung (km) |  | X |
