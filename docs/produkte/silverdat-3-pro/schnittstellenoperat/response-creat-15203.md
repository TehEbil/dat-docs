---
title: "Response createValuationN - variant with incomplete vehicle identification"
topic_id: "15203"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Erstellen einer neuen Bewertung in der Anwendung > Response createValuationN - variant with incomplete vehicle identification"
---

# Response createValuationN - variant with incomplete vehicle identification

###### Response createValuationN - variant with incomplete vehicle identification Eine Beschreibung aller Response-Parameter finden Sie unter [Datenaustauschformat VXS](../../../vxs/aktenzeichenvorgange-doss/index.md). ``` <S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">    <S:Body>       <ns4:createValuationNResponse xmlns:ns4="http://www.dat.eu/myClaim/soap/v2/ValuationServiceN">          <VXS type="incompleteValuation">             <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">                <ns1:DossierId>1292283</ns1:DossierId>             </ns1:Dossier>          </VXS>       </ns4:createValuationNResponse>    </S:Body> </S:Envelope> ```
