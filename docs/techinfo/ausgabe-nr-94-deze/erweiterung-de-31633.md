---
title: "Erweiterung der Stammnummer für die Schweiz"
topic_id: "31633"
breadcrumb: "Technische Informationen > Ausgabe Nr. 94 Dezember 2025 > Fahrzeugidentifikation > Abkündigungen > Erweiterung der Stammnummer für die Schweiz"
---

# Erweiterung der Stammnummer für die Schweiz

Ab Jahresbeginn 2026 wird es in der Schweiz auch Stammnummern geben, die anstelle
9 dann 12 Stellen haben, Beispielsweise "136.936.153.123". Dieses betrifft die Schnittstellenfunktion
getVehicleIdentificationByCodeSwitzerland.

Zur Ausgabe der Werte mit der neuen Länge wurde im Dossier Vehicle.RegistrationData ein neues Element namens BaseNumberN mit einer Länge von 12 Zeichen eingeführt. Das bisherige Element BaseNumber ist hiermit abgekündigt und wird voraussichtlich mit dem Release 2026-003 entfernt.
