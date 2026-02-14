---
title: "getData Response (Beispiel)"
topic_id: "14149"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Authentifizierung der SilverDAT Webservices > Delegated Sign On (DSO) Service > getData Response (Beispiel)"
---

# getData Response (Beispiel)

Die Antwort beinhaltet ein base64-codiertes und mittels publicKey verschlüsseltes anonymes JSON-Object.

Der zur Entschlüsselung benötigte privateKey hat ausschließlich der DSO-Partner.

Beispiel:

| Element | Inhalt |
| --- | --- |
| Response (base64-codiert) | HpE2cSX5agbvDUIgPzTmvtBdyNmuiABtKp/QMZk7t0QWEjHvAuwq81rrk/GIlDzVsqtfb5mLC4k2CansxLq1FE1tFg1NDA2XuKGvpYvX/bKF1ROOMCDiZGaO7pnBWpEP7XocyQk0JSj9cb6PLe5crzQwG25uDtYbeNJ32uk5qXYRp1yygTSuRNaBV1OKBZAvgCoTD4bVT8g6+bo2DWgTsvB4gnroodk6ETGj+mBgbcCCO0/6DEZ4efGsuRWW6DoSjsstiODe2bHEYOKCnWNq/PEtVVSR3FtxW/11V1qaa+/vH+Wb2Z6jXpDkK/CJq1GyBJ+pb1Bq7dHe9FzVTK2m1sJ4RTFy5Bik09EPP2Njps+LNmv0fchPiotJybnQdBlWC25+vKsiFqFoHMCwSQoyywA2Jsw9roJtrEe0cUD9N3HuCq4PNKVmj15iFxpPeb/B/Kjqw9U9F5fFbG1tgpcp08qXhfoU8WxqSbgrXq26pYZih++8y8sol1rzEstzxNCajHooOjITrxtU71BBaUCQT7AcFdXvMnCit/cEs6fZcpZegwSuj48cY4+vGTCezRt8wvAg/ugp/JrqqY0KEI76It+KWxRFOkuGqe9ycY6rL1um5yyWZ2Qpo6aMKeMrLSfWy0vOl2BFSQqFUoc4cpYSYJ8wfAa9IB4TSKd4LEaugTw= |
| DSO-Partner: base64-decode der Antwort | (binärer Inhalt) |
| DSO-Partner: decrypt mit privateKey | { "DatCustomerIdHash":"EF1B49C78F9DE6451A9C6342B84C2CC9", "DatUserIdHash":"790A163C9AB4FA20AC95169D3DE5B25D" } |
