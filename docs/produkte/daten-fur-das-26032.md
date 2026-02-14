---
title: "Daten für das Ankaufsangebot anlegen"
topic_id: "26032"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Status umbuchen > Daten für das Ankaufsangebot anlegen"
---

# Daten für das Ankaufsangebot anlegen

Mit der Funktion setPurchaseOffer legen Sie ein Ankaufsangebot zu einem bestehenden Vorgang an.

Parameter setPurchaseOffer

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ContractID | Long | Eindeutige Vorgangserkennung | numerisch | x |
| PurchaseOffer | PurchaseOffer | Daten für das Verkaufsangebot |  | X |

Parameter PurchaseOffer

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| PurchasePriceNet | Decimal | Angebotspreis Netto |  | bedingt |
| PurchasePriceGross | Decimal | Angebotspreis Brutto |  | bedingt |
| ResubmissionDate | Date | Wiedervorlagedatum | Format[YYYY-MM-DD] |  |
| OfferDate | Date | Angebotsdatum | Format[YYYY-MM-DD] | X |
| OfferedBy | Long | ID des Verkäufers (erhält man durch die Methode [getPossibleContactPersons](#expandblock-26032-d2e968246) uner dem Parameter id)  ``` <S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">    <S:Body>       <ns3:getPossibleContactPersonsResponse xmlns:ns3="http://www.dat.eu/myClaim/soap/v2/MyClaimExternalService">          <PossibleContactPersons>             <firstName>Max</firstName>             <id>2781</id>             <name>34, Mustermann</name>             <salutation>titleMr</salutation>             <surname>34</surname>          </PossibleContactPersons>       </ns3:getPossibleContactPersonsResponse>    </S:Body> </S:Envelope> ``` |  | X |
| Titles | String | Anrede |  |  |
| Comments | String | Bemerkung |  |  |
| PurchaseOfferNumber | String | Angebotsnummer |  |  |
