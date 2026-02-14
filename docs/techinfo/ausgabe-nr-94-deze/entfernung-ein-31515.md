---
title: "Entfernung einer schema-Datei im VehicleUserPropertiesService"
topic_id: "31515"
breadcrumb: "Technische Informationen > Ausgabe Nr. 94 Dezember 2025 > Fahrzeugbewertung > valuateExpert/valuateExpertPlusPartner > Abkündigungen > Entfernung einer schema-Datei im VehicleUserPropertiesService"
---

# Entfernung einer schema-Datei im VehicleUserPropertiesService

Mit dem ersten Release im Jahr 2026 wird es eine Anpassung der Schema-Dateien des
VehicleUserPropertiesService geben.

Die Inhalte der Dateien

```
<xsd:import namespace="http://www.dat.de/vxs" schemaLocation="https://www.dat.de/valuateNG/soap/VehicleUserPropertiesService/VehicleUserPropertiesService_schema1.xsd"/>
<xsd:import namespace="http://sphinx.dat.de/services/VehicleUserPropertiesService" schemaLocation="https://www.dat.de/valuateNG/soap/VehicleUserPropertiesService/VehicleUserPropertiesService_schema2.xsd"/>
```

werden in einer Datei zusammengeführt.

Diese Datei wird dann als

```
<xsd:import namespace="http://sphinx.dat.de/services/VehicleUserPropertiesService" schemaLocation="https://www.dat.de/valuateNG/soap/VehicleUserPropertiesService/VehicleUserPropertiesService_schema1.xsd"/>
```

bereitgestellt.

Bitte planen Sie die entsprechenden Anpassungen zum ersten Release im Jahr 2026 ein,
sodass auch nach dem Update alles erwartungsgemäß funktioniert.
