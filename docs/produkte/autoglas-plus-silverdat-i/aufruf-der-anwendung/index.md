---
title: "Aufruf der Anwendungsoberfläche über Schnittstelle"
topic_id: "2064"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Aufruf der Anwendungsoberfläche über Schnittstelle"
---

# Aufruf der Anwendungsoberfläche über Schnittstelle

Mit dem September Release 2025 entfallen die calculateGlass Schnittstellen, die unter https://www.dat.de/GlassRep/services?wsdl zu finden sind. Der Aufruf der SilverDAT calculateGlass Oberflächenschnittstelle wird
ebenfalls nicht mehr unterstützt. Bitte beachten Sie, dass die Applikation SilverDAT calculateGlass zukünftig durch SilverDAT 3 Glas (SilverDAT myClaim https://www.dat.de/myClaim/soap/v2/MyClaimExternalService?wsdl) ersetzt wird.

Die Datenübergabe einer Fremdapplikation an autoglas Plus kann auch durch einen HTTP-POST Request erfolgen. Vorgesehen ist eine Datenübergabe allerdings nur an die Auftragseröffnungsmaske:

Ablauf der Datenübergabe

Ziel ist es, über eine Fremdapplikation, z.B. ein Dealer-Management-System, die Auftragseröffnungsmaske
von autoglas Plus oder SilverDAT calculateGlass in einem Browser zu öffnen, damit die Daten, die Sie aus Ihrem System an autoglas Plus oder SilverDAT calculateGlass übergeben haben, weiterbearbeitet werden können. Sie übergeben die Daten im VXS-Format und die Daten werden automatisch in die Auftragseröffnungsmaske übertragen.

Das Bild oben zeigt, dass die Auftragseröffnungsmaske nur eines von mehreren aufeinanderfolgenden
Masken ist, die korrekt ausgefüllt werden müssen, damit eine Kalkulation erfolgen
kann. Damit Sie nach Eröffnung des Auftrags auf die Folgeseiten navigieren können,
müssen alle Pflichtfelder in der Oberfläche (sind mit einem \* gekennzeichnet) korrekt
ausgefüllt sein. Die Daten können Sie entweder über ein VXS übergeben oder Sie erfassen sie manuell, in der Auftragseröffnungsmaske, nach.

In jedem Fall muss mit dem VXS immer eine OrderNumber übergeben werden, da diese nicht in der Auftragseröffnung nacherfasst werden kann.
Fehlt sie in der VXS-Datei, führt dies zu einem Fehler.

Ein Beispiel, wie ein Skript aussehen könnte, das für den Upload der Daten genutzt
werden kann, finden Sie im Kapitel [Beispiel für den Daten-Upload via POST](beispiel-fur-d-2068.md). Das Beispiel zeigt die zwei Möglichkeiten des Daten-Uploads, jeweils dargestellt
über ein Formular. Der obere Upload lässt zu, dass eine VXS-Datei aus dem Dateisystem ausgewählt werden kann; die untere Upload-Möglichkeit sieht
ein Textfeld vor, indem die VXS-Datei in Klartext hineinkopiert werden kann.

Durch das Absenden nimmt dieses Formular Kontakt mit der jeweiligen Glas-Anwendung
auf und übertragt die Daten in die jeweiligen Datenfelder.

Ein Beispiel für eine entsprechende VXS-Datei finden Sie im Kapitel [Beispiel VXS-Datei Auftragseroeffnung](beispiel-vxs-d-2070.md). Informationen zum genutzten VXS-Schema finden Sie in der Dokumentation VXS-Struktur.

- [beispiel-fur-d-2068](beispiel-fur-d-2068.md)
- [beispiel-vxs-d-2070](beispiel-vxs-d-2070.md)
- [parameter-fur-2150](parameter-fur-2150.md)
- [parameter-fur-2152](parameter-fur-2152.md)
