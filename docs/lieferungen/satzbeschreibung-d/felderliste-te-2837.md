---
title: "Felderliste technische Zusatzinformationen"
topic_id: "2837"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 3 > Felderliste technische Zusatzinformationen"
---

# Felderliste technische Zusatzinformationen

| Feld | Beschreibung | DB-Feld | Datentyp | Bemerkungen |
| --- | --- | --- | --- | --- |
| DATECode | DAT €uropa-Code | HTUV\_FZA + HTUV\_HST + HTUV\_HT + HTUV\_UT + HTUV\_UTV | C, fix 15 Ziffern | PK; (Fahrzeugart + Hersteller + Haupttyp + Untertyp + 4-stellige Untertypvariante; jede Komponente bei Bedarf links mit Nullen aufgefüllt) |
| Con | Marktindex | XLAN\_ISO\_LKZ\_2 + HTUC\_UTV\_CNR | C, fix 5 Zeichen | PK; alphanumerisch (zweistelliges ISO-Länderkennzeichen + 3-stellige Nummer) |
| BwBZ | Bewertungsbauzeit | MDUB\_BJ | N, 4-stellig | PK(kann aber auch fehlen); DAT-Bauzeit-Verschlüsselung zum Stichtag 1. Mai des Baujahres. |
| PS | PS | MSUT\_PS | N, ####,## |  |
| SKl | Schadstoffklasse | MSUT\_SKL | C, 2 Zeichen |  |
| VerbrMV | Verbrauch Mischverkehr | HTUW\_VERBR\_MI | N, ####,# |  |
| VerbrIO | Verbrauch inner\-orts | HTUW\_VERBR\_IO | N, ####,# | kann auch fehlen |
| VerbrAO | Verbrauch außerorts | HTUW\_VERBR\_AO | N, ####,# | kann auch fehlen |
| CO2MV | CO2-Ausstoß Mischverkehr | HTUW\_CO2 | N, 5-stellig | nur bei FZA 1 – PKW und 2 – Transporter , nur bei Benzin- und Diesel-Fahrzeugen |
| Rf1 | Reifen 1 | MREI\_GROESSE | C, 20 Zeichen | über MDUB\_MREI\_LNR; nicht bei FZA 4 – LKW und 5 – Omnibus |
| Rf2 | Reifen 2 | MREI\_GROESSE | C, 20 Zeichen | über MDUB\_MREI\_LNR\_2; nicht bei FZA 4 – LKW und 5 – Omnibus |
| NPb | Neupreis brutto | MDCN\_NEUPR\_1\_B | N, ###########,# | nicht bei FZA 4 – LKW und 5 – Omnibus |
| NPn | Neupreis Komplettfahrzeug netto | MDCN\_NEUPREIS\_1 | N, ###########,# | nur bei FZA 4 – LKW und 5 – Omnibus, nicht bei HST 570 – Mercedes-Benz |
| CKz | Kennzeichen Neupreis Komplettfahrzeug netto nur Ca-Angabe | MDCN\_KZ\_CA | C, 1 Zeichen | nur bei FZA 4 – LKW, nicht bei HST 570 – Mercedes-Benz |
| NPFgn | Neupreis Fahrgestell netto | MDCN\_NEUPREIS\_2 | N, ###########,# | nur bei FZA 4 – LKW, nicht bei HST 570 – Mercedes-Benz |
| BwJ | Jahr der Bewertungsbauzeit | MDUB\_BJ | N, 4-stellig | kann auch fehlen |
| BwM | Monat der Bewertungsbauzeit |  | N, 2-stellig | 1-12; kann auch fehlen |
| DrMo | Drehmoment in Nm | MSUT\_DM | N, 5 stellig | Kann fehlen |
| DrMoUm | Drehmoment bei Umdrehung | MSUT\_UM\_MI\_BDM | N, 10 stellig | Kann fehlen |
| Tank | Tankinhalt in Liter | MSUT\_TANK | N, 5 stellig | Kann fehlen |
| Laeng | Länge in mm | MSUT\_LAENGE | N, 10 stellig | Kann fehlen |
| Breit | Breite in mm | MSUT\_BREITE | N, 10 stellig | Kann fehlen |
| Hoeh | Höhe in mm | MSUT\_HOEHE | N, 10 stellig | Kann fehlen |
| KmH | Höchstgeschwindigkeit | HTUW\_KMH | N, 5 stellig | Kann fehlen |
| Beschl | Beschleunigung von 0 auf 100 km/h in Sek. | HTUW\_BESCHLEUN | N, ###,# | Kann fehlen |
| MaxVol | Maximalvolumen des Lade- bzw. Gepäckraums als Innenmaß in cdm. | MSUT\_LAD\_V\_MAX | N, 10 stellig | Kann fehlen |
| VolLad | Volumen des Lade- bzw. Gepäackraums als Innenmaß in cdm | MSUT\_LAD\_V | N, 10 stellig | Kann fehlen |
| Leer | Leergewicht in kg | HTUW\_LEER\_GEW | N, 10 stellig | Kann fehlen |
| GrpFor | Gruppierung der Fahrzeuge für die Fahrzeugsegmente, Produktgruppe | MSUT\_FZ\_GRP\_FOR | N, 5 stellig | Kann fehlen |
| AnzAirb | Anzahl Airbags | MSUT\_ANZ\_AIRBAG | N, 5 stellig | Kann fehlen |
| Breit2 | Breite in mm (Garagenmaß) | MSUT\_BREITE\_2 | N, 10 stellig | Kann fehlen |
| GgFzgK | Zul. Gesamtgewicht der Fahrzeugkombination in kg | HTUW\_GES\_GEW\_K | N, 10 stellig | Kann fehlen |
| VerbrMVBiv | Bivalent: Verbrauch Mischverkehr | HTUW\_B\_VERBR\_MI | N, ####,## | nur bei FZA 1 - PKW und 2 - Transporter |
| VerbrAOBiv | Bivalent: Verbrauch außerorts | HTUV\_B\_VERBR\_AO | N, ####,## | nur bei FZA 1 - PKW und 2 - Transporter, kann auch fehlen |
| VerbrIOBiv | Bivalent: Verbrauch innerorts | HTUV\_B\_VERBR\_ST | N, ####,## | nur bei FZA 1 - PKW und 2 - Transporter, kann auch fehlen |
| Tank2 | Alternativer Tankinhalt in Liter | MSUT\_TANK\_2 | N, 5 stellig | Kann fehlen |
| PSElektroMax | Maximale Leistung in PS (Elektromotor) | MSUT\_PS\_M | N, ####,## | Kann fehlen |
| AkkuSpa | Batteriespannung in V (Elektromotor) | MSUT\_AKKU\_SPA | N, ####,# | Kann fehlen |
| AkkuKap | Batteriekapazität in kWh (Elektromotor) | MSUT\_AKKU\_KAP | N, ####,# | Kann fehlen |
| AkkuGew | Batteriegewicht in kg (Elektromotor) | MSUT\_AKKU\_GEW | N, ####,# | Kann fehlen |
| AkkuArt | Art der Batterie (Elektromotor) | MSUT\_AKKU\_ART | C, 100 Zeichen | Kann fehlen |
| LadeSta | Standardladung in V (Elektromotor) | MSUT\_LAD\_STA | N, 5 stellig | Kann fehlen |
| LadedauSta | Ladedauer bei Standardladung in Std. (Elektromotor) | MSUT\_LAD\_STA\_D | N, ##,# | Kann fehlen |
| LadeSch | Schnellladung in V (Elektromotor) | MSUT\_LAD\_SCH | N, 5 stellig | Kann fehlen |
| LadedauSch | Ladedauer bei Schnellladung in Std. (Elektromotor) | MSUT\_LAD\_SCH\_D | N, ##,# | Kann fehlen |
| SteTyp | Ladestromsteckertyp (Elektromotor) | MSUT\_LAD\_ST\_TYP | C, 100 Zeichen | Kann fehlen |
| VerbEl | Stromverbrauch in kWh pro 100 km (Elektromotor) | HTUW\_S\_VERBR | N, ####,# | Kann fehlen |
| ReichwEMo | Reichweite in km (Elektromotor) | HTUW\_REICHW\_EMO | N, 5 stellig | Kann fehlen |
| ReichwGes | Gesamtreichweite in km | HTUW\_REICHW\_GES | N, 5 stellig | Kann fehlen |
| KzPlugin | Kennzeichen, ob ein Plugin-System vorhanden | MSUT\_KZ\_PLUGIN | C, 1 Zeichen | 2 Werte möglich: J oder N |
| KzQuickdr | Kennzeichen, ob ein Quickdrop-System vorhanden | MSUT\_KZ\_QUICKDR | C, 1 Zeichen | 2 Werte möglich: J oder N |
| KzE10 | Kennzeichen für E10 geeignet | MSUT\_KZ\_LOESCH | C, 1 Zeichen | 2 Werte möglich: J oder N |
| MK | ID der Mietwagenklasse | HHMK\_LNR | N, 5 stellig | Kann fehlen |
| MKBenn | Benennung der Mietwagenklasse | HHMK\_BENN | C, 100 Zeichen | Kann fehlen |

PK (Primary Key) bedeutet: Teil der eindeutigen Identifizierung des Datensatzes.
