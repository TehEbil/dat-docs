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

Das [Restriction Objekt](../datentypen/restriction-2419.md) definiert die zu überprüfenden Eigenschaften. Es wird nur auf das Vorhandensein einer
Eigenschaft, nicht das Fehlen geprüft.

Wenn keine Ergebnisse gefunden wurden, wird eine Fehlermeldung zurückgegeben.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| ExternalId | String, optional |  | Externe ID für die Identifizierung der zusammengehörigen Teilvorgänge |
| [restriction](../datentypen/restriction-2419.md) | [restriction](../datentypen/restriction-2419.md) |  | Filter, der die notwendigen Eigenschaften beschreibt. |
| [settings](../datentypen/settings-2421.md) | [settings](../datentypen/settings-2421.md) |  | Mit dem Attribut settings kann der Response wie gewünscht eingestellt werden.  (Mögliche Einstellungen: Sprache, Offset sowie Eingrenzung der Ergebnismenge) |
| sortingCriterions  | Attribut | Bedeutung | Typ und Wertebereich | | --- | --- | --- | | [contractName](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [orderNumber](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [invoiceNumber](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [garageContractName](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | registrationNumber |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [vin](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [datEcode](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [createDateFrom](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [createDateTo](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [changeDateFrom](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [changeDateTo](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [vehicleType](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [manufacturer](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [baseModel](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [subModel](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [insuranceClaim](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | sortingCriterions  | Attribut | Bedeutung | Typ und Wertebereich | | --- | --- | --- | | [contractName](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [orderNumber](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [invoiceNumber](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [garageContractName](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | registrationNumber |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [vin](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [datEcode](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [createDateFrom](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [createDateTo](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [changeDateFrom](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [changeDateTo](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [vehicleType](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [manufacturer](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [baseModel](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [subModel](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | | [insuranceClaim](../datentypen/orderinfo-6718.md) |  | [orderInfo](../datentypen/orderinfo-6718.md) | |  | Anordnen von Elementen in einer durch ein bestimmtes Kriterium geordneten Reihenfolge (auf-, oder absteigend) |

Rückgabe

Alle Dossiers sowie die zugehörigen DatProcessInfos die die Eigenschaften der [Restrictions](../datentypen/restriction-2419.md) erfüllen.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| countOfContractslsFound | Integer | Gesamtzahl der gefundenen Ergebnisse |
| countOfContractssReturned | Integer | Zahl der tatsächlich zurückgegebenen Verträge. Die Anzahl der Suchergebnisse kann über den settings Parameter begrenzt und mit einem offset versehen werden. |
| [Dossiers](../../../vxs/aktenzeichenvorgange-doss/index.md) | [Dossier](../../../vxs/aktenzeichenvorgange-doss/aktenzeichenvorgang/index.md) | Ein Dossier Objekt, das eine Liste mit allen Ergebnissen enthält. |
| [dossiersDatProcessInfos](../datentypen/dossiersdatpro-2427.md) | [dossiersDatProcessInfos](../datentypen/dossiersdatpro-2427.md) |  |
