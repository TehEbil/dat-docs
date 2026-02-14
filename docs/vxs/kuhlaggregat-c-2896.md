---
title: "Kühlaggregat (CoolingUnit)"
topic_id: "2896"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Aufbauten (UpperBodies) > Kühlaggregat (CoolingUnit)"
---

# Kühlaggregat (CoolingUnit)

<CoolingUnit> ist ein Unter-Element von <UpperBody> und enthält die Daten des Kühlaggregats (nur bei LKW-Aufbauten).

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| Manufacturer | Integer | Hersteller |
| ManufacturerName | String | Herstellerbezeichnung |
| MainModel | Integer | Modell |
| MainModelName | String | Modellbezeichnung |
| InitialRegistration | Date | Erstzulassung |
| (Dat)OriginalPrice | Decimal | Neupreis |
| (Dat)OriginalPriceGross | Decimal | Neupreis (brutto) |
| (Dat)GeneralCondition | Decimal | Erhaltungszustand |
| (Dat)SalesPrice | Decimal | Verkaufspreis |
| (Dat)SalesPriceGross | Decimal | Verkaufspreis (brutto) |
| DriveType | String | Antriebsart; Kommaseparierte Liste, Trennzeichen=;  gasoline engine = Benzinmotor;  diesel engine = Dieselmotor;  electric motor = Elektromotor;  generator = Generator;  hydraulics = Hydraulik;  compressor = Kompressor;  vehicle engine = Lkw-Motor;  power connection = Netzanschluss |
| Usage | String | Verwendung; Kommaseparierte Liste, Trennzeichen=;  heating = heizen  cooling = kühlen |
| (Dat)MinRecommendedBodyLength | Integer | Minimale empfohlene Aufbaulänge in mm |
| (Dat)MaxRecommendedBodyLength | Integer | Maximale empfohlene Aufbaulänge in mm |
