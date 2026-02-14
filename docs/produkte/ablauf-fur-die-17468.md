---
title: "Ablauf für die Abfrage von kostenpflichtigen rückwirkenden Bewertungen (SilverDAT
      3 valuateExpert, valuateExpertPlusPartner)"
topic_id: "17468"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Ablauf für die Abfrage von kostenpflichtigen rückwirkenden Bewertungen (SilverDAT 3 valuateExpert, valuateExpertPlusPartner)"
---

# Ablauf für die Abfrage von kostenpflichtigen rückwirkenden Bewertungen (SilverDAT
      3 valuateExpert, valuateExpertPlusPartner)

#### Ablauf für die Abfrage von kostenpflichtigen rückwirkenden Bewertungen (SilverDAT 3 valuateExpert, valuateExpertPlusPartner)

Für SilverDAT valuateExpert und valuateExpertPlusPartner gibt es eine Besonderheit bei der Abfrage von kostenpflichtigen rückwirkenden Bewertungen,
die mit den Funktionen createDossierN oder changeDossierN ausgeführt werden.  
Bei kostenpflichtigen rückwirkenden Bewertungen handelt es sich um Bewertungen, bei
denen der Stichtag für die Bewertung DeterminatedDate im vorletzten Monat oder noch weiter zurückliegt.

Bitte beachten Sie, dass sich Änderungen bei Abfragen ergeben, bei denen es sich um
kostenpflichtige rückwirkende Bewertungen handelt. Dies ist bei der Vorgabe eines
Stichtags für die Bewertung DeterminatedDate der Fall, der mindestens zwei Monatswechsel beinhaltet. Das ist zum Beispiel der
Fall, wenn der aktuelle Monat Februar 2023 ist und der Stichtag für die Bewertung
sich im Dezember 2022 oder früher befindet.

Der neue Ablauf sieht wie folgt aus:

1. Sie geben einen Stichtag für die Bewertung an, der entsprechend weit in der Vergangenheit
liegt. Die erste Abfrage liefert dann den Hinweis auf die zusätzlichen Kosten und
den Approval-Wert faultApprovalValue.

|  |  |
| --- | --- |
|  | Abfrage mit createDossierN oder changeDossierN |
| Request | ``` <vxs:Valuation>    <vxs:DeterminatedDate>2022-11-02</vxs:DeterminatedDate> </vxs:Valuation> ``` |
| Response | ``` <S:Fault>    <faultcode xmlns:dat="http://www.dat.de">dat:validation.approval.message</faultcode>    <faultstring>Der ausgewählte Stichtag führt zu einer kostenpflichtigen rückwirkenden Bewertung. Soll die rückwirkende Bewertung tatsächlich durchgeführt werden?</faultstring>    <faultactor>de.dat.sphinx.valadv.trading.vxs.DossierNTradingVxsImportConverter</faultactor>    <detail>       <faultApprovalValue>98167fc05c778ce14fb3a6adac0d2f7d3842eae83f0193e0407b5eab73c1e65a</faultApprovalValue>    </detail> </S:Fault ``` |

2. Sie übernehmen den Approval-Wert faultApprovalValue in den Request und fragen erneut ab, falls Sie den zusätzlichen Kosten zustimmen.
Der Response liefert dann das Bewertungsergebnis zurück. Bitte beachten Sie, dass
der Approval-Wert nur eine Stunde lang gültig ist.

|  |  |
| --- | --- |
|  | Bewertung mit createDossierN oder changeDossierN |
| Request | ``` <vxs:Valuation>        <vxs:Version>V1.1</vxs:Version>    <vxs:DeterminatedDate>2021-10-02</vxs:DeterminatedDate>    <vxs:Approval>98167f...c1e65a</vxs:Approval> </vxs:Valuation> ``` |
| Response | ``` <ns1:Valuation>     <ns1:OriginalPrice origin="dat">32590</ns1:OriginalPrice>     ...     <ns1:SignDeterminatedDate>true</ns1:SignDeterminatedDate>     <ns1:DeterminatedDate>2021-10-02+02:00</ns1:DeterminatedDate>     <vxs:Approval>98167f...c1e65a</vxs:Approval>     ... </ns1:Valuation> ``` |
