---
title: "Response setValueInfluencingFactors"
topic_id: "25289"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Benutzerdefinierte Handelsspanne > Benutzerdefinierte Handelsspanne anlegen > Response setValueInfluencingFactors"
---

# Response setValueInfluencingFactors

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns5:setValueInfluencingFactorsResponse xmlns:ns5="http://www.dat.de/services/Dossier1N">
         <setValueInfluencingFactorsResponse>
            <DossierId>2188609</DossierId>
            <VehicleType>5</VehicleType>
            <NominalDaysOnLot origin="user" xmlns:ns1="http://www.dat.de/vxs">150</NominalDaysOnLot>
            <DatNominalDaysOnLot>120</DatNominalDaysOnLot>
            <SalesPriceNet origin="dat" xmlns:ns1="http://www.dat.de/vxs">26129.98</SalesPriceNet>
            <SalesPriceGross origin="dat" xmlns:ns1="http://www.dat.de/vxs">26654.36</SalesPriceGross>
            <MarginFromFactorsNet>600.00</MarginFromFactorsNet>
            <MarginFromFactorsGross>714.00</MarginFromFactorsGross>
            <ValueInfluencingFactorList>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927860</ValueInfluencingFactorId>
                  <IntoAccountCheck>true</IntoAccountCheck>
                  <Designation>Aufbereitungskosten</Designation>
                  <Occurrence>Einmaliger Faktor</Occurrence>
                  <Category>Kostenfaktor</Category>
                  <Period>Gesamte Standzeit</Period>
                  <DatValueNet>142.86</DatValueNet>
                  <DatValueGross>170.00</DatValueGross>
                  <ValueNet origin="user" xmlns:ns1="http://www.dat.de/vxs">100.00</ValueNet>
                  <ValueGross origin="user" xmlns:ns1="http://www.dat.de/vxs">119.00</ValueGross>
               </ValueInfluencingFactorItem>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927857</ValueInfluencingFactorId>
                  <IntoAccountCheck>true</IntoAccountCheck>
                  <Designation>Gemeinkosten</Designation>
                  <Occurrence>Wiederkehrender Faktor</Occurrence>
                  <Category>Kostenfaktor</Category>
                  <Period>Monatlich</Period>
                  <DatValueNet>302.52</DatValueNet>
                  <DatValueGross>360.00</DatValueGross>
                  <ValueNet origin="user" xmlns:ns1="http://www.dat.de/vxs">100.00</ValueNet>
                  <ValueGross origin="user" xmlns:ns1="http://www.dat.de/vxs">119.00</ValueGross>
               </ValueInfluencingFactorItem>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927862</ValueInfluencingFactorId>
                  <IntoAccountCheck>true</IntoAccountCheck>
                  <Designation>Gewinn</Designation>
                  <Occurrence>Einmaliger Faktor</Occurrence>
                  <Category>Gewinnfaktor</Category>
                  <Period>Gesamte Standzeit</Period>
                  <PercentageFromSP>3</PercentageFromSP>
                  <DatValueNet>671.96</DatValueNet>
                  <DatValueGross>799.63</DatValueGross>
                  <ValueNet origin="user" xmlns:ns1="http://www.dat.de/vxs">100.00</ValueNet>
                  <ValueGross origin="user" xmlns:ns1="http://www.dat.de/vxs">119.00</ValueGross>
               </ValueInfluencingFactorItem>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927858</ValueInfluencingFactorId>
                  <IntoAccountCheck>true</IntoAccountCheck>
                  <Designation>Kapitalzinsen</Designation>
                  <Occurrence>Wiederkehrender Faktor</Occurrence>
                  <Category>Kostenfaktor</Category>
                  <Period>Jährlich</Period>
                  <PercentageFromSP>6.5</PercentageFromSP>
                  <DatValueNet>485.30</DatValueNet>
                  <DatValueGross>577.51</DatValueGross>
                  <ValueNet origin="user" xmlns:ns1="http://www.dat.de/vxs">100.00</ValueNet>
                  <ValueGross origin="user" xmlns:ns1="http://www.dat.de/vxs">119.00</ValueGross>
               </ValueInfluencingFactorItem>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927861</ValueInfluencingFactorId>
                  <IntoAccountCheck>true</IntoAccountCheck>
                  <Designation>Verkäuferprovision</Designation>
                  <Occurrence>Einmaliger Faktor</Occurrence>
                  <Category>Provisionsfaktor</Category>
                  <Period>Gesamte Standzeit</Period>
                  <PercentageFromSP>2.5</PercentageFromSP>
                  <DatValueNet>559.97</DatValueNet>
                  <DatValueGross>666.36</DatValueGross>
                  <ValueNet origin="user" xmlns:ns1="http://www.dat.de/vxs">100.00</ValueNet>
                  <ValueGross origin="user" xmlns:ns1="http://www.dat.de/vxs">119.00</ValueGross>
               </ValueInfluencingFactorItem>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927859</ValueInfluencingFactorId>
                  <IntoAccountCheck>true</IntoAccountCheck>
                  <Designation>Wertverlust</Designation>
                  <Occurrence>Wiederkehrender Faktor</Occurrence>
                  <Category>Kostenfaktor</Category>
                  <Period>Jährlich</Period>
                  <PercentageFromSP>8</PercentageFromSP>
                  <DatValueNet>597.30</DatValueNet>
                  <DatValueGross>710.79</DatValueGross>
                  <ValueNet origin="user" xmlns:ns1="http://www.dat.de/vxs">100.00</ValueNet>
                  <ValueGross origin="user" xmlns:ns1="http://www.dat.de/vxs">119.00</ValueGross>
               </ValueInfluencingFactorItem>
            </ValueInfluencingFactorList>
         </setValueInfluencingFactorsResponse>
      </ns5:setValueInfluencingFactorsResponse>
   </S:Body>
</S:Envelope>
```
