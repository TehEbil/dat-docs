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

Das [Restriction Objekt](restriction-2419.md) definiert die zu überprüfenden Eigenschaften. Es wird nur auf das Vorhandensein einer
Eigenschaft, nicht das Fehlen geprüft.

Wenn keine Ergebnisse gefunden wurden, wird eine Fehlermeldung zurückgegeben.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| ExternalId | String, optional |  | Externe ID für die Identifizierung der zusammengehörigen Teilvorgänge |
| [restriction](restriction-2419.md) | [restriction](restriction-2419.md) |  | Filter, der die notwendigen Eigenschaften beschreibt. |
| [settings](settings-2421.md) | [settings](settings-2421.md) |  | Mit dem Attribut settings kann der Response wie gewünscht eingestellt werden.  (Mögliche Einstellungen: Sprache, Offset sowie Eingrenzung der Ergebnismenge) |
| [sortingCriterions](#expandblock-2417-d2e85353)  | Attribut | Bedeutung | Typ und Wertebereich | | --- | --- | --- | | [contractName](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [orderNumber](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [invoiceNumber](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [garageContractName](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | registrationNumber |  | [orderInfo](orderinfo-6718.md) | | [vin](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [datEcode](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [createDateFrom](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [createDateTo](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [changeDateFrom](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [changeDateTo](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [vehicleType](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [manufacturer](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [baseModel](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [subModel](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [insuranceClaim](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [sortingCriterions](#expandblock-2417-d2e85358)  | Attribut | Bedeutung | Typ und Wertebereich | | --- | --- | --- | | [contractName](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [orderNumber](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [invoiceNumber](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [garageContractName](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | registrationNumber |  | [orderInfo](orderinfo-6718.md) | | [vin](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [datEcode](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [createDateFrom](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [createDateTo](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [changeDateFrom](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [changeDateTo](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [vehicleType](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [manufacturer](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [baseModel](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [subModel](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | | [insuranceClaim](orderinfo-6718.md) |  | [orderInfo](orderinfo-6718.md) | |  | Anordnen von Elementen in einer durch ein bestimmtes Kriterium geordneten Reihenfolge (auf-, oder absteigend) |

Rückgabe

Alle Dossiers sowie die zugehörigen DatProcessInfos die die Eigenschaften der [Restrictions](restriction-2419.md) erfüllen.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| countOfContractslsFound | Integer | Gesamtzahl der gefundenen Ergebnisse |
| countOfContractssReturned | Integer | Zahl der tatsächlich zurückgegebenen Verträge. Die Anzahl der Suchergebnisse kann über den settings Parameter begrenzt und mit einem offset versehen werden. |
| [Dossiers](../../vxs/aktenzeichenvo-1369.md) | [Dossier](../../vxs/aktenzeichenvorgan/aktenzeichenvo-1371.md) | Ein Dossier Objekt, das eine Liste mit allen Ergebnissen enthält. |
| [dossiersDatProcessInfos](dossiersdatpro-2427.md) | [dossiersDatProcessInfos](dossiersdatpro-2427.md) |  |
