---
title: "Aufbauten (UpperBodies)"
topic_id: "2894"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Aufbauten (UpperBodies)"
---

# Aufbauten (UpperBodies)

<UpperBodies> ist ein Unter-Element von <Vehicle>. Im <UpperBodies>-Element können beliebig viele <UpperBody>-Elemente enthalten sein. Diese enthalten die Informationen zum Fahrzeugaufbau.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| UpperBodyType | integer | Aufbauart |
| (Dat)UpperBodyTypeName | string | Aufbauartbezeichnung |
| Manufacturer | integer | Hersteller (momentan nur 999 = Sammelhersteller verfügbar) |
| (Dat)ManufacturerName | string | Aufbauherstellerbezeichnung |
| MainModel | integer | Haupttyp |
| (Dat)MainModelName | string | Typbezeichnung |
| SubModel | integer | Untertyp |
| (Dat)SubModelName | string | Modellbezeichnung |
| InitialRegistration | date | Erstzulassung |
| IdentificationNumber | string | Identifizierungsnummer |
| UpperBodyColor | string | Aufbaufarbe |
| PaintLabelDescription | string | Beschreibung von Lackierung und  Beschriftung |
| (Dat)OriginalPrice | decimal | Neupreis netto |
| (Dat)OriginalPriceGross | decimal | Neupreis brutto |
| (Dat)GeneralCondition | decimal | Erhaltungszustand |
| (Dat)BasePrice | decimal | Basiswert netto |
| (Dat)BasePriceGross | decimal | Basiswert brutto |
| (Dat)SalesPrice | decimal | Verkaufspreis netto |
| (Dat)SalesPriceGross | decimal | Verkaufspreis brutto |
| IsDisengaged | boolean | freier Aufbau |
