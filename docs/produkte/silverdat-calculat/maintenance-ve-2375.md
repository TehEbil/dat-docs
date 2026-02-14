---
title: "MAINTENANCE (Veraltet!)"
topic_id: "2375"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Datentypen > datProcessInfo und DVNInfo (Veraltet!) > MAINTENANCE (Veraltet!)"
---

# MAINTENANCE (Veraltet!)

Definiert Materialkosten bei der Wartungskalkulation. Die Wartungskalkulation ist
durch das type Attribut verfeinert. Es gibt die folgenden Typen:

|  |  |
| --- | --- |
| TYPE | Bedeutung |
| LABOUR (default) | Arbeitsposition |
| MATERIAL | Materialposition |
| INTERVAL | Wartungsintervall |

Attribute

|  |  |  |  |
| --- | --- | --- | --- |
| Attribute | Typ | Bedeutung | Wert |
| amount | Material |  | Decimal |
| price | Material |  | Decimal |

Beispiel für Material der Wartungskalkulation

```
<!-- Maintenance -->
<datProcessInfo method="MAINTENANCE" type="INTERVAL">
<datProcessId>94030</datProcessId>
</datProcessInfo>

<!-- Zahnriemen der Motorsteuerung austauschen -->
<datProcessInfo method="MAINTENANCE" type="LABOUR">
<datProcessId>81715</datProcessId>
</datProcessInfo>

<!-- REP.-SATZ ZAHNRIEMEN -->
<datProcessInfo method="MAINTENANCE" type="MATERIAL">
<datProcessId>81715</datProcessId>
<amount>2</amount>
<price>130.90</price>
</datProcessInfo>
```
