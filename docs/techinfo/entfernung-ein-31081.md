---
title: "Entfernung einer schema-Datei im ValuationVehiclePropertiesService"
topic_id: "31081"
breadcrumb: "Technische Informationen > Ausgabe Nr. 93 September 2025 > Fahrzeugbewertung > SilverDAT 3 PRO > Abkündigungen > Entfernung einer schema-Datei im ValuationVehiclePropertiesService"
---

# Entfernung einer schema-Datei im ValuationVehiclePropertiesService

Mit dem ersten Release im Jahr 2026 wird es eine Anpassung der Schema-Dateien des
ValuationVehiclePropertiesService geben.

Die Inhalte der Dateien

```
<xsd:import namespace="http://www.dat.eu/myClaim/soap/v2/ValuationVehiclePropertiesService" schemaLocation="https://www.dat.de/myClaim/soap/v2/ValuationVehiclePropertiesService/ValuationVehiclePropertiesService_schema1.xsd"/>
<xsd:import namespace="http://www.dat.de/vxs" schemaLocation="https://www.dat.de/myClaim/soap/v2/ValuationVehiclePropertiesService/ValuationVehiclePropertiesService_schema2.xsd"/>
```

werden in einer Datei zusammengeführt.

Diese Datei wird dann als

```
<xsd:import namespace="http://www.dat.eu/myClaim/soap/v2/ValuationVehiclePropertiesService" schemaLocation="https://www.dat.de/myClaim/soap/v2/ValuationVehiclePropertiesService/ValuationVehiclePropertiesService_schema1.xsd"/>
```

bereitgestellt.

Bitte planen Sie die entsprechenden Anpassungen zum ersten Release im Jahr 2026 ein,
sodass auch nach dem Update alles erwartungsgemäß funktioniert.
