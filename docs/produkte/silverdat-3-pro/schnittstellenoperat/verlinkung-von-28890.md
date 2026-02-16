---
title: "Verlinkung von Vorgängen"
topic_id: "28890"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Verlinkung von Vorgängen"
---

# Verlinkung von Vorgängen

Bestehende Verlinkungen von Vorgängen werden in den Responses des ValuationServiceN ausgegeben. Über die Funktionen getValuationN, changeValuationN und resetValuation2defaultN werden folgende Informationen zu einem verlinkten Vorgang ausgegeben:

- Claim-ID des verlinkten Vorgangs - contractId
- Auftragstyp des verlinkten Vorgangs - contractType
- Verlinkungsart - linkKind

Diese Informationen werden unter dem Node LinkedContracts unter Dossier ausgegeben.

Eine Verlinkung kann nur zwischen einem Bewertungs- und Kalkulationsauftrag oder einem
Bewertungs- und Glasauftrag bestehen. Die Verlinkung kann nur über die Oberfläche
hergestellt werden. Eine Verlinkung über die Schnittstellen ist nicht möglich.

Auszug aus der Response:

```
<ns1:LinkedContracts>
   <ns1:LinkedContract>
      <ns1:contractId>3054791</ns1:contractId>
      <ns1:contractType>vro_calculation</ns1:contractType>
      <ns1:linkKind>CALC_VAL</ns1:linkKind>
   </ns1:LinkedContract>
</ns1:LinkedContracts>
```
