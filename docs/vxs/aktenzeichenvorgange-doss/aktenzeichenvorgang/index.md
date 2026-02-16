---
title: "Aktenzeichen/Vorgang (Dossier)"
topic_id: "1371"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Aktenzeichen/Vorgang (Dossier)"
---

# Aktenzeichen/Vorgang (Dossier)

Im <Dossiers>-Element können beliebig viele <Dossier>-Elemente enthalten sein, diese entsprechen den „Vorgängen" (SD3).
   Felder:
   
      
         
            
               
                  Element
               
               
                  Typ
               
               
                  Beschreibung
               
            
            
               
                  Name
               
               
                  String
               
               
                  Vorgangsname in SilverDAT valuateFinance
               
            
            
               
                  Description
               
               
                  String
               
               
                  Vorgangsname in SilverDAT calculatePro und SilverDAT calculateExpert
               
            
            
               
                  UUID
               
               
                  String
               
               
                  Weltweite ID des Dossiers
               
            
            
               
                  ExternalId
               
               
                  String
               
               
                  Identifikation im Fremdsystem
               
            
            
               
                  IdSD2
               
               
                  String12
               
               
                  Identifikation für SilverDAT II
               
            
            
               
                  IdSDo
               
               
                  Integer
               
               
                  Identifikation für SilverDAT online
               
            
            
               
                  IdSD3Local
               
               
                  Integer
               
               
                  Identifikation für SilverDAT 3 lokale Installation
               
            
            
               
                  DossierId
               
               
                  Integer
               
               
                  Identifikation für SilverDAT 3; (entspricht der contractID)
               
            
            
               
                  IdSD3Network
               
               
                  Integer
               
               
                  Zusätzliche Identifikation für SilverDAT 3 
               
            
            
               
                  IdExtern
               
               
                  String40
               
               
                  Identifikation im Fremdsystem
               
            
            
               
                  Country
               
               
                  String3
               
               
                  Landeskürzel für den Zielmarkt; ISO 3166 ALPHA-2, zum Beispiel: ES.
                  weitere Infos siehe Popup-Fenster
               
            
            
               
                  Language
               
               
                  String5
               
               
                  Sprachkennzeichen in ISO-Kodierung, zum Beispiel: DE_de
                  weitere Infos siehe Popup-Fenster
               
            
            
               
                  DataVersion
               
               
                  Decimal
               
               
                  Datenstand (Versionnummer Datenbestand von DAT)
               
            
            
               
                  Currency
               
               
                  String3
               
               
                  Währung
               
            
            
               
                  DatCustomerId
               
               
                  String10
               
               
                  Kundennummer bei der DAT
               
            
            
               
                  MerchandId
               
               
                  Decimal
               
               
                  Kundennummer einem Verband
               
            
            
               
                  DossierType
               
               
                  String
               
               
                  Nutzungskennzeichen / Auftragstyp, z.B. repair für das Produkt SilverDAT calculatePRO oder calculateExpert für SilverDAT calculateExpert
               
            
            
               
                  DossierOrigin
               
               
                  String
               
               
                  Ursprung Dossier
               
            
            
               
                  CreateDate
               
               
                  DateTime
               
               
                  Erstellungsdatum
               
            
            
               
                  CreateUser
               
               
                  String
               
               
                  Benutzer, der das Dossier erzeugt hat
               
            
            
               
                  ChangeDate
               
               
                  DateTime
               
               
                  Datum der letzten Änderung
               
            
            
               
                  ChangeUser
               
               
                  String
               
               
                  Benutzer der letzten Änderung
               
            
            
               
                  CDYear
               
               
                  Integer
               
               
                  Datenbestand Jahr
               
            
            
               
                  CDMonth
               
               
                  Integer
               
               
                  Datenbestand Monat
               
            
            
               
                  ProcedureType
               
               
                  String
               
               
                  Art des Vorgangs in SilverDAT 3 PRO, z.B. NEW_VEHICLE für ein Neufahrzeug
               
            
            
               
                  DatCustomerAddress
               
               
                  address
               
               
                  Adressdaten (Address)
                  weitere Infos siehe Popup-Fenster
               
            
            
               
                  Vehicle
               
               
                  Vehicle
               
               
                  Fahrzeugdaten
               
            
            
               
                  Images
               
               
                  Images
               
               
                  Bilder (obsolet)
               
            
            
               
                  ImageList
               
               
                  ImageList
               
               
                  Bilder
               
            
            
               
                  VAT
               
               
                  VAT
               
               
                  Informationen zur Umsatzsteuer
               
            
            
               
                  Management
               
               
                  anyType
               
               
                  Datenorganisation für Einkauf und Verkauf sowie Inventarisierung
               
            
            
               
                  TradingData
               
               
                  TradingData
               
               
                  Handelsdaten, Partneraddressen sowie Vorbesitzer
               
            
            
               
                  Labelling
               
               
                  Labelling
               
               
                  Auszeichnungsdaten
               
            
            
               
                  ContractData
               
               
                  ContractData
               
               
                  Vertragsdaten
               
            
            
               
                  Valuation
               
               
                  Valuation
               
               
                  Bewertungsdaten für Gebrauchtfahrzeuge
               
            
            
               
                  Compare
               
               
                  Compare
               
               
                  Gebrauchtfahrzeugvergleichsdaten
               
            
            
               
                  RepairCalculation
               
               
                  RepairCalculation
               
               
                  Reparaturkalkulation
               
            
            
               
                  RepairOrder
               
               
                  RepairOrder
               
               
                  Reparaturauftrag der Versicherung, enthält Versicherungs- und Freigabenummern sowie
                     Informationen zum Datum, Selbstbehalt und ähnlichem.
               
            
            
               
                  SparePartPositions
               
               
                  SparePartPositions
               
               
                  Ersatzteile Position
               
            
            
               
                  MaintenanceIntervals
               
               
                  MaintenanceIntervals
               
               
                  Wartungsintervalle
               
            
            
               
                  Comments
               
               
                  Comments
               
               
                  Kommentare
               
            
            
               
                  Attachments
               
               
                  Attachments
               
               
                  Anhang
               
            
            
               
                  AdditionalVehicles
               
               
                  AdditionalVehicles
               
               
                  Weitere Fahrzeugdaten
               
            
            
               
                  ChangeUserId
               
               
                  Integer
               
               
                  ID der Person, die ändert 
               
            
            
               
                  CreateUserId
               
               
                  Integer
               
               
                  ID des Person, die erstellt
               
            
            
               
                  WearCalculation
               
               
                  Boolean
               
               
                  Kalkulation Verschleiss
               
            
            
               
                  InsuranceClaim
               
               
                  Boolean
               
               
                  Versicherung
               
            
            
               
                  AdditionalServices
               
               
                  AdditionalServices
               
               
                  Zusätzliche Dienstleistungen zur  Kalkulation
               
            
            
               
                  ProcessManagement
               
               
                  ProcessManagement
               
               
                  Informationen über Schadensmanagement, Rechnungen und weitere Informationen von der
                     Versicherung
               
            
            
               
                  TradingActivity
                  
                     
                        Das Element <TradingActivity> enthält die Informationen zu den Handelstätigkeiten. Es befindet sich direkt unter
                           dem Dossier Element. Die zugehörigen Kindelemente enthalten die Details zu den jeweiligen
                           Handelstätigkeiten.
                        Zum Setzen der Daten lesen Sie bitte das Kapitel "Status umbuchen".
                        
                           
                              
                                 
                                    
                                       Element 
                                    
                                    
                                       Typ
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Schreibweise
                                    
                                 
                                 
                                    
                                       State
                                    
                                    
                                       String
                                    
                                    
                                       Aktueller Status des DossiersErfasstDispositionBestandVerkauft
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       Purchase
                                       
                                          
                                             Das Element <Purchase> ist ein Unterelement von <TradingActivity> und enthält die Details zum Ankauf eines Fahrzeugs.
                                             Zum Setzen der Daten rufen Sie die Methode setPurchaseData auf. Bitte lesen Sie den entsprechenden Kapitel "Status umbuchen" durch.
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            BuyerId
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            ID des Käufers
                                                         
                                                         
                                                            numerisch
                                                         
                                                      
                                                      
                                                         
                                                            VehicleGroup
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Fahrzeuggruppe
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            DeregistrationDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Abmeldedatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyType
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Restgarantieart
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyUntil
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Restgarantie bis
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PaymentAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Zahlungsvereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            OtherAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Sonstige Vereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PurchaseDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Ankaufsdatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            PurchasePriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Einkaufspreis (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PurchasePriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Einkaufspreis (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            MileageExpected
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Voraussichtliche Laufleistung (km)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ProvisionOn
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Bereitstellung am
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            AcceptanceDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            geplantes Hereinnahmedatum
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            AcceptanceDetails
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Hereinnahmedetails
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       Purchase
                                       
                                          
                                             Das Element <Purchase> ist ein Unterelement von <TradingActivity> und enthält die Details zum Ankauf eines Fahrzeugs.
                                             Zum Setzen der Daten rufen Sie die Methode setPurchaseData auf. Bitte lesen Sie den entsprechenden Kapitel "Status umbuchen" durch.
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            BuyerId
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            ID des Käufers
                                                         
                                                         
                                                            numerisch
                                                         
                                                      
                                                      
                                                         
                                                            VehicleGroup
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Fahrzeuggruppe
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            DeregistrationDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Abmeldedatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyType
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Restgarantieart
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyUntil
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Restgarantie bis
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PaymentAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Zahlungsvereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            OtherAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Sonstige Vereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PurchaseDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Ankaufsdatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            PurchasePriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Einkaufspreis (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PurchasePriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Einkaufspreis (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            MileageExpected
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Voraussichtliche Laufleistung (km)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ProvisionOn
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Bereitstellung am
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            AcceptanceDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            geplantes Hereinnahmedatum
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            AcceptanceDetails
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Hereinnahmedetails
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       Ankauf
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       PlanData
                                    
                                    
                                       PlanData
                                    
                                    
                                       Plandaten
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       PriceCalculation
                                       
                                          
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Verkaufspreis (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Verkaufspreis (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PurchasePriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Einkaufspreis (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PurchasePriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Einkaufspreis (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            VehicleNewPriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Listenneupreis einschließlich SA (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            VehicleNewPriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Listenneupreis einschließlich SA (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            LabelPriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Auszeichnung (EUR) Netto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            LabelPriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Auszeichnung (EUR) Brutto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceMinimumNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Mindest-Verkaufspreis Netto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceMinimumGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Mindest-Verkaufspreis Brutto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResellerSalesPriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Wiederverkäuferpreis Netto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResellerSalesPriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Wiederverkäuferpreis Brutto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            (DAT)NominalDaysOnLot
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Standtage [d]
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ActualRepairCosts
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Aktuelle Instandsetzungskosten 
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            DifferenceRepairCosts
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Differenz Instandsetzungskosten
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       PriceCalculation
                                       
                                          
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Verkaufspreis (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Verkaufspreis (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PurchasePriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Einkaufspreis (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PurchasePriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Einkaufspreis (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            VehicleNewPriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Listenneupreis einschließlich SA (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            VehicleNewPriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Listenneupreis einschließlich SA (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            LabelPriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Auszeichnung (EUR) Netto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            LabelPriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Auszeichnung (EUR) Brutto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceMinimumNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Mindest-Verkaufspreis Netto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceMinimumGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Mindest-Verkaufspreis Brutto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResellerSalesPriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Wiederverkäuferpreis Netto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResellerSalesPriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Wiederverkäuferpreis Brutto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            (DAT)NominalDaysOnLot
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Standtage [d]
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ActualRepairCosts
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Aktuelle Instandsetzungskosten 
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            DifferenceRepairCosts
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Differenz Instandsetzungskosten
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       Preiskalkulation
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       Admission
                                       
                                          
                                             Das Element <Admission> ist ein Unterelement von <TradingActivity> und enthält die Details zum Zugang eines Fahrzeugs.
                                             Zum Setzen der Daten rufen Sie die Methode setAdmissionData auf. Bitte lesen Sie den entsprechenden Kapitel "Status umbuchen" durch.
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            AdmissionDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Ankaufsdatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            AdmissionPriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Ankaufspreis (EUR) Netto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            AdmissionPriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Ankaufspreis (EUR) Brutto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            AcceptanceDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Hereinnahmedatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            AcceptanceDetails
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Hereinnahmedetails
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            MileageVehicle
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Fahrzeug Laufleistung (km)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            MileageOdometer
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Laufleistung entsprechend der Tachoanzeige bei der Hereinnahme des Fahrzeugs (km)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            Location
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Standort des Fahrzeugs
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            DeregistrationDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Abmeldedatum
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyType
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Restgarantieart
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyUntil
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Restgarantie bis
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert Netto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert Brutto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PaymentAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Zahlungsvereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            OtherAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Sonstige Vereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ProvisionOn
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Bereitstellung am
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            BuyerId
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Id des Einkäufers
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            VehicleGroup
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Fahrzeuggruppe
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       Admission
                                       
                                          
                                             Das Element <Admission> ist ein Unterelement von <TradingActivity> und enthält die Details zum Zugang eines Fahrzeugs.
                                             Zum Setzen der Daten rufen Sie die Methode setAdmissionData auf. Bitte lesen Sie den entsprechenden Kapitel "Status umbuchen" durch.
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            AdmissionDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Ankaufsdatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            AdmissionPriceNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Ankaufspreis (EUR) Netto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            AdmissionPriceGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Ankaufspreis (EUR) Brutto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            AcceptanceDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Hereinnahmedatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            AcceptanceDetails
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Hereinnahmedetails
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            MileageVehicle
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Fahrzeug Laufleistung (km)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            MileageOdometer
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Laufleistung entsprechend der Tachoanzeige bei der Hereinnahme des Fahrzeugs (km)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            Location
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Standort des Fahrzeugs
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            DeregistrationDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Abmeldedatum
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyType
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Restgarantieart
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyUntil
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Restgarantie bis
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert Netto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert Brutto
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PaymentAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Zahlungsvereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            OtherAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Sonstige Vereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ProvisionOn
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Bereitstellung am
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            BuyerId
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Id des Einkäufers
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            VehicleGroup
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Fahrzeuggruppe
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       Zugang
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       Sale
                                       
                                          
                                             Das Element <Sale> ist ein Unterelement von <TradingActivity> und enthält die Details zum Verkauf eines Fahrzeugs.
                                             Zum Setzen der Daten rufen Sie setSalesData auf. Bitte lesen Sie das entsprechende Kapitel "Status umbuchen" durch.
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            OrderDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Auftragsdatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            SellerId
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Eindeutige ID des Verkäufers (Ansprechpartner)
                                                         
                                                         
                                                            numerisch
                                                         
                                                      
                                                      
                                                         
                                                            BusinessType
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Geschäftsart
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            VehicleGroup
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Fahrzeuggruppe
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceNet
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Verkaufspreis (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceGross
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Verkaufspreis (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            DeliveryDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Auslieferungsdatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            MileageVehicle
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Fahrzeug Laufleistung 
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            MileageOdometer
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Laufleistung entsprechend der Tachoanzeige (km)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            RegistrationNumber
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Amtliches Kennzeichen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesDetails
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Verkaufsangaben
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            LicenseNumberPurchase
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Amtliches Kennzeichen zum Zeitpunkt des Ankaufs
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PaymentAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Zahlungsvereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            OtherAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Sonstige Vereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            RenewEmissionVehicleInspectionCheck
                                                         
                                                         
                                                            Boolean
                                                         
                                                         
                                                            Hauptuntersuchung wird durch den Wert true zum Pflichtfeld
                                                         
                                                         
                                                            true, false
                                                         
                                                      
                                                      
                                                         
                                                            AcceptanceDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Annahmedatum
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyType
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Restgarantieart
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyUntil
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Restgarantie bis
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            Provider
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Garantieanbieter
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            RepaymentTerm
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Rückzahlungsdauer (Monate)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            StartDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Beginn der Garantie
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            EndDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Ende der Garantie
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            WarrantyNumber
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Garantienummer
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            WarrantyAmountNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Garantiebetrag (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            WarrantyAmountGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Garantiebetrag (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            NextVehicleInspectionDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Nächste Hauptuntersuchung
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            NextEmissionsTestDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Nächste Abgasuntersuchung
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            Labelling
                                                         
                                                         
                                                            Labelling
                                                         
                                                         
                                                            Auszeichnung
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            AgreementOnDeviationsCheck
                                                         
                                                         
                                                            Boolean
                                                         
                                                         
                                                            Vereinbarung über Abweichungen
                                                         
                                                         
                                                            true, false
                                                         
                                                      
                                                      
                                                         
                                                            ShorteningLimitationPeriodCheck
                                                         
                                                         
                                                            Boolean
                                                         
                                                         
                                                            Verkürzung der Verjährungsfrist
                                                         
                                                         
                                                            true, false
                                                         
                                                      
                                                      
                                                         
                                                            ExclusionOfObligationToUpdateCheck
                                                         
                                                         
                                                            Boolean
                                                         
                                                         
                                                            Ausschluss der Aktualisierungspflicht
                                                         
                                                         
                                                            true, false
                                                         
                                                      
                                                      
                                                         
                                                            UpdateInformationCheck
                                                         
                                                         
                                                            Boolean
                                                         
                                                         
                                                            Information zur Aktualisierung
                                                         
                                                         
                                                            true, false
                                                         
                                                      
                                                      
                                                         
                                                            InfoReqUpdatesAndInstallation
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Angaben zu den erforderlichen Aktualisierungen und deren Installation
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            AgreementOnDeviationsList
                                                         
                                                         
                                                            
                                                         
                                                         
                                                            Vereinbarung über Abweichungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            WarrantyType
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Garantietyp
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            WarrantyPeriod
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Garantiezeitraum
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                             Element AgreementOnDeviationsList
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            AgreementPosition
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Position in der Liste
                                                         
                                                         
                                                            numerisch
                                                         
                                                      
                                                      
                                                         
                                                            Feature
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Merkmal der Abweichung
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            State
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Tatsächliche Beschaffenheit
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       Sale
                                       
                                          
                                             Das Element <Sale> ist ein Unterelement von <TradingActivity> und enthält die Details zum Verkauf eines Fahrzeugs.
                                             Zum Setzen der Daten rufen Sie setSalesData auf. Bitte lesen Sie das entsprechende Kapitel "Status umbuchen" durch.
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            OrderDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Auftragsdatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            SellerId
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Eindeutige ID des Verkäufers (Ansprechpartner)
                                                         
                                                         
                                                            numerisch
                                                         
                                                      
                                                      
                                                         
                                                            BusinessType
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Geschäftsart
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            VehicleGroup
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Fahrzeuggruppe
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceNet
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Verkaufspreis (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesPriceGross
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Verkaufspreis (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            DeliveryDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Auslieferungsdatum
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            MileageVehicle
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Fahrzeug Laufleistung 
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            MileageOdometer
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Laufleistung entsprechend der Tachoanzeige (km)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            RegistrationNumber
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Amtliches Kennzeichen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            SalesDetails
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Verkaufsangaben
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            LicenseNumberPurchase
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Amtliches Kennzeichen zum Zeitpunkt des Ankaufs
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            PaymentAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Zahlungsvereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            OtherAgreements
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Sonstige Vereinbarungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            RenewEmissionVehicleInspectionCheck
                                                         
                                                         
                                                            Boolean
                                                         
                                                         
                                                            Hauptuntersuchung wird durch den Wert true zum Pflichtfeld
                                                         
                                                         
                                                            true, false
                                                         
                                                      
                                                      
                                                         
                                                            AcceptanceDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Annahmedatum
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyType
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Restgarantieart
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyUntil
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Restgarantie bis
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            ResidualWarrantyValueGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Restgarantiewert (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            Provider
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Garantieanbieter
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            RepaymentTerm
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Rückzahlungsdauer (Monate)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            StartDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Beginn der Garantie
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            EndDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Ende der Garantie
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            WarrantyNumber
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Garantienummer
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            WarrantyAmountNet
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Garantiebetrag (Netto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            WarrantyAmountGross
                                                         
                                                         
                                                            Decimal
                                                         
                                                         
                                                            Garantiebetrag (Brutto)
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            NextVehicleInspectionDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Nächste Hauptuntersuchung
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            NextEmissionsTestDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Nächste Abgasuntersuchung
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            Labelling
                                                         
                                                         
                                                            Labelling
                                                         
                                                         
                                                            Auszeichnung
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            AgreementOnDeviationsCheck
                                                         
                                                         
                                                            Boolean
                                                         
                                                         
                                                            Vereinbarung über Abweichungen
                                                         
                                                         
                                                            true, false
                                                         
                                                      
                                                      
                                                         
                                                            ShorteningLimitationPeriodCheck
                                                         
                                                         
                                                            Boolean
                                                         
                                                         
                                                            Verkürzung der Verjährungsfrist
                                                         
                                                         
                                                            true, false
                                                         
                                                      
                                                      
                                                         
                                                            ExclusionOfObligationToUpdateCheck
                                                         
                                                         
                                                            Boolean
                                                         
                                                         
                                                            Ausschluss der Aktualisierungspflicht
                                                         
                                                         
                                                            true, false
                                                         
                                                      
                                                      
                                                         
                                                            UpdateInformationCheck
                                                         
                                                         
                                                            Boolean
                                                         
                                                         
                                                            Information zur Aktualisierung
                                                         
                                                         
                                                            true, false
                                                         
                                                      
                                                      
                                                         
                                                            InfoReqUpdatesAndInstallation
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Angaben zu den erforderlichen Aktualisierungen und deren Installation
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            AgreementOnDeviationsList
                                                         
                                                         
                                                            
                                                         
                                                         
                                                            Vereinbarung über Abweichungen
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            WarrantyType
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Garantietyp
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            WarrantyPeriod
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Garantiezeitraum
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                             Element AgreementOnDeviationsList
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            AgreementPosition
                                                         
                                                         
                                                            Integer
                                                         
                                                         
                                                            Position in der Liste
                                                         
                                                         
                                                            numerisch
                                                         
                                                      
                                                      
                                                         
                                                            Feature
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Merkmal der Abweichung
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            State
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Tatsächliche Beschaffenheit
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       Verkauf
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       SalesPreparation
                                       
                                          
                                             Das Element <Reservierungsdetails> ist ein Unterelement von <TradingActivity> und enthält die Details zur Reservierung eines Fahrzeugs.
                                             
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            StartReservationDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Reservierungsdatum (Start)
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            EndReservationDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Reservierungsdatum (Ende)
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            ReservedFor
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Informationen, für welchen Ansprechpartner die Reservierung vorgenommen wurde.
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            CarriedOutBy
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Informationen, von wem die Reservierung vorgenommen wurde.
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            Comment
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Bemerkung zur Reservierung.
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       SalesPreparation
                                       
                                          
                                             Element vxs:SalesPreparation
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            MarketplaceImageList
                                                         
                                                         
                                                            MarketplaceImageList
                                                         
                                                         
                                                            Börsenbilder
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       Verkaufsvorbereitung
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ReservationData
                                       
                                          
                                             Das Element <Reservierungsdetails> ist ein Unterelement von <TradingActivity> und enthält die Details zur Reservierung eines Fahrzeugs.
                                             
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            StartReservationDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Reservierungsdatum (Start)
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            EndReservationDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Reservierungsdatum (Ende)
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            ReservedFor
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Informationen, für welchen Ansprechpartner die Reservierung vorgenommen wurde.
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            CarriedOutBy
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Informationen, von wem die Reservierung vorgenommen wurde.
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            Comment
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Bemerkung zur Reservierung.
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       ReservationData
                                       
                                          
                                             Das Element <Reservierungsdetails> ist ein Unterelement von <TradingActivity> und enthält die Details zur Reservierung eines Fahrzeugs.
                                             
                                             
                                                
                                                   
                                                      
                                                         
                                                            Name
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                      
                                                      
                                                         
                                                            StartReservationDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Reservierungsdatum (Start)
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            EndReservationDate
                                                         
                                                         
                                                            Date
                                                         
                                                         
                                                            Reservierungsdatum (Ende)
                                                         
                                                         
                                                            Format [YYYY-MM-DD]
                                                         
                                                      
                                                      
                                                         
                                                            ReservedFor
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Informationen, für welchen Ansprechpartner die Reservierung vorgenommen wurde.
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            CarriedOutBy
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Informationen, von wem die Reservierung vorgenommen wurde.
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            Comment
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Bemerkung zur Reservierung.
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       Reservierungsdetails
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                     
                  
               
               
                  TradingActivity
               
               
                  Handelsaktivität für den Prozessablauf des Autohauses
               
            
            
               
                  TradingAdditional
                  
                     
                        Das Element <TradingAdditional> enthält die Informationen zu den weiteren Handelstätigkeiten. Es befindet sich direkt
                           unter dem Dossier Element. Die zugehörigen Kindelemente enthalten die Details zu den
                           jeweiligen weiteren Handelstätigkeiten.
                        
                           
                              
                                 
                                    
                                       Name
                                    
                                    
                                       Datentyp
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Schreibweise
                                    
                                 
                                 
                                    
                                       MarketplacePreparation
                                    
                                    
                                       MarketplacePreparation
                                    
                                    
                                       Börsenaufbereitung
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       PurchaseOfferList
                                    
                                    
                                       PurchaseOffer
                                    
                                    
                                       Ankaufsangebote
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       SalesOfferList
                                    
                                    
                                       SalesOffer
                                    
                                    
                                       Verkaufsangebote
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                     
                  
               
               
                  TradingAdditional
               
               
                  Weitere Daten für den  Prozessablauf des Autohauses
               
            
            
               
                  MetaPositions
               
               
                  MetaPositions
               
               
                  Dossier-Metapositionen 
               
            
            
               
                  overwrite
               
               
                  Boolean
               
               
                  Vorhandenes/-n Aktenzeichen/Vorgang überschreiben?
               
            
         
      
   
   
   Beispiel einer Dossierstruktur:
   
   Dossier
    DatCustomerAddress
    Vehicle
        RegistrationData
        Engine
        TechInfo
            FillingQuantities
        Equipment
            DenialCaseEquipment
   
           Tires
    VAT
    TradingData
        Owner
        Opponent
        ClientContactAddresses
    RepairCalculation
        Vehicle
            RegistrationData
            Engine
            TechInfo
                FillingQuantities
            Equipment
        RepairWages
        RepairParameters
   
           ProcedureRelatedParameters
        RepairPositions
   
           CalcResultToUse
        CalcResultCommon
            MaterialPositions
            LabourPositions
            LacquerPositions
            RepairCalculationSummary
   
           DiscountPositions
        CalculationSummary
   
       RepairOrder
   
       Attachments
   
       WearCalculation
   
       InsuranceClaim
   
       ProcessManagement

- [adressdaten-ad-1375](adressdaten-ad-1375.md)
