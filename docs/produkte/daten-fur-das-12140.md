---
title: "Daten für das Verkaufsangebot anlegen"
topic_id: "12140"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Status umbuchen > Daten für das Verkaufsangebot anlegen"
---

# Daten für das Verkaufsangebot anlegen

Mit der Funktion setSalesOffer legen Sie ein Verkaufsangebot zu einem bestehenden Vorgang an.

Parameter setSalesOffer

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ContractID | Long | Eindeutige Vorgangserkennung | numerisch | x |
| SalesOffer | SalesOffer | Daten für das Verkaufsangebot |  | X |

Parameter SalesOffer

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| SalesPriceNet | Decimal | Angebotspreis Netto |  | bedingt |
| SalesPriceGross | Decimal | Angebotspreis Brutto |  | bedingt |
| OfferDate | Date | Angebotsdatum | Format[YYYY-MM-DD] | X |
| SalesOfferNumber | String | Angebotsnummer |  |  |
| GuaranteeDate | Date | Garantiedatum | Format[YYYY-MM-DD] |  |
| ResumbmissionDate | Date | Wiedervorlagedatum | Format[YYYY-MM-DD] |  |
| OfferedBy | Long | ID des Verkäufers (erhält man durch die Methode [getPossibleContactPersons](#expandblock-12140-d2e719337) uner dem Parameter id)  ``` <S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">    <S:Body>       <ns3:getPossibleContactPersonsResponse xmlns:ns3="http://www.dat.eu/myClaim/soap/v2/MyClaimExternalService">          <PossibleContactPersons>             <firstName>Max</firstName>             <id>2781</id>             <name>34, Mustermann</name>             <salutation>titleMr</salutation>             <surname>34</surname>          </PossibleContactPersons>       </ns3:getPossibleContactPersonsResponse>    </S:Body> </S:Envelope> ``` |  |  |
| Titles | String | Anrede |  |  |
| Comments | String | Bemerkung |  |  |
| Agreements | String | Vereinbarung |  |  |
| NextEmissionsTestDate | Date | Nächste Abgasuntersuchung. Wird nur angezeigt, wenn Country nicht auf Deutschland gesetzt ist. | Format[MM-YYYY] |  |
| NextVehicleInspectionDate | Date | Datum der nächsten Hauptuntersuchung. | Format[MM-YYYY] |  |
| RenewEmissionVehicleInspectionCheck | Boolean | Hauptuntersuchung und Abgasuntersuchung erneuern | true false |  |
