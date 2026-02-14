---
title: "Exportieren von manuellen Positionen"
topic_id: "11885"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Exportieren von manuellen Positionen"
---

# Exportieren von manuellen Positionen

Mit der Schnittstellenfunktion exportManualPositions() werden die eigenen, wiederkehrenden "Manuelle Positionen" (Material- und/oder Lohnpositionen)
exportiert.

Parameter

Es ist keine Parameterübergabe erforderlich. Das Request muss leer abgeschickt werden.

Rückgabe

Als Antwort wird eine Liste von Kategorien der enthaltenen manuellen Positionen zurückgegeben.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [manualPositions](#showid/11910 "Manuelle Positionen manualPositions") | complexType    [DatCategory](#showid/11911 "DatCategory")  [DatPosition](#showid/11912 "DatPosition") | Liste von Kategorien mit Namen und darunterliegenden manuellen Positionen |
