---
title: "Fahrzeugbeschreibung anlegen"
topic_id: "12145"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Verwalten der Fahrzeugbeschreibung > Fahrzeugbeschreibung anlegen"
---

# Fahrzeugbeschreibung anlegen

Mit der Funktion setVehicleColorUpholstery legen Sie eine Fahrzeugbeschreibung (Daten zum Polster und zur Farbe ) zu einem bestehenden
Vorgang an. Diese Methode ist für folgende Anwendungen verfügbar: SilverDAT 3 valuateExpert/valuateExpertPlusPartner .

Parameter setVehicleColorUpholstery

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Eindeutige Vorgangserkennung | numerisch | x |
| ColorTypeN | String | Farbschema | anthracite beige blue bordeaux brown bronze yellow gold gray green orange pink red black silver turquoise violet white |  |
| Color | String | Fahrzeugfarbe |  |  |
| ColorVariantN | String | Farbausprägung | normal light dark |  |
| LacquerTypeN | String | Lackart | normal metallic special |  |
| CushionTypeN | String | Polsterart | fabric  fabric/leather alcantara velours leatherette leather |  |
| CushionColorTypeN | String | Polsterschema | tan anthrancite blue brown creme yellow gray green red black white |  |
| CushionColor | String | Polsterfarbe |  |  |
| CushionTypeName | String | Polsterbezeichnung |  |  |
