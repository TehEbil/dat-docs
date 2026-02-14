---
title: "Request exportRentalOffers"
topic_id: "15681"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenprotokoll erstellen > Request exportRentalOffers"
---

# Request exportRentalOffers

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ren="http://sphinx.dat.de/services/RentalPricesService">
   <soapenv:Header/>
   <soapenv:Body>
      <ren:exportRentalOffers>
         <ExportRentalOffersRequest>
            <Locale country="DE" datCountryIndicator="DE" language="de"/>
            <!--Optional:-->
            <DATECode>019051080040002DE0025430</DATECode>
            <!--Optional:-->
            <rentalCarClass></rentalCarClass>
            <!--Optional:-->
            <VIN></VIN>
            <firstRegistration>2015-10-01</firstRegistration>
            <!--Optional:-->
            <beginnigOfRental>2020-04-24</beginnigOfRental>
            <!--Optional:-->
            <endOfRental>2020-04-26</endOfRental>
            <postalCode>73760</postalCode>
            <!--Optional:-->
            <duration></duration>
            <!--Optional:-->
            <radius>10</radius>
            <!--Optional:-->
            <priceType></priceType>
            <!--Optional:-->
            <fileReference>my file reference</fileReference>
            <!--Optional:-->
            <damageNumber>my damage number</damageNumber>
            <!--Optional:-->
            <specificConditions>false</specificConditions>
            <!--Optional:-->
            <deliveryInTown></deliveryInTown>
            <!--Optional:-->
            <deliveryOutOfTown></deliveryOutOfTown>
            <!--Optional:-->
            <emergencyFee></emergencyFee>
            <!--Optional:-->
            <oneWayRental></oneWayRental>
            <!--Optional:-->
            <deductibleOf0></deductibleOf0>
            <!--Optional:-->
            <deductibleOf100></deductibleOf100>
            <!--Optional:-->
            <deductibleOf150></deductibleOf150>
            <!--Optional:-->
            <deductibleOf300></deductibleOf300>
            <!--Optional:-->
            <deductibleOf450></deductibleOf450>
            <!--Optional:-->
            <additionalDriver></additionalDriver>
            <!--Optional:-->
            <driverUnder25></driverUnder25>
            <!--Optional:-->
            <winterTire></winterTire>
            <!--Optional:-->
            <navigationDevice></navigationDevice>
            <!--Optional:-->
            <trailerHitch></trailerHitch>
            <!--Optional:-->
            <snowChains></snowChains>
            <!--Optional:-->
            <roofRack></roofRack>
            <!--Optional:-->
            <withoutAdvanceFinancing><withoutAdvanceFinancing>
            <!--Optional:-->
            <drivingSchoolEquipment></drivingSchoolEquipment>
            <!--Optional:-->
            <openEndRentalPeriod></openEndRentalPeriod>
            <!--Optional:-->
            <minimumAdvanceBookingPeriod></minimumAdvanceBookingPeriod>
            <!--Optional:-->
            <withoutDriverMinimumAge></withoutDriverMinimumAge>
         </ExportRentalOffersRequest>
      </ren:exportRentalOffers>
   </soapenv:Body>
</soapenv:Envelope>
```
