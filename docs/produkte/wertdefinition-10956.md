---
title: "Wertdefinitionen anlegen zu einem Produkt in ExpertPlusPartner"
topic_id: "10956"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Wertdefinitionen anlegen zu einem Produkt in ExpertPlusPartner"
---

# Wertdefinitionen anlegen zu einem Produkt in ExpertPlusPartner

Mit der Funktion setBasecheckValueDefinitionDetails/setLeasingReturnValueDefinitionDetails/setConditionReportValueDefinitionDetails/setValuationExpertiseValueDefinitionDetails/setEstimationCertificateValueDefinitionDetails legen Sie Wertedefinitionsdaten zu einem Produkt (Grundüberprüfung, Leasingrückgabe, Zustandsbericht, Bewertungsgutachten oder Schätzurkunde) zu einem bestehenden Vorgang an.

Parameter   
setBasecheckValueDefinitionDetails  
setLeasingReturnValueDefinitionDetails  
setConditionReportValueDefinitionDetails  
setValuationExpertiseValueDefinitionDetails  
setEstimationCertificateValueDefinitionDetails

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Eindeutige Vorgangserkennung | numerisch | x |
| ConfirmValue | Boolean | Bestätigung des Verkaufspreises gemäß Festlegung Sachverständiger in Brutto |  |  |
| ExpertDefinedSalesValueGross | Decimal | Verkaufspreis gemäß Festlegung Sachverständiger(Brutto) |  |  |
| RemarkRegardingOtherSource | String | Bemerkung sonstige Quelle |  |  |
| SumAccordingToOtherGross | Decimal | Verkaufspreis aus sonstiger Quelle in Brutto |  |  |
| SumAsOfWebScanGross | Decimal | Verkaufspreis aus webScan in Brutto |  |  |
