---
title: "Verkaufsdaten"
topic_id: "25931"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Erfassung von Neufahrzeugen, Tageszulassungen und Vorführfahrzeugen > Verkaufsdaten"
---

# Verkaufsdaten

Mit der Funktion setSalesData legen Sie Verkaufsdaten zu einem bestehenden Vorgang an.

Hinweis: Nachdem Sie die Verkaufsdaten angelegt haben, können Sie den Status des Dossiers
mit der Funktion changeContractStatus nach Verkauft ändern.

Parameter setSalesData

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ContractID | Long | Eindeutige Vorgangskennung (DossierId) | numerisch | X |
| Orderdate | Date | Auftragsdatum | Format[YYYY-MM-DD] | X |
| SellerId | Integer | ID des Verkäufers (erhält man durch die Methode [getPossibleContactPersons](#expandblock-25931-d2e963134)Response unter dem Parameter id)  ``` <S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">    <S:Body>       <ns3:getPossibleContactPersonsResponse xmlns:ns3="http://www.dat.eu/myClaim/soap/v2/MyClaimExternalService">          <PossibleContactPersons>             <firstName>Max</firstName>             <id>2781</id>             <name>34, Mustermann</name>             <salutation>titleMr</salutation>             <surname>34</surname>          </PossibleContactPersons>       </ns3:getPossibleContactPersonsResponse>    </S:Body> </S:Envelope> ``` | numerisch | X |
| BusinessType | String | Geschäftsart;Hinweis: Die Werte für die Geschäftsarten legen Sie in den Stammdaten an und holen die Daten mit [getBusinessTypeList](#expandblock-25931-d2e963162).Der Reponseparameter BusinessType muss eingegeben werden  Parameter getBusinessTypeListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | BusinessTypeListResponse | businessTypeListResponse | Enthält vxs:BusinessTypeList als Unterelement |  |  Element vxs:BusinessTypeListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | BusinessTypeList | businessTypeList | Enthält 0 bis n Positionen vxs:BusinessTypeItem als Unterelemente |  |  Element vxs:BusinessTypeList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | BusinessTypeItem | businessTypeItem | Enthält die Geschäftsartendetails |  |  Element vxs:BusinessTypeItem  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | Designation | String | Bezeichnung von Geschäftsarten |  | | UniqueCode | String | Eindeutiger Code |  | | ValidVehicleTypes | String | Fahrzeugarten |  | | BusinessType | Integer | Eindeutige Nummerierung der Geschäftsarten | numerisch | |  |  |
| VehicleGroup | String | Fahrzeuggruppe;  Hinweis: Die Werte für die Fahrzeuggruppen legen Sie in den Stammdaten an und holen die Daten mit [getVehicleGroupList](#expandblock-25931-d2e963189). Der Reponseparameter VehicleGroup muss eingegeben werden.  Bitte beachten Sie, dass die Fahrzeuggruppe, die im Parameter ValidVehicleTypes angegeben ist, mit der Fahrzeugart des Dossiers übereinstimmen muss.  Parameter getVehicleGroupListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupListResponse | vehicleGroupListResponse | Enthält die VehicleGroupList als Unterelement |  |  Element vxs:VehicleGroupListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupList | vehicleGroupList | Enthält 0 bis n Positionen VehicleGroupItem als Unterelemente |  |  Element vxs:VehicleGroupList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | VehicleGroupItem | vehicleGroupItem | Enthält die Fahrzeuggruppendetails |  |  Element vxs:VehicleGroupItem  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | Designation | String | Bezeichnung von Fahrzeuggruppen |  | | UniqueCode | String | Eindeutiger Code |  | | ValidVehicleTypes | String | Fahrzeugarten |  | | VehicleGroup | Integer | Eindeutige Nummerierung der Fahrzeuggruppen. | numerisch | |  |  |
| DeliveryDate | Date | Auslieferungsdatum | Format[YYYY-MM-DD] |  |
| DeliveryBinding | Boolean | true = verbindliche Lieferung false = unverbindliche Lieferung (Default) | true, false |  |
| MileageVehicle | Integer | Fahrzeug Laufleistung |  |  |
| MileageOdometer | Integer | Laufleistung entsprechend der Tachoanzeige (km) |  |  |
| RegistrationNumber | String | Amtliches Kennzeichen |  |  |
| SalesDetails | String | Verkaufsangaben;  Hinweis: Die Werte für die Verkaufsangaben legen Sie in den Stammdaten an und holen die Daten mit [getSalesDetailsList](#expandblock-25931-d2e963310). Der Reponseparameter SalesDetails muss eingegeben werden  Parameter getSalesDetailsListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | SalesDetailsListResponse | salesDetailsListResponse | Enthält die vxs:SalesDetailsList als Unterelement |  |  Element vxs:SalesDetailsListResponse  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | SalesDetailsList | salesDetailsList | Enthält 0 bis n Positionen vxs:SalesDetailsItem als Unterelemente |  |  Element vxs:SalesDetailsList  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | SalesDetailsItem | salesDetailsItem | Enthält die Verkaufsangabendetails |  |  Element vxs:SalesDetailsItem  | Name | Datentyp | Beschreibung | Schreibweise | | --- | --- | --- | --- | | Designation | String | Bezeichnung von Verkaufsangaben |  | | UniqueCode | String | Eindeutiger Code |  | | ValidVehicleTypes | String | Fahrzeugarten |  | | SalesDetails | Integer | Eindeutige Nummerierung der Verkaufsangaben für die Verkaufsmaske. | numerisch | |  |  |
| PaymentAgreements | String | Zahlungsvereinbarungen |  |  |
| OtherAgreements | String | Sonstige Vereinbarungen |  |  |
| RenewVehicleInspection | Date | Datum der erneuten Fahrzeuginspektion | Format[YYYY-MM-DD] |  |
| AgreementOnDeviationsCheck | Boolean | Vereinbarung über Abweichungen | true, false |  |
| ExclusionOfObligationToUpdateCheck | Boolean | Ausschluss der Aktualisierungspflicht | true, false |  |
| UpdateInformationCheck | Boolean | Information zur Aktualisierung | true, false |  |
| InfoReqUpdatesAndInstallation | String | Angaben zu den erforderlichen Aktualisierungen und deren Installation. Nur zulässig falls UpdateInformationCheck gesetzt wurde. |  |  |
| AgreementOnDeviationsList |  | Vereinbarung über Abweichungen |  |  |
| Labelling | Labelling | Auszeichnungsdaten |  |  |

Element AgreementOnDeviationsList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| AgreementOnDeviationItem |  | Vereinbarung über Abweichung |  |  |

Element AgreementOnDeviationItem

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Feature | String | Merkmal der Abweichung |  |  |
| State | String | Tatsächliche Beschaffenheit |  |  |

Element Labelling

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| SalesPriceDiscountPerc | Decimal | Nachlass in Prozent |  |  |
| SalesPriceDiscountNet | Decimal | Nachlass in Euro (Netto) wurde dieser Wert angegeben, ist der Wert immer führend und Werte für SalesPriceDiscountPerc und SalesDiscountGross ignoriert |  |  |
| SalesDiscountGross | Decimal | Nachlass in Euro (Brutto) |  |  |
| TransferCostsNet | Decimal | Überführungskosten (Netto) |  |  |
| TransferCostsGross | Decimal | Überführungskosten (Brutto) |  |  |
| IncludingTransferCosts | Boolean | inklusive Überführungskosten | true = Überführungskosten sind inklusive false = Überführungskosten werden zusätzlich angegeben |  |
| IncidentalCostsNet | Decimal | Zulassungs-/ Nebenkosten (Netto) |  |  |
| IncidentalCostsGross | Decimal | Zulassungs-/ Nebenkosten (Brutto) |  |  |
| IncludingIncidentalCosts | Boolean | inklusive Zulassung-/ Nebenkosten | true = Zulassung-/ Nebenkosten sind inklusive false = Zulassung-/ Nebenkosten werden zusätzlich angegeben |  |
| DisplayPriceNet | Decimal | Auszeichnungspreis (Netto) |  |  |
| DisplayPriceGross | Decimal | Auszeichnungspreis (Brutto) |  |  |
| DeviatingMarketPlacePrice | Boolean | Abweichender Börsenpreis | true = Abweichender Börsenpreis false = kein abweichender Börsenpreis |  |
| DisplayPriceMarketPlaceNet | Decimal | Auszeichnungspreis Börse (Netto) |  |  |
| DisplayPriceMarketPlaceGross | Decimal | Auszeichnungspreis Börse (Brutto) |  |  |
| MinimumSalesPriceNet | Decimal | Mindest-Verkaufspreis (Netto) |  |  |
| MinimumSalesPriceGross | Decimal | Mindest-Verkaufspreis (Brutto) |  |  |
| ResellerPriceNet | Decimal | Wiederverkäuferpreis (Netto) |  |  |
| ResellerPriceGross | Decimal | Wiederverkäuferpreis (Brutto) |  |  |
