---
title: "Request getDVNEquipments"
topic_id: "2417"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abruf von Ausstattungen zu DVN > Request getDVNEquipments"
---

# Request getDVNEquipments

##### Abfrage der Vorgangsübersicht

Die Funktion getContractList() durchsucht alle gespeicherten Vorgänge auf Eigenschaften und gibt alle übereinstimmenden
Vorgänge als Dossier zurück.

Da die Ergebnismenge sehr groß sein kann, werden maximal 100 Ergebnisse zurückgegeben.
Die Anzahl kann über das Settings-Objekt weiter eingeschränkt werden. Über die Offset Eigenschaft lässt sich durch die Ergebnisse blättern.

Das [Restriction Objekt](#showid/2419 "restriction") definiert die zu überprüfenden Eigenschaften. Es wird nur auf das Vorhandensein einer
Eigenschaft, nicht das Fehlen geprüft.

Wenn keine Ergebnisse gefunden wurden, wird eine Fehlermeldung zurückgegeben.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| ExternalId | String, optional |  | Externe ID für die Identifizierung der zusammengehörigen Teilvorgänge |
| [restriction](#showid/2419 "restriction") | [restriction](#showid/2419 "restriction") |  | Filter, der die notwendigen Eigenschaften beschreibt. |
| [settings](#showid/2421 "Settings") | [settings](#showid/2421 "Settings") |  | Mit dem Attribut settings kann der Response wie gewünscht eingestellt werden.  (Mögliche Einstellungen: Sprache, Offset sowie Eingrenzung der Ergebnismenge) |
| [sortingCriterions](#expandblock-2417-d2e85353)  | Attribut | Bedeutung | Typ und Wertebereich | | --- | --- | --- | | [contractName](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [orderNumber](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [invoiceNumber](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [garageContractName](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | registrationNumber |  | [orderInfo](#showid/6718 "OrderInfo") | | [vin](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [datEcode](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [createDateFrom](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [createDateTo](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [changeDateFrom](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [changeDateTo](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [vehicleType](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [manufacturer](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [baseModel](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [subModel](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [insuranceClaim](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [sortingCriterions](#expandblock-2417-d2e85358)  | Attribut | Bedeutung | Typ und Wertebereich | | --- | --- | --- | | [contractName](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [orderNumber](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [invoiceNumber](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [garageContractName](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | registrationNumber |  | [orderInfo](#showid/6718 "OrderInfo") | | [vin](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [datEcode](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [createDateFrom](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [createDateTo](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [changeDateFrom](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [changeDateTo](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [vehicleType](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [manufacturer](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [baseModel](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [subModel](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | | [insuranceClaim](#showid/6718 "OrderInfo") |  | [orderInfo](#showid/6718 "OrderInfo") | |  | Anordnen von Elementen in einer durch ein bestimmtes Kriterium geordneten Reihenfolge (auf-, oder absteigend) |

Rückgabe

Alle Dossiers sowie die zugehörigen DatProcessInfos die die Eigenschaften der [Restrictions](#showid/2419 "restriction") erfüllen.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| countOfContractslsFound | Integer | Gesamtzahl der gefundenen Ergebnisse |
| countOfContractssReturned | Integer | Zahl der tatsächlich zurückgegebenen Verträge. Die Anzahl der Suchergebnisse kann über den settings Parameter begrenzt und mit einem offset versehen werden. |
| [Dossiers](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)") | [Dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") | Ein Dossier Objekt, das eine Liste mit allen Ergebnissen enthält. |
| [dossiersDatProcessInfos](#showid/2427 "DossiersDatProcessInfos") | [dossiersDatProcessInfos](#showid/2427 "DossiersDatProcessInfos") |  |
