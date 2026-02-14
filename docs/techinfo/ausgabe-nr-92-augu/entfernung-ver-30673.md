---
title: "Entfernung veralteter Elemente unter TradingActivity"
topic_id: "30673"
breadcrumb: "Technische Informationen > Ausgabe Nr. 92 August 2025 > Fahrzeugbewertung > valuateExpert/valuateExpertPlusPartner > Abkündigungen > Entfernung veralteter Elemente unter TradingActivity"
---

# Entfernung veralteter Elemente unter TradingActivity

Untenstehende Parameter unter TradingActivity werden mit dem Release Oktober 2025 endgültig aus dem VXS-Austauschformat entfernt.

Parameter unter Purchase

- CustomerId
- TaxationType
- UserId
- AcceptanceType

Parameter unter Admission

- CustomerId
- PurchasePriceNet
- PurchasePriceGross
- TaxationType
- BusinessType
- AcceptanceInfo
- Buyer
- FollowUpBusiness

Parameter unter FollowUpBusiness

- FollowUpBusinessType
- BusinessType
- VehicleNo
- VehicleIdentNo
- KbaKey
- Details

Parameter unter Sale

- CustomerId
- LicenseNumber
- ProcedureName
- RenewMot
- Purchaser
- Seller
- SalesType
- PayementAgreements

Bitte führen Sie in Ihren Anwendungen die erforderlichen Anpassungen durch, damit
auch nach dem Update alles erwartungsgemäß funktioniert.
