---
title: "Daten für den Verkauf anlegen"
topic_id: "12137"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Status umbuchen > Daten für den Verkauf anlegen"
---

# Daten für den Verkauf anlegen

Mit der Funktion setSalesData legen Sie Verkaufsdaten zu einem bestehenden Vorgang an.

Hinweis: Nachdem Sie die Verkaufsdaten angelegt haben, können Sie den Status des Dossiers
mit der Funktion changeContractStatus nach Verkauft ändern.

Parameter setSalesData

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ContractID | Long | Eindeutige Vorgangskennung (DossierId) | numerisch | X |
| Orderdate | Date | Auftragsdatum | Format[YYYY-MM-DD] | X |
| SellerId | Integer | ID des Verkäufers (erhält man durch die Methode getPossibleContactPersonsResponse unter dem Parameter id)  ``` <S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">    <S:Body>       <ns3:getPossibleContactPersonsResponse xmlns:ns3="http://www.dat.eu/myClaim/soap/v2/MyClaimExternalService">          <PossibleContactPersons>             <firstName>Max</firstName>             <id>2781</id>             <name>34, Mustermann</name>             <salutation>titleMr</salutation>             <surname>34</surname>          </PossibleContactPersons>       </ns3:getPossibleContactPersonsResponse>    </S:Body> </S:Envelope> ``` | numerisch | X |
| BusinessType | String | Geschäftsart;Hinweis: Die Werte für die Fahrzeuggruppen legen Sie in den Stammdaten an und holen die Daten mit getBusinessTypeList.Der Reponseparameter BusinessType muss eingegeben werden  Parameter getBusinessTypeListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | BusinessTypeListResponse | businessTypeListResponse | Enthält vxs:BusinessTypeList als Unterelement |  |  Element vxs:BusinessTypeListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | BusinessTypeList | businessTypeList | Enthält 0 bis n Positionen vxs:BusinessTypeItem als Unterelemente |  |  Element vxs:BusinessTypeList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | BusinessTypeItem | businessTypeItem | Enthält die Geschäftsartendetails |  |  Element vxs:BusinessTypeItem  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | Designation | String | Bezeichnung von Geschäftsarten |  | | UniqueCode | String | Eindeutiger Code |  | | ValidVehicleTypes | String | Fahrzeugarten |  | | BusinessType | Integer | Eindeutige Nummerierung der Geschäftsarten | numerisch | |  |  |
| VehicleGroup | String | Fahrzeuggruppe;  Hinweis: Die Werte für die Fahrzeuggruppen legen Sie in den Stammdaten an und holen die Daten mit getVehicleGroupList. Der Reponseparameter VehicleGroup muss eingegeben werden.  Bitte beachten Sie, dass die Fahrzeuggruppe, die im Parameter ValidVehicleTypes angegeben ist, mit der Fahrzeugart des Dossiers übereinstimmen muss.  Parameter getVehicleGroupListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupListResponse | vehicleGroupListResponse | Enthält die VehicleGroupList als Unterelement |  |  Element vxs:VehicleGroupListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupList | vehicleGroupList | Enthält 0 bis n Positionen VehicleGroupItem als Unterelemente |  |  Element vxs:VehicleGroupList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupItem | vehicleGroupItem | Enthält die Fahrzeuggruppendetails |  |  Element vxs:VehicleGroupItem  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | Designation | String | Bezeichnung von Fahrzeuggruppen |  | | UniqueCode | String | Eindeutiger Code |  | | ValidVehicleTypes | String | Fahrzeugarten |  | | VehicleGroup | Integer | Eindeutige Nummerierung der Fahrzeuggruppen. | numerisch | |  | X |
| SalesPriceNet | Decimal | Verkaufspreis (EUR) Netto Werden SalesPriceNet und SalesPriceGross angegeben, wird SalesPriceNet verwendet. |  | bedingt (SalesPriceNet oder SalesPriceGross muss angegeben sein) |
| SalesPriceGross | Decimal | Verkaufspreis (EUR) Brutto Werden SalesPriceNet und SalesPriceGross angegeben, wird SalesPriceNet verwendet. |  | bedingt (SalesPriceNet oder SalesPriceGross muss angegeben sein) |
| DeliveryDate | Date | Auslieferungsdatum | Format[YYYY-MM-DD] |  |
| MileageVehicle | Integer | Fahrzeug Laufleistung |  |  |
| MileageOdometer | Integer | Laufleistung entsprechend der Tachoanzeige (km) |  |  |
| RegistrationNumber | String | Amtliches Kennzeichen |  |  |
| SalesDetails | String | Verkaufsangaben;  Hinweis: Die Werte für die Verkaufsangaben legen Sie in den Stammdaten an und holen die Daten mit getSalesDetailsList. Der Reponseparameter SalesDetails muss eingegeben werden  Parameter getSalesDetailsListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | SalesDetailsListResponse | salesDetailsListResponse | Enthält die vxs:SalesDetailsList als Unterelement |  |  Element vxs:SalesDetailsListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | SalesDetailsList | salesDetailsList | Enthält 0 bis n Positionen vxs:SalesDetailsItem als Unterelemente |  |  Element vxs:SalesDetailsList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | SalesDetailsItem | salesDetailsItem | Enthält die Verkaufsangabendetails |  |  Element vxs:SalesDetailsItem  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | Designation | String | Bezeichnung von Verkaufsangaben |  | | UniqueCode | String | Eindeutiger Code |  | | ValidVehicleTypes | String | Fahrzeugarten |  | | SalesDetails | Integer | Eindeutige Nummerierung der Verkaufsangaben für die Verkaufsmaske. | numerisch | |  |  |
| PaymentAgreements | String | Zahlungsvereinbarungen |  |  |
| OtherAgreements | String | Sonstige Vereinbarungen |  |  |
| RenewVehicleInspection | Date | Datum der erneuten Fahrzeuginspektion | Format[YYYY-MM-DD] |  |
| AgreementOnDeviationsCheck | Boolean | Vereinbarung über Abweichungen | true, false |  |
| ShorteningLimitationPeriodCheck | Boolean | Verkürzung der Verjährungsfrist | true, false |  |
| ExclusionOfObligationToUpdateCheck | Boolean | Ausschluss der Aktualisierungspflicht | true, false |  |
| UpdateInformationCheck | Boolean | Information zur Aktualisierung | true, false |  |
| InfoReqUpdatesAndInstallation | String | Angaben zu den erforderlichen Aktualisierungen und deren Installation. Nur zulässig falls UpdateInformationCheck gesetzt wurde. |  |  |
| AgreementOnDeviationsList |  | Vereinbarung über Abweichungen |  |  |

Element AgreementOnDeviationsList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| AgreementOnDeviationItem |  | Vereinbarung über Abweichung |  |  |

Element AgreementOnDeviationItem

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Feature | String | Merkmal der Abweichung |  |  |
| State | String | Tatsächliche Beschaffenheit |  |  |
