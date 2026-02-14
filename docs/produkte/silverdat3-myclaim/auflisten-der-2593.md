---
title: "Auflisten der Aufträge"
topic_id: "2593"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Auflisten von Informationen innerhalb einer Kundennummer > Auflisten der Aufträge"
---

# Auflisten der Aufträge

Die Funktion listContracts listet alle Aufträge innerhalb einer Kundennummer auf. Das Ergebnis kann dann mit
den optionalen Filtern wie Netzwerktyp, Auftragstyp weiter eingeschränkt werden.

Hinweis

Für das Auflisten von Fahrzeuginstandsetzungskalkulationen verwenden Sie im Parameter
contractTypes den Wert vro\_calculation, für Bewertungen bundle\_valuation.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| statusesId | List<Long> |  | Status ID des Auftrags |  |
| contractTypes | List<String> | vro\_calculation  bundle\_valuation | Nur Auftäge dieses bestimmten Auftragstyps werden angezeigt. |  |
| networkTypes | List<String> | DAT, NISSAN... | Nur Aufträge dieses bestimmten Netzwerktyps werden aufgelistet. |  |
| partnersToRetrieve | List<String> | MANUFACTURER... | Liste der Rollen für gültige Partner |  |
| openedSince | Date |  | Nur Aufträge die ab diesem bestimmten Datum erstellt wurden werden aufgelistet. |  |
| changedSince | Date |  | Nur Aufträge die ab diesem bestimmten Datum geändert wurden werden aufgelistet. |  |
| folderType | claimFolderType | ALL\_CLAIMS  NEW\_ASSIGNED\_CLAIMS  MY\_CLAIMS  GROUP\_AND\_OWN  GROUP | ALL\_CLAIMS: Alle eigenen Aufträge und alle Vorgänge bei denen man als Partner zugewiesen wurde.    NEW\_ASSIGNED\_CLAIMS: Beauftragte Vorgänge    MY\_CLAIMS: Eigene Vorgänge      GROUP: Zeigt die Vorgänge an, die im Mandantenverbund geteilt wurden. Eigene Vorgänge werden nur aufgelistet, wenn sie auch anderen Mandantenverbunden zum Lesen freigegeben wurden    GROUP\_AND\_OWN: Zeigt die Vorgänge an, die im Mandantenverbund geteilt wurden, sowie die eigenen Vorgänge, auch wenn diese nicht für andere Mandantenverbunde freigegeben wurden. |  |
| folder | Long |  | Nur Aufträge dieses bestimmten Ordners werden aufgelistet. |  |
| pageLimit | int |  | Schränkt die Anzahl der aufgelisteten Aufträge ein.    Es wird empfohlen, das Limit von 1000 nicht zu überschreiten, da sonst eine Timeout-Exception aufgrund von Performance-Problemen ausgelöst werden kann. |  |
| pageOffset | int |  | Überspringt die übergebene Anzahl an Datensätzen bis der erste Auftrag angezeigt wird. |  |
| attributes | attributes |  | Attribute zum Filtern |  |

Parameter attributes

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| referenceNumber | String |  | Nur Aufträge mit einem bestimmten Vorgangsnamen. |  |
| templateIds | Long |  | Nur Aufträge mit einem bestimmten Template. |  |
| creatorNumber | String |  | Nur Aufträge, die von dieser Kundennummer erstellt wurden. |  |
| assignedTags | assignedTags |  | Filtern nach einem bestimmten Merkmal |  |
| vehicleInfo | vehicleInfo |  | Filtern nach Fahrzeugdaten |  |

Parameter assignedTags

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| designation | String |  | Benennung des Merkmals |  |
| identification | String |  | ID des Merkmals |  |
| tagType | String |  | Typ des Merkmals |  |

Parameter vehicleInfo

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| hsn | String |  | Identifikationsnummer |  |
| mileage | String |  | Kilometerangabe |  |
| manufacturer | String |  | Name des Herstellers |  |
| mainModel | String |  | Haupttyp des Fahrzeugs |  |
| subType | String |  | Untertyp des Fahrzeugs |  |
| plateNumber | String |  | Kennzeichen |  |
| tsn | String |  | Typschlüsselnummer |  |
| vin | String |  | Fahrgestellnummer |  |

Rückgabe

Liste der gefilterten Aufträge.
