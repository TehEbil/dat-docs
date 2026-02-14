---
title: "Exportieren von Dokumenten"
topic_id: "2338"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Exportieren von Dokumenten"
---

# Exportieren von Dokumenten

Mit der Schnittstellenfunktion exportDossierToDocument() können die Daten eines Kalkulationsergebnisses exportiert werden. Die Funktion bietet
eine Vielzahl von Exportmöglichkeiten, wie beispielsweise die Kalkulation mit Bildern,
die Kalkulation mit Protokoll, kombinierte Ausdrücke usw.

Derzeit wird der Export als PDF, DOCX, TXT und HTML unterstützt.

Bitte beachten Sie, dass das Druckprodukt (printProduct) "protocol" nur im Ausgabeformat "PDF" exportiert werden kann. Hingegen kann eine Kalkulation, Rechnung oder einen Kostenvoranschlag
als DOCX, PDF oder HTML-Datei ausgegeben werden.

Im Gegensatz zu den Formaten PDF und DOCX erhebt die TXT-Ausgabe keinen Anspruch auf inhaltliche Vollständigkeit. Als möglicher Anwendungsfall
steht hier die Informationsweitergabe des Schadenumfangs bspw. an Restwertbörsen im
Vordergrund. Für die Anwendung im Rahmen eines Kostenvoranschlags oder eines Gutachtens
sollte die TXT-Ausgabe nicht verwendet werden.

Die Vorgangsnummer dossierID ist identisch mit der DossierID aus der Funktion [importDossier](erstellen-aktu-1367.md)().

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| dossierID | Long, Pflicht |  | Die eindeutige Kennung eines Vorgangs. |
| locale | Locale |  | Ausgabesprache des Dokuments. |
| format | String | "PDF" | "DOCX" |" HTML" | "TXT" | Das Ausgabeformat, derzeit wird "PDF", "DOCX", "HTML" und "TXT" unterstützt. |
| product | String | "VRO\_CALC\_RESULT" |  "BLANKET\_CALC\_RESULT" | "common" |  "optimized" |  "glass" |  "italyCommon" |  "italyOptimized" |  "italyGlass" |  "customerRanking" | "commonSerialSUTC" |  "spo" | Art der Kalkulation. |
| printProduct | String | "calculation" |  "estimate" |  "invoice" |  "images" |  "protocol" |  "inspectionProtocol" |  "sumOfCosts" |  "partList" |  "addressList" |  "sparePartsList" |  "calculationInsurance" |  "invoiceInsurance" |  "calculationWithImages" |  "calculationWithProtocol" |  "summary"  "depreciationinformation"  "maintenanceSchedule"  "withoutInsuranceData"  "withoutOwnerData"  "withoutDriverData"  "withoutGarageData"  "withoutOpponentData"  "withoutEquipments"  "withoutRepairCostExpansion" | Art des Druckprodukts (Bild, Kalkulation, Kostenvoranschlag, Kostenvoranschlag inkl. Bilder, Protokoll oder Rechnung).  Der Parameter "printProduct" ermöglicht, kombinierte Ausdrucke mit einem einzigen Aufruf von exportDossierToDocument() erhalten zu können. Die Werte müssen durch Kommata getrennt werden. |
| layout | String | Ausdruckname z. B. KalkulationXY oder dessen ID | 1. Druckvorlage  Wenn dieser Parameter übersprungen wird, dann wird die DAT-Standard-Vorlage verwendet werden.    2. Bildvorlage  Bei dem Druckprodukt "images" stehen folgende Werte für "layout" zur Verfügung:  [large | middle | small] |
| damageSegmentNumber | Integer |  | Ermöglicht den Ausdruck eines bestimmten Schadenskalkulation. Bitte beachten Sie, dass das Attribut nur für das Datenland Österreich vorgesehen ist und die entsprechende Schadensnummer in der Kalkulation enthalten sein muss. |

Rückgabe

Als Antwort wird ein Dokument als String im Base64-Format zurückgegeben, ansonsten wird eine Fehlermeldung zurückgeliefert.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| exportDocument | String | Das generierte Dokument wird als Base64 kodierter String zurückgegeben.    Die Base64 Kodierung schützt das Dokument vor Fehlern durch Zeichensatzkonvertierungen. Wird der String weiterverarbeitet oder abgespeichert, so muss er immer zuerst dekodiert werden.    Die Base64 Dekodierung ist sehr einfach und entsprechende Funktionen in allen Programmiersprachen enthalten.    Ein Base64 Onlinekonverter hier verfügbar:  <https://base64.guru/converter> |
