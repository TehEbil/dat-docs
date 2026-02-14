---
title: "Zukunftsprognose auf ein Jahr erweitert"
topic_id: "31528"
breadcrumb: "Technische Informationen > Ausgabe Nr. 94 Dezember 2025 > Fahrzeugbewertung > valuateExpert/valuateExpertPlusPartner > Erweiterungen > Zukunftsprognose auf ein Jahr erweitert"
---

# Zukunftsprognose auf ein Jahr erweitert

Die Zukunftsprognose wurde für die Datenländer Deutschland, Österreich und Spanien
auf ein Jahr erweitert.

Im Node Valuation kann im Parameter PrognosisDate ab sofort ein Datum bis zu 12 Monate in die Zukunft übergeben werden.

Die Fehlermeldung mit dem Faultcode dat:validation.futurePrognosis.dateInTheFuture wurde so angepasst, dass für die Datenländer Deutschland, Österreich und Spanien
nun der folgende faultstring ausgegeben wird:

"Die Zukunftsprognose ist nur bis max. 12 Monate in die Zukunft möglich."

Für alle anderen Datenländer wird weiterhin der folgende faultstring ausgegeben:

"Die Zukunftsprognose ist nur bis max. 6 Monate in die Zukunft möglich."
