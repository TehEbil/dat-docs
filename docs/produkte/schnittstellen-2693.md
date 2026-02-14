---
title: "Schnittstellenoperationen"
topic_id: "2693"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen"
---

# Schnittstellenoperationen

SilverDAT myClaim stellt Fremdsystemen verschiedene SOAP Webservices zur Verfügung.

Die WSDL kann unter der Adresse https://www.dat.de/myClaim/soap/v2/MyClaimExternalService?wsdl abgerufen werden.

Folgende Funktionen stehen dann zur Verfügung:

- [addMessage()](#showid/2581 "Hinzufügen einer Nachricht zu einem Auftrag")
- [assignPartnerByCustomerNumber()](#showid/2585 "Zuweisen eines Partners anhand der Kundennummer")
- [assignPartnerByInternalIdentification()](#showid/2587 "Zuweisen eines Partners anhand der internen Identifikation")
- [assignPartnerToContract()](#showid/2589 "Zuweisen eines Partners")
- [assignUsersToContract()](#showid/2702 "Zuweisen eines Benutzers")
- [assignInvoiceRateToContract()](#showid/2615 "Zuweisung eines Verrechnungssatzes zu einem Auftrag")
- [changeContractStatus()](#showid/2573 "Ändern eines Auftragsstatus")
- [copyClaim()](#showid/9346 "Kopieren eines Auftrags")
- [createOrUpdateContract()](#showid/16529 "Erstellen eines neuen Auftrags mit Option zum Aktualisieren/Überschreiben")
- [createOrUpdateContractN()](#showid/16529 "Erstellen eines neuen Auftrags mit Option zum Aktualisieren/Überschreiben")
- [findContract()](#showid/1473 "Finden eines Auftrags")
- [getContract()](#showid/1471 "Abrufen eines Auftrags")
- [getContractStatus()](#showid/2567 "Abrufen eines Auftragsstatus")
- getContactData()
- getPrintReport()
- [getGeoCoordinates](#showid/2611 "Abrufen der Geo Koordinaten einer angegeben Adresse")()
- [getCalculatedSpareParts](#showid/7494 "Abrufen von Ersatzteilen aus einer Kalkulation")()
- [getCalculatedSpareParts](#showid/7494 "Abrufen von Ersatzteilen aus einer Kalkulation")()
- [getPossibleContractStatusTransitions()](#showid/9174 "Auflisten von möglichen nachfolgenden Status zu einem Auftrag")
- [getPossibleNetworkStatuses()](#showid/9168 "Abrufen der Status zu einem Netzwerk")
- [getPossibleContactPersons()](#showid/9171 "Auflisten von Ansprechpartnern")
- [getAddressBook()](#showid/14240 "Abrufen eines Adressbuchs")
- [importCalculationSummaryByType()](#showid/7500 "Übergabe von strukturierten Rechnungs- oder Kalkulationsdaten ")
- [importCalculationSummaryByType()](#showid/7500 "Übergabe von strukturierten Rechnungs- oder Kalkulationsdaten ")
- [listAttachmentFolders()](#showid/2603 "Auflisten der Anhangsordner")
- [listAttachmentsOfContract](#showid/2591 "Auflisten der Anhänge")()
- [listContracts()](#showid/2593 "Auflisten der Aufträge")
- [listPartners()](#showid/2569 "Auflisten der Partner")
- [listTemplates()](#showid/2595 "Auflisten der Vorlagen")
- [listInvoiceRates](#showid/2613 "Auflisten der Verrechnungssätze")()
- [listAvailableNetworkTypes()](#showid/9283 "Auflisten der vorhandenen Netzwerktypen")
- [listAdressBook()](#showid/14237 "Auflisten der Adressbücher")
- [removeAddressBook()](#showid/14246 "Löschen eines Adressbuchs")
- [searchForPartners](#showid/2605 "Suchen nach Partnern")()
- [saveAddressBook()](#showid/14243 "Anlegen eines Adressbuchs")
- [uploadAttachmentByFolderID()](#showid/2577 "Hochladen von Anhängen anhand einer Ordner ID")
- [uploadAttachmentByIdentification()](#showid/2579 "Hochladen von Anhängen anhand einer Identifikation")
- [unassignPartnerFromContract()](#showid/2599 "Entfernen einer Partnerzuweisung aus einem Auftrag")
- [unassingUsersFromContract()](#showid/2601 "Entfernen einer Benutzerzuweisung aus einem Auftrag")
