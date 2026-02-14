---
title: "Verkaufsangebote"
topic_id: "25932"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Erfassung von Neufahrzeugen, Tageszulassungen und Vorführfahrzeugen > Verkaufsangebote"
---

# Verkaufsangebote

Mit der Funktion setSalesOffer legen Sie ein Verkaufsangebot zu einem bestehenden Vorgang an.

Parameter setSalesOffer

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ContractID | Long | Eindeutige Vorgangserkennung | numerisch | X |
| SalesOffer | SalesOffer |  |  |  |

Parameter SalesOffer

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ResubmissionDate | Date | Wiedervorlagedatum | Format[YYYY-MM-DD] |  |
| OfferDate | Date | Angebotsdatum | Format[YYYY-MM-DD] | X |
| OfferedBy | Long | ID des Verkäufers (erhält man durch die Methode getPossibleContactPersons uner dem Parameter id)  ``` <S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">    <S:Body>       <ns3:getPossibleContactPersonsResponse xmlns:ns3="http://www.dat.eu/myClaim/soap/v2/MyClaimExternalService">          <PossibleContactPersons>             <firstName>Max</firstName>             <id>2781</id>             <name>34, Mustermann</name>             <salutation>titleMr</salutation>             <surname>34</surname>          </PossibleContactPersons>       </ns3:getPossibleContactPersonsResponse>    </S:Body> </S:Envelope> ``` |  |  |
| Titles | String | Anrede |  |  |
| Comments | String | Bemerkung |  |  |
| SalesPriceNet | Decimal | Verkaufspreis (Netto) |  | bedingt |
| SalesPriceGross | Decimal | Verkaufspreis (Brutto) |  | bedingt |
| SalesOfferNumber | String | Angebotsnummer |  |  |
| GuaranteeDate | Date | Garantie | Format[YYYY-MM-DD] |  |
| Agreements | String | Vereinbarung |  |  |
| Labelling | Labelling | Auszeichnunsdaten |  |  |

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
