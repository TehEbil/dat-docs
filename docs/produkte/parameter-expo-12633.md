---
title: "Parameter exportDossierN (SilverDAT 3 valuateExpert)"
topic_id: "12633"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Exportieren von Dokumenten (SilverDAT 3 valuateExpert, valuateExpertPlusPartner) > Parameter exportDossierN (SilverDAT 3 valuateExpert)"
---

# Parameter exportDossierN (SilverDAT 3 valuateExpert)

Sachverständige können mithilfe der Funktion exportDossierN einen Ausdruck gemäß DAT oder gemäß Sachverständiger erstellen. Zusätzlich können Sachverständige
      noch eine Urkundennummer erzeugen. Es existieren Anhänge und Gutachten, diese werden
      über das Attribute productName ausgewählt. 
   
      
         Der Ausdruck gemäß DAT oder Sachverständiger wird durch das Attribut value gesteuert.
      
      
         Die Generierung der Urkundennummer wird über den Parameter ExportCertificateAddOns gesteuert.
      
   
   Übersicht der möglichen Ausdrucke productName
   
      
         
            
               
                  Wert
               
               
                  Produkt Beschreibung
               
               
                  Format 
               
               
                  In folgenden Produkten enthalten
               
               
                  Link
               
            
            
               
                  UsedVehicleEvaluationForValuateExpert
               
               
                  Gebrauchtwagen
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpert/valuateExpertPlusPartner
               
               
                  Gebrauchtwagenbewertung
                  
                     
                        Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
                        Gebrauchtwagenbewertungsausdruck
                        Parameter vxs:ExportProduct mit folgenden Attributen
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Pflicht
                                    
                                 
                                 
                                    
                                       productName
                                    
                                    
                                       UsedVehicleEvaluationForValuateExpert
                                    
                                    
                                       Gebrauchtwagenbewertung
                                    
                                    
                                       X
                                    
                                 
                              
                           
                        
                        Parameter vxs:ExportProductAddOns mit folgenden Attributen
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Bedingung
                                    
                                 
                                 
                                    
                                       product
                                    
                                    
                                       VALUATION
                                    
                                    
                                       Wertermittlung
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       valueIndication
                                       
                                    
                                    
                                       ValuesDealerProcurementPrice
                                    
                                    
                                       Einkaufspreis
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ValuesDealerSalesPrice
                                    
                                    
                                       Verkaufspreis
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ValuesDealerProcurementPriceAndDealerSalesPrice
                                    
                                    
                                       Einkaufspreis und Verkaufspreis
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ReplacementValue
                                    
                                    
                                       Wiederbeschaffungswert
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ActualCashValue
                                    
                                    
                                       Zeitwert
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ValueAccordingToMarket
                                    
                                    
                                       Marktwert
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       tax
                                       
                                    
                                    
                                       DIFFERENCE
                                    
                                    
                                       Differenzbesteuert (inkl. Anteil MwSt)
                                    
                                    
                                       Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                                    
                                 
                                 
                                    
                                       DIFFERENCE_TAX_AVG_VAT
                                    
                                    
                                       Differenzbesteuert (durchschnittlicher Anteil MwSt.)
                                    
                                    
                                       Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                                    
                                 
                                 
                                    
                                       PRIVATE
                                    
                                    
                                       Privatmarkt (MwSt neutral)
                                    
                                    
                                       Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist. 
                                    
                                 
                                 
                                    
                                       RULE
                                    
                                    
                                       Besteuerungsart: Regelbesteuerung
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       value
                                       
                                    
                                    
                                       DAT
                                    
                                    
                                       gemäß DAT
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       EXPERT
                                    
                                    
                                       gemäß Festlegung der Sachverständiger
                                    
                                    
                                       Geben Sie mit setValueDefinition den Sachverständiger Wert an.
                                    
                                 
                                 
                                    
                                       printOption
                                       
                                    
                                    
                                       PREVIEW
                                    
                                    
                                       Vorschau (kostenloser Ausdruck)
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ACTUALPRINT
                                    
                                    
                                       Kostenpflichtiger Echtdruck
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                        Request exportDossierN Gebrauchtwagenbewertung 
                        
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>123456789</DossierId>
         <Locale country="DE" datCountryIndicator="DE" language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="UsedVehicleEvaluationForValuateExpert"/>
         <!--Optional:-->
         <ExportProductAddOns printOption="ACTUALPRINT" product="VALUATION" tax="DIFFERENCE" value="DAT" valueIndication="ReplacementValue"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

                     
                  
               
            
            
               
                  ProtocolForExpert
               
               
                  Protokoll
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpert/valuateExpertPlusPartner
               
               
                  Protokoll
                  
                     
                        Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
                        Parameter vxs:ExportProduct mit folgenden Attributen
                        
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Vorbedingung
                                    
                                 
                                 
                                    
                                       productName
                                    
                                    
                                       ProtocolForExpert 
                                    
                                    
                                       Protokoll
                                    
                                    
                                       X
                                    
                                 
                              
                           
                        
                        Parameter vxs:ExportProductAddOns mit folgenden Attributen
                        
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Vorbedingung
                                    
                                 
                                 
                                    
                                       product
                                    
                                    
                                       VALUATION,
                                       BASECHECK,
                                       LEASING_RETURN,
                                       CONDITION_REPORT,
                                       ESTIMATION_CERTIFICATE
                                       VALUATION_EXPERTISE
                                    
                                    
                                       für alle Produkte verfügbar. Auswahl des Produkts.
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       withEquipmentReport
                                    
                                    
                                       true, false
                                    
                                    
                                       Ausstattungsbericht
                                    
                                    
                                       Ausstattungen müssen in der Ausstattungsmaske oder mit createDossier gesetzt werden.
                                    
                                 
                                 
                                    
                                       withValueDecrease
                                    
                                    
                                       true, false
                                    
                                    
                                       Wertminderung
                                    
                                    
                                       Die Daten müssen auf der Zustandsmaske oder mit setConditionDetails gesetzt werden
                                    
                                 
                                 
                                    
                                       withValueIncrease
                                    
                                    
                                       true, false
                                    
                                    
                                       Werterhöhung
                                    
                                    
                                       Die Daten müssen auf der Zustandsmaske oder mit setConditionDetails gesetzt werden
                                    
                                 
                                 
                                    
                                       withRepairCosts
                                    
                                    
                                       true, false
                                    
                                    
                                       Reparaturkosten
                                    
                                    
                                       Die Daten müssen auf der Zustandsmaske oder mit setConditionDetails gesetzt werden
                                    
                                 
                                 
                                    
                                       withValueIncreaseDetails
                                    
                                    
                                       true, false
                                    
                                    
                                       Werterhöhungsdetails
                                    
                                    
                                       Das Attribut withValueIncrease muss auf true gesetzt sein
                                    
                                 
                                 
                                    
                                       withRepairCostsDetails
                                    
                                    
                                       true, false
                                    
                                    
                                       Reparaturkostendetails
                                    
                                    
                                       Das Attribut withRepairCosts muss auf true gesetzt sein
                                    
                                 
                                 
                                    
                                       withTruckBodies
                                    
                                    
                                       true, false
                                    
                                    
                                       LKW- Aufbauten
                                    
                                 
                                 
                                    
                                       value
                                       
                                    
                                    
                                       DAT
                                    
                                    
                                       gemäß DAT
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       EXPERT
                                    
                                    
                                       gemäß Festlegung der Sachverständiger
                                    
                                    
                                       Geben Sie mit setValueDefinition den Sachverständiger Wert an.
                                    
                                 
                                 
                                    
                                       printOption
                                       
                                    
                                    
                                       PREVIEW
                                    
                                    
                                       Vorschau (kostenloser Ausdruck), Probedruck
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ACTUALPRINT
                                    
                                    
                                       Kostenpflichtiger Echtdruck
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                        Request exportDossierN Protokoll
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct productName="ProtocolForExpert " />
         <ExportProductAddOns printOption="ACTUALPRINT" />
         <ExportCertificateAddOns ePrint="true" />
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

                        
                     
                  
               
            
            
               
                  OptionalEquipmentChecklist
               
               
                  Checkliste Sonderausstattungen
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpert/valuateExpertPlusPartner
               
               
                  Checkliste Sonderausstattungen
                  
                     
                        Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
                        Parameter vxs:ExportProduct mit folgenden Attributen
                        
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Vorbedingung
                                    
                                 
                                 
                                    
                                       productName
                                    
                                    
                                       OptionalEquipmentChecklist
                                    
                                    
                                       Checkliste Sonderausstattungen
                                    
                                    
                                       X
                                    
                                 
                              
                           
                        
                        Parameter vxs:ExportProductAddOns mit folgenden Attributen
                        
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Vorbedingung
                                    
                                 
                                 
                                    
                                       product
                                    
                                    
                                       VALUATION,
                                       BASECHECK,
                                       LEASING_RETURN,
                                       CONDITION_REPORT,
                                       ESTIMATION_CERTIFICATE
                                       VALUATION_EXPERTISE
                                    
                                    
                                       für alle Produkte verfügbar. Auswahl des Produkts.
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       printOption
                                       
                                    
                                    
                                       PREVIEW
                                    
                                    
                                       Vorschau (kostenloser Ausdruck), Probedruck
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ACTUALPRINT
                                    
                                    
                                       Kostenpflichtiger Echtdruck
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                        Request exportDossierN Checkliste Sonderausstattungen
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale country="DE" datCountryIndicator="de" language="de_DE"/>
         <Format>pdf</Format>
         <ExportProduct productName="OptionalEquipmentChecklist"/>
         <ExportProductAddOns printOption="ACTUALPRINT" product="VALUATION"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

                        
                     
                  
               
            
            
               
                  VehicleData
               
               
                  Fahrzeugdaten
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpert/valuateExpertPlusPartner
               
               
                  
               
            
            
               
                  BaseCheckReportNew
               
               
                  Urkunde der Grundüberprüfung 
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  Grundüberprüfung
                  
                     
                        Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
                        Grundüberprüfungsausdruck
                        Bitte beachten Sie beim Erstellen der Ausdrucke für die Grundüberprüfung, dass immer
                           zuerst die neue Urkunde productName="BaseCheckReportNew" ausgedruckt wird. 
                        Alle eventuell benötigten weiteren Seiten müssen mittels eines zweiten Aufrufs der
                           Funktion exportDossierN erzeugt werden, wobei hier die Option productName="BaseCheckReport" zu verwenden ist. 
                        Parameter vxs:ExportProduct mit folgenden Attributen
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Pflicht
                                    
                                 
                                 
                                    
                                       productName
                                       
                                    
                                    
                                       BaseCheckReportNew
                                    
                                    
                                       Urkunde der Grundüberprüfung
                                    
                                    
                                       X
                                       
                                    
                                 
                                 
                                    
                                       BaseCheckReport
                                    
                                    
                                       Anhang der Grundüberprüfung
                                    
                                 
                              
                           
                        
                        Parameter vxs:ExportProductAddOns mit folgenden Attributen
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Bedingung
                                    
                                 
                                 
                                    
                                       product
                                    
                                    
                                       BASECHECK
                                    
                                    
                                       Grundüberprüfung
                                    
                                    
                                       Geben Sie mit setProductCheckDetailsList die Grundüberprüfungsinformation an.
                                    
                                 
                                 
                                    
                                       layout
                                       
                                    
                                    
                                       ListLayoutWithoutPictures
                                    
                                    
                                       Layout ohne Bilder
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ListLayoutWithPictures
                                    
                                    
                                       Layout mit Bildern
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ExtendedLayout
                                    
                                    
                                       Erweitertes Layout
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       SpecialLayout
                                    
                                    
                                       Speziallayout
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       valueIndication
                                       
                                    
                                    
                                       WithoutValue
                                    
                                    
                                       Keine Presiangaben
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ValuesDealerProcurementPrice
                                    
                                    
                                       Einkaufspreis
                                    
                                    
                                       Geben Sie mit setBaseCheckValueDefinition den Sachverständiger Wert an und setzen Sie den Attribut value auf EXPERT.
                                    
                                 
                                 
                                    
                                       ValuesDealerSalesPrice
                                    
                                    
                                       Verkaufspreis
                                    
                                    
                                       Geben Sie mit setBaseCheckValueDefinition den Sachverständiger Wert an und setzen Sie den Attribut value auf EXPERT.
                                    
                                 
                                 
                                    
                                       ValuesDealerProcurementPriceAndDealerSalesPrice
                                    
                                    
                                       Einkaufspreis und Verkaufspreis
                                    
                                    
                                       Geben Sie mit setBaseCheckValueDefinition den Sachverständiger Wert an und setzen Sie den Attribut value auf EXPERT.
                                    
                                 
                                 
                                    
                                       value
                                       
                                    
                                    
                                       DAT
                                    
                                    
                                       gemäß DAT
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       EXPERT
                                    
                                    
                                       gemäß Festlegung der Sachverständiger
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       printOption
                                       
                                    
                                    
                                       PREVIEW
                                    
                                    
                                       Vorschau (kostenloser Ausdruck)
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ACTUALPRINT
                                    
                                    
                                       Kostenpflichtiger Echtdruck
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       withConditionComments
                                       
                                    
                                    
                                       1 (true)
                                    
                                    
                                       Ausdruck mit Anhang Fahrzeugzustandsbemerkungen
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       0 (false)
                                    
                                    
                                       Ausdruck ohne Anhang Fahrzeugzustandsbemerkungen
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                        Request exportDossierN zum Erzeugen der Urkunde 
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="BaseCheckReportNew"/>
         <!—Beispiel: layout="Listenlayout ohne Bilder" und ohne Wertangabe, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="WithoutValue" printOption="PREVIEW" product="BASECHECK"/>
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
                        
                        
                        Request exportDossierN zum Erzeugen der weiteren Seiten 
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="BaseCheckReport" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und ohne Wertangabe, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="WithoutValue" printOption="PREVIEW" product="BASECHECK" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

                     
                  
               
            
            
               
                  BaseCheckReport
               
               
                  Anhang der Grundüberprüfung
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  Anhang der Grundüberprüfung
               
            
            
               
                  LeasingReturnReportNew
               
               
                  Urkunde der Leasingrückgabe
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  Leasingrückgabe
                  
                     
                        Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
                        Leasingrückgabeausdruck
                        Bitte beachten Sie beim Erstellen der Ausdrucke für die Leasingrückgabe, dass immer
                           zuerst die neue Urkunde productName="LeasingReturnReportNew" ausgedruckt wird. 
                        Alle eventuell benötigten weiteren Seiten müssen mittels eines zweiten Aufrufs der
                           Funktion exportDossierN erzeugt werden, wobei hier die Option productName=LeasingReturnReport" zu verwenden ist. 
                        Parameter vxs:ExportProduct mit folgenden Attributen
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Pflicht
                                    
                                 
                                 
                                    
                                       productName
                                       
                                    
                                    
                                       LeasingReturnReportNew
                                    
                                    
                                       Urkunde der Leasingrückgabe
                                    
                                    
                                       X
                                       
                                    
                                 
                                 
                                    
                                       LeasingReturnReport
                                    
                                    
                                       Anhang der Leasingrückgabe
                                    
                                 
                              
                           
                        
                        Parameter vxs:ExportProductAddOns mit folgenden Attributen
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Bedingung
                                    
                                 
                                 
                                    
                                       product
                                    
                                    
                                       LEASING_RETURN
                                    
                                    
                                       Leasingrückgabe
                                    
                                    
                                       Geben Sie mit setProductCheckDetailsList die Leasingrückgabeinformation an
                                    
                                 
                                 
                                    
                                       layout
                                       
                                    
                                    
                                       ListLayoutWithoutPictures
                                    
                                    
                                       Layout ohne Bilder
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ListLayoutWithPictures
                                    
                                    
                                       Layout mit Bilder
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ExtendedLayout
                                    
                                    
                                       Erweitertes Layout
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       SpecialLayout
                                    
                                    
                                       Speziallayout
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       valueIndication
                                       
                                    
                                    
                                       WithoutValue
                                    
                                    
                                       Ohne Verkaufs oder Einkaufspreis
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ValuesDealerProcurementPrice
                                    
                                    
                                       Einkaufspreis
                                    
                                    
                                       Geben Sie mit setLeasingReturnValueDefinition den Sachverständiger Wert an und setzen Sie das Attribut value auf EXPERT.
                                    
                                 
                                 
                                    
                                       ValuesDealerSalesPrice
                                    
                                    
                                       Verkaufspreis
                                    
                                    
                                       Geben Sie mit setLeasingReturnValueDefinition den Sachverständiger Wert an und setzen Sie das Attribut value auf EXPERT.
                                    
                                 
                                 
                                    
                                       ValuesDealerProcurementPriceAndDealerSalesPrice
                                    
                                    
                                       Einkaufspreis und Verkaufspreis
                                    
                                    
                                       Geben Sie mit setLeasingReturnValueDefinition den Sachverständiger Wert an und setzen Sie das Attribut value auf EXPERT.
                                    
                                 
                                 
                                    
                                       value
                                       
                                    
                                    
                                       DAT
                                    
                                    
                                       gemäß DAT
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       EXPERT
                                    
                                    
                                       gemäß Festlegung der Sachverständiger
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       printOption
                                       
                                    
                                    
                                       PREVIEW
                                    
                                    
                                       Vorschau (kostenloser Ausdruck)
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ACTUALPRINT
                                    
                                    
                                       Kostenpflichtiger Echtdruck
                                    
                                    
                                       
                                       
                                    
                                 
                                 
                                    
                                       withConditionComments
                                       
                                    
                                    
                                       1 (true)
                                    
                                    
                                       Ausdruck mit Anhang Fahrzeugzustandsbemerkungen
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       0 (false)
                                    
                                    
                                       Ausdruck ohne Anhang Fahrzeugzustandsbemerkungen
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                        Request exportDossierN zum Erzeugen der Urkunde
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="LeasingReturnReportNew" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und ohne Wertangabe, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="WithoutValue" printOption="PREVIEW" product="LEASING_RETURN" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

                        Request exportDossierN zum Erzeugen der weiteren Seiten
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="LeasingReturnReport" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und ohne Wertangabe, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="WithoutValue" printOption="PREVIEW" product="LEASING_RETURN" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

                     
                  
               
            
            
               
                  LeasingReturnReport
               
               
                  Anhang der Leasingrückgabe
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  Anhang der Leasingrückgabe
               
            
            
               
                  ConditionReportNew
               
               
                  Urkunde des Zustandsberichts
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  Zustandsbericht
                  
                     
                        Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
                        Zustandsberichtausdruck
                        Bitte beachten Sie beim Erstellen der Ausdrucke für den Zustandsbericht, dass immer
                           zuerst die neue Urkunde productName="ConditionReportNew" ausgedruckt wird. 
                        Alle eventuell benötigten weiteren Seiten müssen mittels eines zweiten Aufrufs der
                           Funktion exportDossierN erzeugt werden, wobei hier die Option productName="ConditionReport" zu verwenden ist. 
                        Parameter vxs:ExportProduct mit folgenden Attributen
                        
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Bedingung
                                    
                                 
                                 
                                    
                                       productName
                                       
                                    
                                    
                                       ConditionReportNew
                                    
                                    
                                       Urkunde des Zustandsberichts
                                    
                                    
                                       X
                                       
                                    
                                 
                                 
                                    
                                       ConditionReport
                                    
                                    
                                       Anhang des Zustandsberichts
                                    
                                 
                              
                           
                        
                        Parameter vxs:ExportProductAddOns mit folgenden Attributen
                        
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Bedingung
                                    
                                 
                                 
                                    
                                       product
                                    
                                    
                                       CONDITION_REPORT
                                    
                                    
                                       Zustandsbericht
                                    
                                    
                                       Geben Sie mit setConditionDetails die Zustandsdetails an.
                                    
                                 
                                 
                                    
                                       layout
                                       
                                    
                                    
                                       ListLayoutWithoutPictures
                                    
                                    
                                       Layout ohne Bilder
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ListLayoutWithPictures
                                    
                                    
                                       Layout mit Bilder
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       value
                                       
                                    
                                    
                                       DAT
                                    
                                    
                                       gemäß DAT
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       EXPERT
                                    
                                    
                                       gemäß Festlegung der Sachverständiger
                                    
                                    
                                       Geben Sie mit setConditionReportValueDefinition den Sachverständiger Wert an.
                                    
                                 
                                 
                                    
                                       printOption
                                       
                                    
                                    
                                       PREVIEW
                                    
                                    
                                       Vorschau (kostenloser Ausdruck)
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ACTUALPRINT
                                    
                                    
                                       Kostenpflichtiger Echtdruck
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       withConditionComments
                                       
                                    
                                    
                                       1 (true)
                                    
                                    
                                       Ausdruck mit Anhang Fahrzeugzustandsbemerkungen
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       0 (false)
                                    
                                    
                                       Ausdruck ohne Anhang Fahrzeugzustandsbemerkungen
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                        Request exportDossierN zum Erzeugen der Urkunde
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="ConditionReportNew" />
         <!—Beispiel: layout="Listenlayout ohne Bilder", Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" printOption="PREVIEW" product="CONDITION_REPORT"/>
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
                        Request exportDossierN zum Erzeugen der weiteren Seiten 
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="ConditionReport" />
         <!—Beispiel: layout="Listenlayout ohne Bilder", Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" printOption="PREVIEW" product="CONDITION_REPORT"/>
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
                     
                  
               
            
            
               
                  ConditionReport
               
               
                  Anhang des Zustandsberichts
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  Anhang des Zustandsberichts
               
            
            
               
                  EstimationCertificateNew
               
               
                  Urkunde der Schätzurkunde
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  Bewertungsgutachten
                  
                     
                        Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
                        Bewertungsgutachtenausdruck
                        Bitte beachten Sie beim Erstellen der Ausdrucke für das Bewertungsgutachten, dass
                           immer zuerst die neue Urkunde productName="ValuationExpertiseNew" ausgedruckt wird. 
                        Alle eventuell benötigten weiteren Seiten müssen mittels eines zweiten Aufrufs der
                           Funktion exportDossierN erzeugt werden, wobei hier die Option productName="ValuationExpertise" zu verwenden ist. 
                        Parameter vxs:ExportProduct mit folgenden Attributen
                        
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Pflicht
                                    
                                 
                                 
                                    
                                       productName
                                       
                                    
                                    
                                       ValuationExpertiseNew
                                    
                                    
                                       Urkunde des Bewertungsgutachtens
                                    
                                    
                                       X
                                       
                                    
                                 
                                 
                                    
                                       ValuationExpertise
                                    
                                    
                                       Anhang des Bewertungsgutachtens 
                                    
                                 
                              
                           
                        
                        Parameter vxs:ExportProductAddOns mit folgenden Attributen
                        
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Bedingung
                                    
                                 
                                 
                                    
                                       product
                                    
                                    
                                       VALUATION_EXPERTISE
                                    
                                    
                                       Bewertungsgutachten
                                    
                                    
                                       Geben Sie mit setValuationExpertiseSpecialAssesmentsDetails die Bewertungsgutachteninformationen an.
                                    
                                 
                                 
                                    
                                       valueIndication
                                       
                                    
                                    
                                       ValuesDealerProcurementPrice
                                    
                                    
                                       Einkaufspreis
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ValuesDealerSalesPrice
                                    
                                    
                                       Verkaufspreis
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ValuesDealerProcurementPriceAndDealerSalesPrice
                                    
                                    
                                       Einkaufspreis und Verkaufspreis
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ReplacementValue
                                    
                                    
                                       Wiederbeschaffungswert
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ActualCashValue
                                    
                                    
                                       Zeitwert
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ValueAccordingToMarket
                                    
                                    
                                       Marktwert
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       tax
                                       
                                    
                                    
                                       DIFFERENCE
                                    
                                    
                                       Differenzbesteuert (inkl. Anteil MwSt)
                                    
                                    
                                       Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                                    
                                 
                                 
                                    
                                       DIFFERENCE_TAX_AVG_VAT
                                    
                                    
                                       Differenzbesteuert (durchschnittlicher Anteil MwSt.)
                                    
                                    
                                       Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                                    
                                 
                                 
                                    
                                       PRIVATE
                                    
                                    
                                       Privatmarkt (MwSt neutral)
                                    
                                    
                                       Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist. 
                                    
                                 
                                 
                                    
                                       RULE
                                    
                                    
                                       Besteuerungsart: Regelbesteuerung
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       value
                                       
                                    
                                    
                                       DAT
                                    
                                    
                                       gemäß DAT
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       EXPERT
                                    
                                    
                                       gemäß Festlegung der Sachverständiger
                                    
                                    
                                       Geben Sie mit setValuationExpertiseValueDefinition den Sachverständiger Wert an.
                                    
                                 
                                 
                                    
                                       printOption
                                       
                                    
                                    
                                       PREVIEW
                                    
                                    
                                       Vorschau (kostenloser Ausdruck)
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ACTUALPRINT
                                    
                                    
                                       Kostenpflichtiger Echtdruck
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       withConditionComments
                                       
                                    
                                    
                                       1 (true)
                                    
                                    
                                       Ausdruck mit Anhang Fahrzeugzustandsbemerkungen
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       0 (false)
                                    
                                    
                                       Ausdruck ohne Anhang Fahrzeugzustandsbemerkungen
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                        Request exportDossierN zum Erzeugen der Urkunde 
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="ValuationExpertiseNew" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und Wiederbeschaffungswert, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="ReplacementValue" printOption="PREVIEW" product="VALUATION_EXPERTISE" value="DAT" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
                        Request exportDossierN zum Erzeugen der weiteren Seiten 
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="ValuationExpertise" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und Wiederbeschaffungswert, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="ReplacementValue" printOption="PREVIEW" product="VALUATION_EXPERTISE" value="DAT" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
                     
                  
               
            
            
               
                  EstimationCertificate 
               
               
                  Anhand der Schätzurkunde
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  Anhand der Schätzurkunde
               
            
            
               
                  ValuationExpertiseNew
               
               
                  Urkunde des Bewertungsgutachtens
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  Schätzurkunde
                  
                     
                        Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
                        Schätzurkundeausdruck
                        Bitte beachten Sie beim Erstellen der Ausdrucke für die Schätzurkunde, dass immer
                           zuerst die neue Urkunde productName="EstimationCertificateNew" ausgedruckt wird. 
                        Alle eventuell benötigten weiteren Seiten müssen mittels eines zweiten Aufrufs der
                           Funktion exportDossierN erzeugt werden, wobei hier die Option productName="EstimationCertificate" zu verwenden ist. 
                        Parameter vxs:ExportProduct mit folgenden Attributen
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Bedingung
                                    
                                 
                                 
                                    
                                       productName
                                       
                                    
                                    
                                       EstimationCertificateNew
                                    
                                    
                                       Urkunde der Schätzurkunde
                                    
                                    
                                       X
                                       
                                    
                                 
                                 
                                    
                                       EstimationCertificate
                                    
                                    
                                       Anhang der Schätzurkunde
                                    
                                 
                              
                           
                        
                        Parameter vxs:ExportProductAddOns mit folgenden Attributen
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Bedingung
                                    
                                 
                                 
                                    
                                       product
                                    
                                    
                                       ESTIMATION_CERTIFICATE
                                    
                                    
                                       Schätzurkunde
                                    
                                    
                                       Geben Sie mit setEstimationCertificateSpecialAssesmentsDetails die Schätzurkundeinformationen an
                                    
                                 
                                 
                                    
                                       valueIndication
                                       
                                    
                                    
                                       ValuesDealerProcurementPrice
                                    
                                    
                                       Einkaufspreis
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ValuesDealerSalesPrice
                                    
                                    
                                       Verkaufspreis
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ValuesDealerProcurementPriceAndDealerSalesPrice
                                    
                                    
                                       Einkaufspreis und Verkaufspreis
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ValuesDealerProcurementPrice
                                    
                                    
                                       Wiederbeschaffungswert
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ValuesDealerSalesPrice
                                    
                                    
                                       Zeitwert
                                    
                                    
                                       Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                                    
                                 
                                 
                                    
                                       ValueAccordingToMarket
                                    
                                    
                                       Marktwert
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       tax
                                       
                                    
                                    
                                       DIFFERENCE
                                    
                                    
                                       Differenzbesteuert (inkl. Anteil MwSt)
                                    
                                    
                                       Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                                    
                                 
                                 
                                    
                                       DIFFERENCE_TAX_AVG_VAT
                                    
                                    
                                       Differenzbesteuert (durchschnittlicher Anteil MwSt.)
                                    
                                    
                                       Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                                    
                                 
                                 
                                    
                                       PRIVATE
                                    
                                    
                                       Privatmarkt (MwSt neutral)
                                    
                                    
                                       Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist. 
                                    
                                 
                                 
                                    
                                       RULE
                                    
                                    
                                       Besteuerungsart: Regelbesteuerung
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       value
                                       
                                    
                                    
                                       DAT
                                    
                                    
                                       gemäß DAT
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       EXPERT
                                    
                                    
                                       gemäß Festlegung der Sachverständiger
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       printOption
                                       
                                    
                                    
                                       PREVIEW
                                    
                                    
                                       Vorschau (kostenloser Ausdruck)
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ACTUALPRINT
                                    
                                    
                                       Kostenpflichtiger Echtdruck
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       withConditionComments
                                       
                                    
                                    
                                       1 (true)
                                    
                                    
                                       Ausdruck mit Anhang Fahrzeugzustandsbemerkungen
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       0 (false)
                                    
                                    
                                       Ausdruck ohne Anhang Fahrzeugzustandsbemerkungen
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                        Request exportDossierN zum Erzeugen der Urkunde 
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="EstimationCertificateNew" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und Wiederbeschaffungswert, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="ReplacementValue" printOption="PREVIEW" product="ESTIMATION_CERTIFICATE" value="DAT" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
                        Request exportDossierN zum Erzeugen der weiteren Seiten
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="EstimationCertificate" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und Wiederbeschaffungswert, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="ReplacementValue" printOption="PREVIEW" product="ESTIMATION_CERTIFICATE" value="DAT" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
                     
                  
               
            
            
               
                  ValuationExpertise
               
               
                  Anhang des Bewertungsgutachtens
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  Anhang des Bewertungsgutachtens
               
            
            
               
                  bafaGutachtenReport
               
               
                  BAFA Gutachten
               
               
                  PDF
               
               
                  SilverDAT 3 valuateExpertPlusPartner
               
               
                  BAFA Gutachten
                  
                     
                        Mit Hilfe der Funktion exportDossierN erstellen Sie das Gutachten zur Förderung für gebrauchte Fahrzeuge entsprechend den
                           Vorgaben des Bundesamt für Wirtschaft und Ausfuhrkontrolle (BAFA). 
                        Übersicht
                        
                           
                              
                                 
                                    
                                       Wert
                                    
                                    
                                       Produkt Beschreibung
                                    
                                    
                                       Format 
                                    
                                    
                                       In folgenden Produkten enthalten
                                    
                                 
                                 
                                    
                                       bafaGutachtenReport
                                    
                                    
                                       BAFA Gutachten
                                    
                                    
                                       PDF
                                    
                                    
                                       SilverDAT 3 valuateExpertPlusPartner
                                    
                                 
                              
                           
                        
                        
                        Überblick der Parameter und deren Attribute
                        
                           
                              
                                 
                                    
                                       Parameter
                                    
                                    
                                       Datentyp
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Schreibweise
                                    
                                    
                                       Pflicht
                                    
                                 
                                 
                                    
                                       DossierId
                                    
                                    
                                       Long
                                    
                                    
                                       EindeutigeVorgangskennung
                                    
                                    
                                       numerisch
                                    
                                    
                                       X
                                    
                                 
                                 
                                    
                                       Locale
                                    
                                    
                                       Locale
                                    
                                    
                                       Beispiel: <Locale country="DE"datCountryIndicator="DE" language="de"/>
                                    
                                    
                                       ISO 3166 ALPHA-2:
                                       country¹,datCountryIndicator¹
                                    
                                    
                                       X
                                    
                                 
                                 
                                    
                                       Format
                                    
                                    
                                       String
                                    
                                    
                                       Ausgabe-Dateiformat.Aktuell nur PDF möglich.
                                    
                                    
                                       PDF
                                    
                                    
                                       X
                                    
                                 
                                 
                                    
                                       ExportProduct
                                    
                                    
                                       String
                                    
                                    
                                       productName (Pflicht)
                                    
                                    
                                       bafaGutachtenReport
                                    
                                    
                                       X
                                    
                                 
                                 
                                    
                                       ExportProductAddOns
                                    
                                    
                                       String
                                    
                                    
                                       printOption
                                    
                                    
                                       ACTUALPRINT=Kostenpflichtiger EchtdruckPREVIEW=Vorschau (kostenloser Ausdruck), Probedruck
                                    
                                    
                                       
                                    
                                 
                                 
                                    
                                       ExportCertificateAddOns
                                    
                                    
                                       String
                                    
                                    
                                       ePrint
                                       Mit dieser Option aktivieren Sie den Druck mit Hintergrund. Dies benötigen Sie, falls
                                          die entsprechende Vorlage (Druckerpapier) für die Urkunde nicht verfügbar ist und
                                          auf normalen Papier gedruckt werden soll.
                                    
                                    
                                       true=Mit Hintergrundfalse=Blanko für Vordruck
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                        Request exportDossierN BAFA
                        
                        <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct productName="bafaGutachtenReport" />
         <ExportProductAddOns printOption="ACTUALPRINT" />
         <ExportCertificateAddOns ePrint="true" />
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

                        
                     
                  
               
            
         
      
   
   
   Überblick der Parameter und deren Attribute
   Request exportDossierN
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  DossierId
               
               
                  Integer
               
               
                  EindeutigeVorgangskennung
               
               
                  numerisch
               
               
                  X
               
            
            
               
                  Locale
               
               
                  Locale
               
               
                  Beispiel: <Locale country="DE"datCountryIndicator="DE" language="de"/>
               
               
                  ISO 3166 ALPHA-2:
                  country¹,datCountryIndicator¹
                  
                     
                        
                           
                              
                                 
                                    
                                       Country
                                    
                                    
                                       Land
                                    
                                    
                                       ISO 3166 ALPHA-2
                                    
                                    
                                       ISO 3166 ALPHA-3
                                    
                                    
                                       DAT-Kodierung
                                    
                                 
                                 
                                    
                                       Afghanistan
                                    
                                    
                                       Afghanistan
                                    
                                    
                                       AF
                                    
                                    
                                       AFG
                                    
                                    
                                       AFG
                                    
                                 
                                 
                                    
                                       Aland Islands
                                    
                                    
                                       Åland
                                    
                                    
                                       AX
                                    
                                    
                                       ALA
                                    
                                    
                                       AX
                                    
                                 
                                 
                                    
                                       Albania
                                    
                                    
                                       Albanien
                                    
                                    
                                       AL
                                    
                                    
                                       ALB
                                    
                                    
                                       AL
                                    
                                 
                                 
                                    
                                       Algeria
                                    
                                    
                                       Algerien
                                    
                                    
                                       DZ
                                    
                                    
                                       DZA
                                    
                                    
                                       DZ
                                    
                                 
                                 
                                    
                                       American Samoa
                                    
                                    
                                       Amerikanisch-Samoa
                                    
                                    
                                       AS
                                    
                                    
                                       ASM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Andorra
                                    
                                    
                                       Andorra
                                    
                                    
                                       AD
                                    
                                    
                                       AND
                                    
                                    
                                       AND
                                    
                                 
                                 
                                    
                                       Angola
                                    
                                    
                                       Angola
                                    
                                    
                                       AO
                                    
                                    
                                       AGO
                                    
                                    
                                       ANG
                                    
                                 
                                 
                                    
                                       Anguilla
                                    
                                    
                                       Anguilla
                                    
                                    
                                       AI
                                    
                                    
                                       AIA
                                    
                                    
                                       AXA
                                    
                                 
                                 
                                    
                                       Antarctica
                                    
                                    
                                       Antarktika
                                    
                                    
                                       AQ
                                    
                                    
                                       ATA
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Antigua and Barbuda
                                    
                                    
                                       Antigua und Barbuda
                                    
                                    
                                       AG
                                    
                                    
                                       ATG
                                    
                                    
                                       AG
                                    
                                 
                                 
                                    
                                       Argentina
                                    
                                    
                                       Argentinien
                                    
                                    
                                       AR
                                    
                                    
                                       ARG
                                    
                                    
                                       RA
                                    
                                 
                                 
                                    
                                       Armenia
                                    
                                    
                                       Armenien
                                    
                                    
                                       AM
                                    
                                    
                                       ARM
                                    
                                    
                                       ARM
                                    
                                 
                                 
                                    
                                       Aruba
                                    
                                    
                                       Aruba
                                    
                                    
                                       AW
                                    
                                    
                                       ABW
                                    
                                    
                                       ARU
                                    
                                 
                                 
                                    
                                       Australia
                                    
                                    
                                       Australien
                                    
                                    
                                       AU
                                    
                                    
                                       AUS
                                    
                                    
                                       AUS
                                    
                                 
                                 
                                    
                                       Austria
                                    
                                    
                                       Österreich
                                    
                                    
                                       AT
                                    
                                    
                                       AUT
                                    
                                    
                                       A
                                    
                                 
                                 
                                    
                                       Azerbaijan
                                    
                                    
                                       Aserbaidschan
                                    
                                    
                                       AZ
                                    
                                    
                                       AZE
                                    
                                    
                                       AZ
                                    
                                 
                                 
                                    
                                       Bahamas
                                    
                                    
                                       Bahamas
                                    
                                    
                                       BS
                                    
                                    
                                       BHS
                                    
                                    
                                       BS
                                    
                                 
                                 
                                    
                                       Bahrain
                                    
                                    
                                       Bahrain
                                    
                                    
                                       BH
                                    
                                    
                                       BHR
                                    
                                    
                                       BRN
                                    
                                 
                                 
                                    
                                       Bangladesh
                                    
                                    
                                       Bangladesch
                                    
                                    
                                       BD
                                    
                                    
                                       BGD
                                    
                                    
                                       BD
                                    
                                 
                                 
                                    
                                       Barbados
                                    
                                    
                                       Barbados
                                    
                                    
                                       BB
                                    
                                    
                                       BRB
                                    
                                    
                                       BDS
                                    
                                 
                                 
                                    
                                       Belarus
                                    
                                    
                                       Belarus (Weißrussland)
                                    
                                    
                                       BY
                                    
                                    
                                       BLR
                                    
                                    
                                       BY
                                    
                                 
                                 
                                    
                                       Belgium
                                    
                                    
                                       Belgien
                                    
                                    
                                       BE
                                    
                                    
                                       BEL
                                    
                                    
                                       B
                                    
                                 
                                 
                                    
                                       Belize
                                    
                                    
                                       Belize
                                    
                                    
                                       BZ
                                    
                                    
                                       BLZ
                                    
                                    
                                       BZ
                                    
                                 
                                 
                                    
                                       Benin
                                    
                                    
                                       Benin
                                    
                                    
                                       BJ
                                    
                                    
                                       BEN
                                    
                                    
                                       BJ
                                    
                                 
                                 
                                    
                                       Bermuda
                                    
                                    
                                       Bermuda
                                    
                                    
                                       BM
                                    
                                    
                                       BMU
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Bhutan
                                    
                                    
                                       Bhutan
                                    
                                    
                                       BT
                                    
                                    
                                       BTN
                                    
                                    
                                       BHT
                                    
                                 
                                 
                                    
                                       Bolivia
                                    
                                    
                                       Bolivien
                                    
                                    
                                       BO
                                    
                                    
                                       BOL
                                    
                                    
                                       BOL
                                    
                                 
                                 
                                    
                                       Bosnia and Herzegovina
                                    
                                    
                                       Bosnien und Herzegowina
                                    
                                    
                                       BA
                                    
                                    
                                       BIH
                                    
                                    
                                       BIH
                                    
                                 
                                 
                                    
                                       Botswana
                                    
                                    
                                       Botswana
                                    
                                    
                                       BW
                                    
                                    
                                       BWA
                                    
                                    
                                       RB
                                    
                                 
                                 
                                    
                                       Bouvet Island
                                    
                                    
                                       Bouvetinsel
                                    
                                    
                                       BV
                                    
                                    
                                       BVT
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Brazil
                                    
                                    
                                       Brasilien
                                    
                                    
                                       BR
                                    
                                    
                                       BRA
                                    
                                    
                                       BR
                                    
                                 
                                 
                                    
                                       British Indian Ocean Territory
                                    
                                    
                                       Britisches Territorium im Indischen Ozean
                                    
                                    
                                       IO
                                    
                                    
                                       IOT
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       British Virgin Islands
                                    
                                    
                                       Britische Jungferninseln
                                    
                                    
                                       VG
                                    
                                    
                                       VGB
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Brunei Darussalam
                                    
                                    
                                       Brunei Darussalam
                                    
                                    
                                       BN
                                    
                                    
                                       BRN
                                    
                                    
                                       BRU
                                    
                                 
                                 
                                    
                                       Bulgaria
                                    
                                    
                                       Bulgarien
                                    
                                    
                                       BG
                                    
                                    
                                       BGR
                                    
                                    
                                       BG
                                    
                                 
                                 
                                    
                                       Burkina Faso
                                    
                                    
                                       Burkina Faso
                                    
                                    
                                       BF
                                    
                                    
                                       BFA
                                    
                                    
                                       BF
                                    
                                 
                                 
                                    
                                       Burundi
                                    
                                    
                                       Burundi
                                    
                                    
                                       BI
                                    
                                    
                                       BDI
                                    
                                    
                                       RU
                                    
                                 
                                 
                                    
                                       Cambodia
                                    
                                    
                                       Kambodscha
                                    
                                    
                                       KH
                                    
                                    
                                       KHM
                                    
                                    
                                       K
                                    
                                 
                                 
                                    
                                       Cameroon
                                    
                                    
                                       Kamerun
                                    
                                    
                                       CM
                                    
                                    
                                       CMR
                                    
                                    
                                       CAM
                                    
                                 
                                 
                                    
                                       Canada
                                    
                                    
                                       Kanada
                                    
                                    
                                       CA
                                    
                                    
                                       CAN
                                    
                                    
                                       CDN
                                    
                                 
                                 
                                    
                                       Cape Verde
                                    
                                    
                                       Kap Verde
                                    
                                    
                                       CV
                                    
                                    
                                       CPV
                                    
                                    
                                       CV
                                    
                                 
                                 
                                    
                                       Cayman Islands
                                    
                                    
                                       Kaimaninseln
                                    
                                    
                                       KY
                                    
                                    
                                       CYM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Central African Republic
                                    
                                    
                                       Zentralafrikanische Republik
                                    
                                    
                                       CF
                                    
                                    
                                       CAF
                                    
                                    
                                       RCA
                                    
                                 
                                 
                                    
                                       Chad
                                    
                                    
                                       Tschad
                                    
                                    
                                       TD
                                    
                                    
                                       TCD
                                    
                                    
                                       TD
                                    
                                 
                                 
                                    
                                       Chile
                                    
                                    
                                       Chile
                                    
                                    
                                       CL
                                    
                                    
                                       CHL
                                    
                                    
                                       RCH
                                    
                                 
                                 
                                    
                                       China
                                    
                                    
                                       China, Volksrepublik
                                    
                                    
                                       CN
                                    
                                    
                                       CHN
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Christmas Island
                                    
                                    
                                       Weihnachtsinsel
                                    
                                    
                                       CX
                                    
                                    
                                       CXR
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Cocos (Keeling) Islands
                                    
                                    
                                       Kokosinseln
                                    
                                    
                                       CC
                                    
                                    
                                       CCK
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Colombia
                                    
                                    
                                       Kolumbien
                                    
                                    
                                       CO
                                    
                                    
                                       COL
                                    
                                    
                                       CO
                                    
                                 
                                 
                                    
                                       Comoros
                                    
                                    
                                       Komoren
                                    
                                    
                                       KM
                                    
                                    
                                       COM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Congo (Brazzaville)
                                    
                                    
                                       Republik Kongo
                                    
                                    
                                       CG
                                    
                                    
                                       COG
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Congo, Democratic Republic of the
                                    
                                    
                                       Kongo, Demokratische Republik (ehem. Zaire)
                                    
                                    
                                       CD
                                    
                                    
                                       COD
                                    
                                    
                                       CGO
                                    
                                 
                                 
                                    
                                       Cook Islands
                                    
                                    
                                       Cookinseln
                                    
                                    
                                       CK
                                    
                                    
                                       COK
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Costa Rica
                                    
                                    
                                       Costa Rica
                                    
                                    
                                       CR
                                    
                                    
                                       CRI
                                    
                                    
                                       CR
                                    
                                 
                                 
                                    
                                       Côte d'Ivoire
                                    
                                    
                                       Côte d’Ivoire (Elfenbeinküste)
                                    
                                    
                                       CI
                                    
                                    
                                       CIV
                                    
                                    
                                       CI
                                    
                                 
                                 
                                    
                                       Croatia
                                    
                                    
                                       Kroatien
                                    
                                    
                                       HR
                                    
                                    
                                       HRV
                                    
                                    
                                       HR
                                    
                                 
                                 
                                    
                                       Cuba
                                    
                                    
                                       Kuba
                                    
                                    
                                       CU
                                    
                                    
                                       CUB
                                    
                                    
                                       C
                                    
                                 
                                 
                                    
                                       Cyprus
                                    
                                    
                                       Zypern
                                    
                                    
                                       CY
                                    
                                    
                                       CYP
                                    
                                    
                                       CY
                                    
                                 
                                 
                                    
                                       Czech Republic
                                    
                                    
                                       Tschechische Republik
                                    
                                    
                                       CZ
                                    
                                    
                                       CZE
                                    
                                    
                                       CZ
                                    
                                 
                                 
                                    
                                       Denmark
                                    
                                    
                                       Dänemark
                                    
                                    
                                       DK
                                    
                                    
                                       DNK
                                    
                                    
                                       DK
                                    
                                 
                                 
                                    
                                       Djibouti
                                    
                                    
                                       Dschibuti
                                    
                                    
                                       DJ
                                    
                                    
                                       DJI
                                    
                                    
                                       DJI
                                    
                                 
                                 
                                    
                                       Dominica
                                    
                                    
                                       Dominica
                                    
                                    
                                       DM
                                    
                                    
                                       DMA
                                    
                                    
                                       WD
                                    
                                 
                                 
                                    
                                       Dominican Republic
                                    
                                    
                                       Dominikanische Republik
                                    
                                    
                                       DO
                                    
                                    
                                       DOM
                                    
                                    
                                       DOM
                                    
                                 
                                 
                                    
                                       Ecuador
                                    
                                    
                                       Ecuador
                                    
                                    
                                       EC
                                    
                                    
                                       ECU
                                    
                                    
                                       EC
                                    
                                 
                                 
                                    
                                       Egypt
                                    
                                    
                                       Ägypten
                                    
                                    
                                       EG
                                    
                                    
                                       EGY
                                    
                                    
                                       ET
                                    
                                 
                                 
                                    
                                       El Salvador
                                    
                                    
                                       El Salvador
                                    
                                    
                                       SV
                                    
                                    
                                       SLV
                                    
                                    
                                       ES
                                    
                                 
                                 
                                    
                                       Equatorial Guinea
                                    
                                    
                                       Äquatorialguinea
                                    
                                    
                                       GQ
                                    
                                    
                                       GNQ
                                    
                                    
                                       GQ
                                    
                                 
                                 
                                    
                                       Eritrea
                                    
                                    
                                       Eritrea
                                    
                                    
                                       ER
                                    
                                    
                                       ERI
                                    
                                    
                                       ER 
                                    
                                 
                                 
                                    
                                       Estonia
                                    
                                    
                                       Estland
                                    
                                    
                                       EE
                                    
                                    
                                       EST
                                    
                                    
                                       EST
                                    
                                 
                                 
                                    
                                       Ethiopia
                                    
                                    
                                       Äthiopien
                                    
                                    
                                       ET
                                    
                                    
                                       ETH
                                    
                                    
                                       ETH
                                    
                                 
                                 
                                    
                                       Falkland Islands (Malvinas)
                                    
                                    
                                       Falklandinseln
                                    
                                    
                                       FK
                                    
                                    
                                       FLK
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Faroe Islands
                                    
                                    
                                       Färöer
                                    
                                    
                                       FO
                                    
                                    
                                       FRO
                                    
                                    
                                       FO
                                    
                                 
                                 
                                    
                                       Fiji
                                    
                                    
                                       Fidschi
                                    
                                    
                                       FJ
                                    
                                    
                                       FJI
                                    
                                    
                                       FJI
                                    
                                 
                                 
                                    
                                       Finland
                                    
                                    
                                       Finnland (früher SF)
                                    
                                    
                                       FI
                                    
                                    
                                       FIN
                                    
                                    
                                       FIN
                                    
                                 
                                 
                                    
                                       France
                                    
                                    
                                       Frankreich
                                    
                                    
                                       FR
                                    
                                    
                                       FRA
                                    
                                    
                                       F
                                    
                                 
                                 
                                    
                                       French Guiana
                                    
                                    
                                       Französisch-Guayana
                                    
                                    
                                       GF
                                    
                                    
                                       GUF
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       French Polynesia
                                    
                                    
                                       Französisch-Polynesien
                                    
                                    
                                       PF
                                    
                                    
                                       PYF
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       French Southern Territories
                                    
                                    
                                       Französische Süd- und Antarktisgebiete
                                    
                                    
                                       TF
                                    
                                    
                                       ATF
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Gabon
                                    
                                    
                                       Gabun
                                    
                                    
                                       GA
                                    
                                    
                                       GAB
                                    
                                    
                                       G
                                    
                                 
                                 
                                    
                                       Gambia
                                    
                                    
                                       Gambia
                                    
                                    
                                       GM
                                    
                                    
                                       GMB
                                    
                                    
                                       WAG
                                    
                                 
                                 
                                    
                                       Georgia
                                    
                                    
                                       Georgien
                                    
                                    
                                       GE
                                    
                                    
                                       GEO
                                    
                                    
                                       GE
                                    
                                 
                                 
                                    
                                       Germany
                                    
                                    
                                       Deutschland
                                    
                                    
                                       DE
                                    
                                    
                                       DEU
                                    
                                    
                                       D
                                    
                                 
                                 
                                    
                                       Ghana
                                    
                                    
                                       Ghana
                                    
                                    
                                       GH
                                    
                                    
                                       GHA
                                    
                                    
                                       GH
                                    
                                 
                                 
                                    
                                       Gibraltar
                                    
                                    
                                       Gibraltar
                                    
                                    
                                       GI
                                    
                                    
                                       GIB
                                    
                                    
                                       GBZ
                                    
                                 
                                 
                                    
                                       Greece
                                    
                                    
                                       Griechenland
                                    
                                    
                                       GR
                                    
                                    
                                       GRC
                                    
                                    
                                       GR
                                    
                                 
                                 
                                    
                                       Greenland
                                    
                                    
                                       Grönland
                                    
                                    
                                       GL
                                    
                                    
                                       GRL
                                    
                                    
                                       KN
                                    
                                 
                                 
                                    
                                       Grenada
                                    
                                    
                                       Grenada
                                    
                                    
                                       GD
                                    
                                    
                                       GRD
                                    
                                    
                                       WG
                                    
                                 
                                 
                                    
                                       Guadeloupe
                                    
                                    
                                       Guadeloupe
                                    
                                    
                                       GP
                                    
                                    
                                       GLP
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Guam
                                    
                                    
                                       Guam
                                    
                                    
                                       GU
                                    
                                    
                                       GUM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Guatemala
                                    
                                    
                                       Guatemala
                                    
                                    
                                       GT
                                    
                                    
                                       GTM
                                    
                                    
                                       GCA
                                    
                                 
                                 
                                    
                                       Guernsey
                                    
                                    
                                       Guernsey (Kanalinsel)
                                    
                                    
                                       GG
                                    
                                    
                                       GGY
                                    
                                    
                                       GBG
                                    
                                 
                                 
                                    
                                       Guinea
                                    
                                    
                                       Guinea
                                    
                                    
                                       GN
                                    
                                    
                                       GIN
                                    
                                    
                                       RG
                                    
                                 
                                 
                                    
                                       Guinea-Bissau
                                    
                                    
                                       Guinea-Bissau
                                    
                                    
                                       GW
                                    
                                    
                                       GNB
                                    
                                    
                                       GUB
                                    
                                 
                                 
                                    
                                       Guyana
                                    
                                    
                                       Guyana
                                    
                                    
                                       GY
                                    
                                    
                                       GUY
                                    
                                    
                                       GUY
                                    
                                 
                                 
                                    
                                       Haiti
                                    
                                    
                                       Haiti
                                    
                                    
                                       HT
                                    
                                    
                                       HTI
                                    
                                    
                                       RH
                                    
                                 
                                 
                                    
                                       Heard Island and Mcdonald Islands
                                    
                                    
                                       Heard und McDonaldinseln
                                    
                                    
                                       HM
                                    
                                    
                                       HMD
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Holy See (Vatican City State)
                                    
                                    
                                       Vatikanstadt
                                    
                                    
                                       VA
                                    
                                    
                                       VAT
                                    
                                    
                                       V
                                    
                                 
                                 
                                    
                                       Honduras
                                    
                                    
                                       Honduras
                                    
                                    
                                       HN
                                    
                                    
                                       HND
                                    
                                    
                                       HN
                                    
                                 
                                 
                                    
                                       Hong Kong, Special Administrative Region of China
                                    
                                    
                                       Hongkong
                                    
                                    
                                       HK
                                    
                                    
                                       HKG
                                    
                                    
                                       HK
                                    
                                 
                                 
                                    
                                       Hungary
                                    
                                    
                                       Ungarn
                                    
                                    
                                       HU
                                    
                                    
                                       HUN
                                    
                                    
                                       H
                                    
                                 
                                 
                                    
                                       Iceland
                                    
                                    
                                       Island
                                    
                                    
                                       IS
                                    
                                    
                                       ISL
                                    
                                    
                                       IS
                                    
                                 
                                 
                                    
                                       India
                                    
                                    
                                       Indien
                                    
                                    
                                       IN
                                    
                                    
                                       IND
                                    
                                    
                                       IND
                                    
                                 
                                 
                                    
                                       Indonesia
                                    
                                    
                                       Indonesien
                                    
                                    
                                       ID
                                    
                                    
                                       IDN
                                    
                                    
                                       RI
                                    
                                 
                                 
                                    
                                       Iran, Islamic Republic of
                                    
                                    
                                       Iran, Islamische Republik
                                    
                                    
                                       IR
                                    
                                    
                                       IRN
                                    
                                    
                                       IR
                                    
                                 
                                 
                                    
                                       Iraq
                                    
                                    
                                       Irak
                                    
                                    
                                       IQ
                                    
                                    
                                       IRQ
                                    
                                    
                                       IRQ
                                    
                                 
                                 
                                    
                                       Ireland
                                    
                                    
                                       Irland
                                    
                                    
                                       IE
                                    
                                    
                                       IRL
                                    
                                    
                                       IRL
                                    
                                 
                                 
                                    
                                       Isle of Man
                                    
                                    
                                       Insel Man
                                    
                                    
                                       IM
                                    
                                    
                                       IMN
                                    
                                    
                                       GBM
                                    
                                 
                                 
                                    
                                       Israel
                                    
                                    
                                       Israel
                                    
                                    
                                       IL
                                    
                                    
                                       ISR
                                    
                                    
                                       IL
                                    
                                 
                                 
                                    
                                       Italy
                                    
                                    
                                       Italien
                                    
                                    
                                       IT
                                    
                                    
                                       ITA
                                    
                                    
                                       I
                                    
                                 
                                 
                                    
                                       Jamaica
                                    
                                    
                                       Jamaika
                                    
                                    
                                       JM
                                    
                                    
                                       JAM
                                    
                                    
                                       JA
                                    
                                 
                                 
                                    
                                       Japan
                                    
                                    
                                       Japan
                                    
                                    
                                       JP
                                    
                                    
                                       JPN
                                    
                                    
                                       J
                                    
                                 
                                 
                                    
                                       Jersey
                                    
                                    
                                       Jersey (Kanalinsel)
                                    
                                    
                                       JE
                                    
                                    
                                       JEY
                                    
                                    
                                       GBJ
                                    
                                 
                                 
                                    
                                       Jordan
                                    
                                    
                                       Jordanien
                                    
                                    
                                       JO
                                    
                                    
                                       JOR
                                    
                                    
                                       JOR
                                    
                                 
                                 
                                    
                                       Kazakhstan
                                    
                                    
                                       Kasachstan
                                    
                                    
                                       KZ
                                    
                                    
                                       KAZ
                                    
                                    
                                       KZ
                                    
                                 
                                 
                                    
                                       Kenya
                                    
                                    
                                       Kenia
                                    
                                    
                                       KE
                                    
                                    
                                       KEN
                                    
                                    
                                       EAK
                                    
                                 
                                 
                                    
                                       Kiribati
                                    
                                    
                                       Kiribati
                                    
                                    
                                       KI
                                    
                                    
                                       KIR
                                    
                                    
                                       KIR
                                    
                                 
                                 
                                    
                                       Korea, Democratic People's Republic of
                                    
                                    
                                       Korea, Demokratische Volksrepublik (Nordkorea)
                                    
                                    
                                       KP
                                    
                                    
                                       PRK
                                    
                                    
                                       KP
                                    
                                 
                                 
                                    
                                       Korea, Republic of
                                    
                                    
                                       Korea, Republik (Südkorea)
                                    
                                    
                                       KR
                                    
                                    
                                       KOR
                                    
                                    
                                       ROK
                                    
                                 
                                 
                                    
                                       Kuwait
                                    
                                    
                                       Kuwait
                                    
                                    
                                       KW
                                    
                                    
                                       KWT
                                    
                                    
                                       KWT
                                    
                                 
                                 
                                    
                                       Kyrgyzstan
                                    
                                    
                                       Kirgisistan
                                    
                                    
                                       KG
                                    
                                    
                                       KGZ
                                    
                                    
                                       KS
                                    
                                 
                                 
                                    
                                       Lao PDR
                                    
                                    
                                       Laos, Demokratische Volksrepublik
                                    
                                    
                                       LA
                                    
                                    
                                       LAO
                                    
                                    
                                       LAO
                                    
                                 
                                 
                                    
                                       Latvia
                                    
                                    
                                       Lettland
                                    
                                    
                                       LV
                                    
                                    
                                       LVA
                                    
                                    
                                       LV
                                    
                                 
                                 
                                    
                                       Lebanon
                                    
                                    
                                       Libanon
                                    
                                    
                                       LB
                                    
                                    
                                       LBN
                                    
                                    
                                       RL
                                    
                                 
                                 
                                    
                                       Lesotho
                                    
                                    
                                       Lesotho
                                    
                                    
                                       LS
                                    
                                    
                                       LSO
                                    
                                    
                                       LS
                                    
                                 
                                 
                                    
                                       Liberia
                                    
                                    
                                       Liberia
                                    
                                    
                                       LR
                                    
                                    
                                       LBR
                                    
                                    
                                       LB
                                    
                                 
                                 
                                    
                                       Libya
                                    
                                    
                                       Libyen
                                    
                                    
                                       LY
                                    
                                    
                                       LBY
                                    
                                    
                                       LAR
                                    
                                 
                                 
                                    
                                       Liechtenstein
                                    
                                    
                                       Liechtenstein
                                    
                                    
                                       LI
                                    
                                    
                                       LIE
                                    
                                    
                                       FL
                                    
                                 
                                 
                                    
                                       Lithuania
                                    
                                    
                                       Litauen
                                    
                                    
                                       LT
                                    
                                    
                                       LTU
                                    
                                    
                                       LT
                                    
                                 
                                 
                                    
                                       Luxembourg
                                    
                                    
                                       Luxemburg
                                    
                                    
                                       LU
                                    
                                    
                                       LUX
                                    
                                    
                                       L
                                    
                                 
                                 
                                    
                                       Macao, Special Administrative Region of China
                                    
                                    
                                       Macau
                                    
                                    
                                       MO
                                    
                                    
                                       MAC
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Macedonia, Republic of
                                    
                                    
                                       Mazedonien
                                    
                                    
                                       MK
                                    
                                    
                                       MKD
                                    
                                    
                                       MK
                                    
                                 
                                 
                                    
                                       Madagascar
                                    
                                    
                                       Madagaskar
                                    
                                    
                                       MG
                                    
                                    
                                       MDG
                                    
                                    
                                       RM
                                    
                                 
                                 
                                    
                                       Malawi
                                    
                                    
                                       Malawi
                                    
                                    
                                       MW
                                    
                                    
                                       MWI
                                    
                                    
                                       MW
                                    
                                 
                                 
                                    
                                       Malaysia
                                    
                                    
                                       Malaysia
                                    
                                    
                                       MY
                                    
                                    
                                       MYS
                                    
                                    
                                       MAL
                                    
                                 
                                 
                                    
                                       Maldives
                                    
                                    
                                       Malediven
                                    
                                    
                                       MV
                                    
                                    
                                       MDV
                                    
                                    
                                       MV
                                    
                                 
                                 
                                    
                                       Mali
                                    
                                    
                                       Mali
                                    
                                    
                                       ML
                                    
                                    
                                       MLI
                                    
                                    
                                       RMM
                                    
                                 
                                 
                                    
                                       Malta
                                    
                                    
                                       Malta
                                    
                                    
                                       MT
                                    
                                    
                                       MLT
                                    
                                    
                                       M
                                    
                                 
                                 
                                    
                                       Marshall Islands
                                    
                                    
                                       Marshallinseln
                                    
                                    
                                       MH
                                    
                                    
                                       MHL
                                    
                                    
                                       MH
                                    
                                 
                                 
                                    
                                       Martinique
                                    
                                    
                                       Martinique
                                    
                                    
                                       MQ
                                    
                                    
                                       MTQ
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Mauritania
                                    
                                    
                                       Mauretanien
                                    
                                    
                                       MR
                                    
                                    
                                       MRT
                                    
                                    
                                       RIM
                                    
                                 
                                 
                                    
                                       Mauritius
                                    
                                    
                                       Mauritius
                                    
                                    
                                       MU
                                    
                                    
                                       MUS
                                    
                                    
                                       MS
                                    
                                 
                                 
                                    
                                       Mayotte
                                    
                                    
                                       Namibia
                                    
                                    
                                       NA
                                    
                                    
                                       NAM
                                    
                                    
                                       NAM
                                    
                                 
                                 
                                    
                                       Mexico
                                    
                                    
                                       Mexiko
                                    
                                    
                                       MX
                                    
                                    
                                       MEX
                                    
                                    
                                       MEX
                                    
                                 
                                 
                                    
                                       Micronesia, Federated States of
                                    
                                    
                                       Mikronesien
                                    
                                    
                                       FM
                                    
                                    
                                       FSM
                                    
                                    
                                       FSM
                                    
                                 
                                 
                                    
                                       Moldova
                                    
                                    
                                       Moldawien (Republik Moldau)
                                    
                                    
                                       MD
                                    
                                    
                                       MDA
                                    
                                    
                                       MD
                                    
                                 
                                 
                                    
                                       Monaco
                                    
                                    
                                       Monaco
                                    
                                    
                                       MC
                                    
                                    
                                       MCO
                                    
                                    
                                       MC
                                    
                                 
                                 
                                    
                                       Mongolia
                                    
                                    
                                       Mongolei
                                    
                                    
                                       MN
                                    
                                    
                                       MNG
                                    
                                    
                                       MGL
                                    
                                 
                                 
                                    
                                       Montenegro
                                    
                                    
                                       Montenegro
                                    
                                    
                                       ME
                                    
                                    
                                       MNE
                                    
                                    
                                       MNE
                                    
                                 
                                 
                                    
                                       Montserrat
                                    
                                    
                                       Montserrat
                                    
                                    
                                       MS
                                    
                                    
                                       MSR
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Morocco
                                    
                                    
                                       Marokko
                                    
                                    
                                       MA
                                    
                                    
                                       MAR
                                    
                                    
                                       MA
                                    
                                 
                                 
                                    
                                       Mozambique
                                    
                                    
                                       Mosambik
                                    
                                    
                                       MZ
                                    
                                    
                                       MOZ
                                    
                                    
                                       MOC
                                    
                                 
                                 
                                    
                                       Myanmar
                                    
                                    
                                       Myanmar (Burma)
                                    
                                    
                                       MM
                                    
                                    
                                       MMR
                                    
                                    
                                       Mya
                                    
                                 
                                 
                                    
                                       Namibia
                                    
                                    
                                       Neukaledonien
                                    
                                    
                                       NC
                                    
                                    
                                       NCL
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Nauru
                                    
                                    
                                       Neutrale Zone (Saudi-Arabien und Irak bis 1993)
                                    
                                    
                                       NT
                                    
                                    
                                       NTZ
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Nepal
                                    
                                    
                                       Nauru
                                    
                                    
                                       NR
                                    
                                    
                                       NRU
                                    
                                    
                                       NAU
                                    
                                 
                                 
                                    
                                       Norway
                                    
                                    
                                       Norwegen
                                    
                                    
                                       NO
                                    
                                    
                                       NOR
                                    
                                    
                                       N
                                    
                                 
                                 
                                    
                                       Netherlands Antilles
                                    
                                    
                                       Niederländische Antillen (historisch)
                                    
                                    
                                       AN
                                    
                                    
                                       ANT
                                    
                                    
                                       NA
                                    
                                 
                                 
                                    
                                       New Caledonia
                                    
                                    
                                       Niger
                                    
                                    
                                       NE
                                    
                                    
                                       NER
                                    
                                    
                                       RN
                                    
                                 
                                 
                                    
                                       New Zealand
                                    
                                    
                                       Neuseeland
                                    
                                    
                                       NZ
                                    
                                    
                                       NZL
                                    
                                    
                                       NZ
                                    
                                 
                                 
                                    
                                       Nicaragua
                                    
                                    
                                       Niue
                                    
                                    
                                       NU
                                    
                                    
                                       NIU
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Niger
                                    
                                    
                                       Norfolkinsel
                                    
                                    
                                       NF
                                    
                                    
                                       NFK
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Nigeria
                                    
                                    
                                       Nicaragua
                                    
                                    
                                       NI
                                    
                                    
                                       NIC
                                    
                                    
                                       Nic
                                    
                                 
                                 
                                    
                                       Niue
                                    
                                    
                                       Niederlande
                                    
                                    
                                       NL
                                    
                                    
                                       NLD
                                    
                                    
                                       NL
                                    
                                 
                                 
                                    
                                       Norfolk Island
                                    
                                    
                                       Nigeria
                                    
                                    
                                       NG
                                    
                                    
                                       NGA
                                    
                                    
                                       NGR
                                    
                                 
                                 
                                    
                                       Northern Mariana Islands
                                    
                                    
                                       Nördliche Marianen
                                    
                                    
                                       MP
                                    
                                    
                                       MNP
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Norway
                                    
                                    
                                       Nepal
                                    
                                    
                                       NP
                                    
                                    
                                       NPL
                                    
                                    
                                       NEP
                                    
                                 
                                 
                                    
                                       Oman
                                    
                                    
                                       Oman
                                    
                                    
                                       OM
                                    
                                    
                                       OMN
                                    
                                    
                                       OM
                                    
                                 
                                 
                                    
                                       Pakistan
                                    
                                    
                                       Pakistan
                                    
                                    
                                       PK
                                    
                                    
                                       PAK
                                    
                                    
                                       PK
                                    
                                 
                                 
                                    
                                       Palau
                                    
                                    
                                       Palau
                                    
                                    
                                       PW
                                    
                                    
                                       PLW
                                    
                                    
                                       PAL
                                    
                                 
                                 
                                    
                                       Palestinian Territory, Occupied
                                    
                                    
                                       Palästina
                                    
                                    
                                       PS
                                    
                                    
                                       PSE
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Panama
                                    
                                    
                                       Panama
                                    
                                    
                                       PA
                                    
                                    
                                       PAN
                                    
                                    
                                       PA
                                    
                                 
                                 
                                    
                                       Papua New Guinea
                                    
                                    
                                       Papua-Neuguinea
                                    
                                    
                                       PG
                                    
                                    
                                       PNG
                                    
                                    
                                       PNG
                                    
                                 
                                 
                                    
                                       Paraguay
                                    
                                    
                                       Paraguay
                                    
                                    
                                       PY
                                    
                                    
                                       PRY
                                    
                                    
                                       PY
                                    
                                 
                                 
                                    
                                       Peru
                                    
                                    
                                       Peru
                                    
                                    
                                       PE
                                    
                                    
                                       PER
                                    
                                    
                                       PE
                                    
                                 
                                 
                                    
                                       Philippines
                                    
                                    
                                       Philippinen
                                    
                                    
                                       PH
                                    
                                    
                                       PHL
                                    
                                    
                                       RP
                                    
                                 
                                 
                                    
                                       Pitcairn
                                    
                                    
                                       Pitcairninseln
                                    
                                    
                                       PN
                                    
                                    
                                       PCN
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Poland
                                    
                                    
                                       Polen
                                    
                                    
                                       PL
                                    
                                    
                                       POL
                                    
                                    
                                       PL
                                    
                                 
                                 
                                    
                                       Portugal
                                    
                                    
                                       Portugal
                                    
                                    
                                       PT
                                    
                                    
                                       PRT
                                    
                                    
                                       P
                                    
                                 
                                 
                                    
                                       Puerto Rico
                                    
                                    
                                       Puerto Rico
                                    
                                    
                                       PR
                                    
                                    
                                       PRI
                                    
                                    
                                       PRI
                                    
                                 
                                 
                                    
                                       Qatar
                                    
                                    
                                       Katar
                                    
                                    
                                       QA
                                    
                                    
                                       QAT
                                    
                                    
                                       Q
                                    
                                 
                                 
                                    
                                       Réunion
                                    
                                    
                                       Réunion
                                    
                                    
                                       RE
                                    
                                    
                                       REU
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Romania
                                    
                                    
                                       Rumänien
                                    
                                    
                                       RO
                                    
                                    
                                       ROU
                                    
                                    
                                       RO
                                    
                                 
                                 
                                    
                                       Russian Federation
                                    
                                    
                                       Russische Föderation
                                    
                                    
                                       RU
                                    
                                    
                                       RUS
                                    
                                    
                                       RUS
                                    
                                 
                                 
                                    
                                       Rwanda
                                    
                                    
                                       Ruanda
                                    
                                    
                                       RW
                                    
                                    
                                       RWA
                                    
                                    
                                       RWA
                                    
                                 
                                 
                                    
                                       Saint Helena
                                    
                                    
                                       St. Helena
                                    
                                    
                                       SH
                                    
                                    
                                       SHN
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Saint Kitts and Nevis
                                    
                                    
                                       St. Kitts und Nevis
                                    
                                    
                                       KN
                                    
                                    
                                       KNA
                                    
                                    
                                       KANN
                                    
                                 
                                 
                                    
                                       Saint Lucia
                                    
                                    
                                       St. Lucia
                                    
                                    
                                       LC
                                    
                                    
                                       LCA
                                    
                                    
                                       WL
                                    
                                 
                                 
                                    
                                       Saint Pierre and Miquelon
                                    
                                    
                                       Saint-Pierre und Miquelon
                                    
                                    
                                       PM
                                    
                                    
                                       SPM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Saint Vincent and Grenadines
                                    
                                    
                                       St. Vincent und die Grenadinen
                                    
                                    
                                       VC
                                    
                                    
                                       VCT
                                    
                                    
                                       WV
                                    
                                 
                                 
                                    
                                       Saint-Barthélemy
                                    
                                    
                                       Saint-Barthélemy
                                    
                                    
                                       BL
                                    
                                    
                                       BLM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Saint-Martin (French part)
                                    
                                    
                                       Saint-Martin (franz. Teil)
                                    
                                    
                                       MF
                                    
                                    
                                       MAF
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Samoa
                                    
                                    
                                       Samoa
                                    
                                    
                                       WS
                                    
                                    
                                       WSM
                                    
                                    
                                       WS
                                    
                                 
                                 
                                    
                                       San Marino
                                    
                                    
                                       San Marino
                                    
                                    
                                       SM
                                    
                                    
                                       SMR
                                    
                                    
                                       RSM
                                    
                                 
                                 
                                    
                                       Sao Tome and Principe
                                    
                                    
                                       Sao Tome u. Principe
                                    
                                    
                                       ST
                                    
                                    
                                       STP
                                    
                                    
                                       STP
                                    
                                 
                                 
                                    
                                       Saudi Arabia
                                    
                                    
                                       Saudi-Arabien
                                    
                                    
                                       SA
                                    
                                    
                                       SAU
                                    
                                    
                                       KSA
                                    
                                 
                                 
                                    
                                       Senegal
                                    
                                    
                                       Senegal
                                    
                                    
                                       SN
                                    
                                    
                                       SEN
                                    
                                    
                                       SN
                                    
                                 
                                 
                                    
                                       Serbia
                                    
                                    
                                       Serbien
                                    
                                    
                                       RS
                                    
                                    
                                       SRB
                                    
                                    
                                       SRB
                                    
                                 
                                 
                                    
                                       Seychelles
                                    
                                    
                                       Seychellen
                                    
                                    
                                       SC
                                    
                                    
                                       SYC
                                    
                                    
                                       SY
                                    
                                 
                                 
                                    
                                       Sierra Leone
                                    
                                    
                                       Sierra Leone
                                    
                                    
                                       SL
                                    
                                    
                                       SLE
                                    
                                    
                                       WAL
                                    
                                 
                                 
                                    
                                       Singapore
                                    
                                    
                                       Singapur
                                    
                                    
                                       SG
                                    
                                    
                                       SGP
                                    
                                    
                                       SGP
                                    
                                 
                                 
                                    
                                       Slovakia
                                    
                                    
                                       Slowakei
                                    
                                    
                                       SK
                                    
                                    
                                       SVK
                                    
                                    
                                       SK
                                    
                                 
                                 
                                    
                                       Slovenia
                                    
                                    
                                       Slowenien
                                    
                                    
                                       SI
                                    
                                    
                                       SVN
                                    
                                    
                                       SLO
                                    
                                 
                                 
                                    
                                       Solomon Islands
                                    
                                    
                                       Salomonen
                                    
                                    
                                       SB
                                    
                                    
                                       SLB
                                    
                                    
                                       SOL
                                    
                                 
                                 
                                    
                                       Somalia
                                    
                                    
                                       Somalia
                                    
                                    
                                       SO
                                    
                                    
                                       SOM
                                    
                                    
                                       SO
                                    
                                 
                                 
                                    
                                       South Africa
                                    
                                    
                                       Südafrika (früher SAU)
                                    
                                    
                                       ZA
                                    
                                    
                                       ZAF
                                    
                                    
                                       ZA
                                    
                                 
                                 
                                    
                                       South Georgia and the South Sandwich Islands
                                    
                                    
                                       Südgeorgien und die Südlichen Sandwichinseln
                                    
                                    
                                       GS
                                    
                                    
                                       SGS
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       South Sudan
                                    
                                    
                                       Südsudan
                                    
                                    
                                       SS
                                    
                                    
                                       SSD
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Spain
                                    
                                    
                                       Spanien
                                    
                                    
                                       ES
                                    
                                    
                                       ESP
                                    
                                    
                                       E
                                    
                                 
                                 
                                    
                                       Sri Lanka
                                    
                                    
                                       Sri Lanka
                                    
                                    
                                       LK
                                    
                                    
                                       LKA
                                    
                                    
                                       CL
                                    
                                 
                                 
                                    
                                       Sudan
                                    
                                    
                                       Sudan
                                    
                                    
                                       SD
                                    
                                    
                                       SDN
                                    
                                    
                                       SUD
                                    
                                 
                                 
                                    
                                       Suriname *
                                    
                                    
                                       Suriname
                                    
                                    
                                       SR
                                    
                                    
                                       SUR
                                    
                                    
                                       SME
                                    
                                 
                                 
                                    
                                       Svalbard and Jan Mayen Islands
                                    
                                    
                                       Svalbard und Jan Mayen
                                    
                                    
                                       SJ
                                    
                                    
                                       SJM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Swaziland
                                    
                                    
                                       Swasiland
                                    
                                    
                                       SZ
                                    
                                    
                                       SWZ
                                    
                                    
                                       SD
                                    
                                 
                                 
                                    
                                       Sweden
                                    
                                    
                                       Schweden
                                    
                                    
                                       SE
                                    
                                    
                                       SWE
                                    
                                    
                                       S
                                    
                                 
                                 
                                    
                                       Switzerland
                                    
                                    
                                       Schweiz (Confoederatio Helvetica)
                                    
                                    
                                       CH
                                    
                                    
                                       CHE
                                    
                                    
                                       CH
                                    
                                 
                                 
                                    
                                       Syrian Arab Republic (Syria)
                                    
                                    
                                       Syrien, Arabische Republik
                                    
                                    
                                       SY
                                    
                                    
                                       SYR
                                    
                                    
                                       SYR
                                    
                                 
                                 
                                    
                                       Taiwan, Republic of China
                                    
                                    
                                       Republik China (Taiwan)
                                    
                                    
                                       TW
                                    
                                    
                                       TWN
                                    
                                    
                                       RC
                                    
                                 
                                 
                                    
                                       Tajikistan
                                    
                                    
                                       Tadschikistan
                                    
                                    
                                       TJ
                                    
                                    
                                       TJK
                                    
                                    
                                       TJ
                                    
                                 
                                 
                                    
                                       Tanzania *, United Republic of
                                    
                                    
                                       Tansania, Vereinigte Republik
                                    
                                    
                                       TZ
                                    
                                    
                                       TZA
                                    
                                    
                                       EAT
                                    
                                 
                                 
                                    
                                       Thailand
                                    
                                    
                                       Thailand
                                    
                                    
                                       TH
                                    
                                    
                                       THA
                                    
                                    
                                       T
                                    
                                 
                                 
                                    
                                       Timor-Leste
                                    
                                    
                                       Osttimor (Timor-Leste)
                                    
                                    
                                       TL
                                    
                                    
                                       TLS
                                    
                                    
                                       TL
                                    
                                 
                                 
                                    
                                       Togo
                                    
                                    
                                       Togo
                                    
                                    
                                       TG
                                    
                                    
                                       TGO
                                    
                                    
                                       TG
                                    
                                 
                                 
                                    
                                       Tokelau
                                    
                                    
                                       Tokelau
                                    
                                    
                                       TK
                                    
                                    
                                       TKL
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Tonga
                                    
                                    
                                       Tonga
                                    
                                    
                                       TO
                                    
                                    
                                       TON
                                    
                                    
                                       TON
                                    
                                 
                                 
                                    
                                       Trinidad and Tobago
                                    
                                    
                                       Trinidad und Tobago
                                    
                                    
                                       TT
                                    
                                    
                                       TTO
                                    
                                    
                                       TT
                                    
                                 
                                 
                                    
                                       Tunisia
                                    
                                    
                                       Tunesien
                                    
                                    
                                       TN
                                    
                                    
                                       TUN
                                    
                                    
                                       TN
                                    
                                 
                                 
                                    
                                       Turkey
                                    
                                    
                                       Türkei
                                    
                                    
                                       TR
                                    
                                    
                                       TUR
                                    
                                    
                                       TR
                                    
                                 
                                 
                                    
                                       Turkmenistan
                                    
                                    
                                       Turkmenistan
                                    
                                    
                                       TM
                                    
                                    
                                       TKM
                                    
                                    
                                       TM
                                    
                                 
                                 
                                    
                                       Turks and Caicos Islands
                                    
                                    
                                       Turks- und Caicosinseln
                                    
                                    
                                       TC
                                    
                                    
                                       TCA
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Tuvalu
                                    
                                    
                                       Tuvalu
                                    
                                    
                                       TV
                                    
                                    
                                       TUV
                                    
                                    
                                       TUV
                                    
                                 
                                 
                                    
                                       Uganda
                                    
                                    
                                       Uganda
                                    
                                    
                                       UG
                                    
                                    
                                       UGA
                                    
                                    
                                       EAU
                                    
                                 
                                 
                                    
                                       Ukraine
                                    
                                    
                                       Ukraine
                                    
                                    
                                       UA
                                    
                                    
                                       UKR
                                    
                                    
                                       UA
                                    
                                 
                                 
                                    
                                       United Arab Emirates
                                    
                                    
                                       Vereinigte Arabische Emirate
                                    
                                    
                                       AE
                                    
                                    
                                       ARE
                                    
                                    
                                       UAE
                                    
                                 
                                 
                                    
                                       United Kingdom
                                    
                                    
                                       Vereinigtes Königreich Großbritannien und Nordirland
                                    
                                    
                                       GB (und UK[1])
                                    
                                    
                                       GBR
                                    
                                    
                                       GB
                                    
                                 
                                 
                                    
                                       United States Minor Outlying Islands
                                    
                                    
                                       United States Minor Outlying Islands
                                    
                                    
                                       UM
                                    
                                    
                                       UMI
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       United States of America
                                    
                                    
                                       USA (früher US)
                                    
                                    
                                       US
                                    
                                    
                                       USA
                                    
                                    
                                       USA
                                    
                                 
                                 
                                    
                                       Uruguay
                                    
                                    
                                       Uruguay
                                    
                                    
                                       UY
                                    
                                    
                                       URY
                                    
                                    
                                       ROU
                                    
                                 
                                 
                                    
                                       Uzbekistan
                                    
                                    
                                       Usbekistan
                                    
                                    
                                       UZ
                                    
                                    
                                       UZB
                                    
                                    
                                       UZ
                                    
                                 
                                 
                                    
                                       Vanuatu
                                    
                                    
                                       Vanuatu
                                    
                                    
                                       VU
                                    
                                    
                                       VUT
                                    
                                    
                                       VAN
                                    
                                 
                                 
                                    
                                       Venezuela (Bolivarian Republic of)
                                    
                                    
                                       Venezuela
                                    
                                    
                                       VE
                                    
                                    
                                       VEN
                                    
                                    
                                       YV
                                    
                                 
                                 
                                    
                                       Viet Nam
                                    
                                    
                                       Vietnam
                                    
                                    
                                       VN
                                    
                                    
                                       VNM
                                    
                                    
                                       VN
                                    
                                 
                                 
                                    
                                       Virgin Islands, US
                                    
                                    
                                       Amerikanische Jungferninseln
                                    
                                    
                                       VI
                                    
                                    
                                       VIR
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Wallis and Futuna Islands
                                    
                                    
                                       Wallis und Futuna
                                    
                                    
                                       WF
                                    
                                    
                                       WLF
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Western Sahara
                                    
                                    
                                       Westsahara
                                    
                                    
                                       EH
                                    
                                    
                                       ESH
                                    
                                    
                                        
                                    
                                 
                                 
                                    
                                       Yemen
                                    
                                    
                                       Jemen
                                    
                                    
                                       YE
                                    
                                    
                                       YEM
                                    
                                    
                                       YEM
                                    
                                 
                                 
                                    
                                       Zambia
                                    
                                    
                                       Sambia
                                    
                                    
                                       ZM
                                    
                                    
                                       ZMB
                                    
                                    
                                       Z
                                    
                                 
                                 
                                    
                                       Zimbabwe
                                    
                                    
                                       Simbabwe (früher RSR)
                                    
                                    
                                       ZW
                                    
                                    
                                       ZWE
                                    
                                    
                                       ZW
                                    
                                 
                                 
                                    
                                       
                                    
                                    
                                       verschiedene Zielländer
                                    
                                    
                                       -
                                    
                                    
                                       -
                                    
                                    
                                       ZZA
                                    
                                 
                                 
                                    
                                       
                                    
                                    
                                       nicht aufgeführtes Land
                                    
                                    
                                       -
                                    
                                    
                                       -
                                    
                                    
                                       ZZZ
                                    
                                 
                              
                           
                        
                        
                        
                     
                  
                  
                     
                        
                           
                              
                                 
                                    
                                       Country
                                    
                                    
                                       Land
                                    
                                    
                                       ISO 3166 ALPHA-2
                                    
                                    
                                       ISO 3166 ALPHA-3
                                    
                                    
                                       DAT-Kodierung
                                    
                                 
                                 
                                    
                                       Afghanistan
                                    
                                    
                                       Afghanistan
                                    
                                    
                                       AF
                                    
                                    
                                       AFG
                                    
                                    
                                       AFG
                                    
                                 
                                 
                                    
                                       Aland Islands
                                    
                                    
                                       Åland
                                    
                                    
                                       AX
                                    
                                    
                                       ALA
                                    
                                    
                                       AX
                                    
                                 
                                 
                                    
                                       Albania
                                    
                                    
                                       Albanien
                                    
                                    
                                       AL
                                    
                                    
                                       ALB
                                    
                                    
                                       AL
                                    
                                 
                                 
                                    
                                       Algeria
                                    
                                    
                                       Algerien
                                    
                                    
                                       DZ
                                    
                                    
                                       DZA
                                    
                                    
                                       DZ
                                    
                                 
                                 
                                    
                                       American Samoa
                                    
                                    
                                       Amerikanisch-Samoa
                                    
                                    
                                       AS
                                    
                                    
                                       ASM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Andorra
                                    
                                    
                                       Andorra
                                    
                                    
                                       AD
                                    
                                    
                                       AND
                                    
                                    
                                       AND
                                    
                                 
                                 
                                    
                                       Angola
                                    
                                    
                                       Angola
                                    
                                    
                                       AO
                                    
                                    
                                       AGO
                                    
                                    
                                       ANG
                                    
                                 
                                 
                                    
                                       Anguilla
                                    
                                    
                                       Anguilla
                                    
                                    
                                       AI
                                    
                                    
                                       AIA
                                    
                                    
                                       AXA
                                    
                                 
                                 
                                    
                                       Antarctica
                                    
                                    
                                       Antarktika
                                    
                                    
                                       AQ
                                    
                                    
                                       ATA
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Antigua and Barbuda
                                    
                                    
                                       Antigua und Barbuda
                                    
                                    
                                       AG
                                    
                                    
                                       ATG
                                    
                                    
                                       AG
                                    
                                 
                                 
                                    
                                       Argentina
                                    
                                    
                                       Argentinien
                                    
                                    
                                       AR
                                    
                                    
                                       ARG
                                    
                                    
                                       RA
                                    
                                 
                                 
                                    
                                       Armenia
                                    
                                    
                                       Armenien
                                    
                                    
                                       AM
                                    
                                    
                                       ARM
                                    
                                    
                                       ARM
                                    
                                 
                                 
                                    
                                       Aruba
                                    
                                    
                                       Aruba
                                    
                                    
                                       AW
                                    
                                    
                                       ABW
                                    
                                    
                                       ARU
                                    
                                 
                                 
                                    
                                       Australia
                                    
                                    
                                       Australien
                                    
                                    
                                       AU
                                    
                                    
                                       AUS
                                    
                                    
                                       AUS
                                    
                                 
                                 
                                    
                                       Austria
                                    
                                    
                                       Österreich
                                    
                                    
                                       AT
                                    
                                    
                                       AUT
                                    
                                    
                                       A
                                    
                                 
                                 
                                    
                                       Azerbaijan
                                    
                                    
                                       Aserbaidschan
                                    
                                    
                                       AZ
                                    
                                    
                                       AZE
                                    
                                    
                                       AZ
                                    
                                 
                                 
                                    
                                       Bahamas
                                    
                                    
                                       Bahamas
                                    
                                    
                                       BS
                                    
                                    
                                       BHS
                                    
                                    
                                       BS
                                    
                                 
                                 
                                    
                                       Bahrain
                                    
                                    
                                       Bahrain
                                    
                                    
                                       BH
                                    
                                    
                                       BHR
                                    
                                    
                                       BRN
                                    
                                 
                                 
                                    
                                       Bangladesh
                                    
                                    
                                       Bangladesch
                                    
                                    
                                       BD
                                    
                                    
                                       BGD
                                    
                                    
                                       BD
                                    
                                 
                                 
                                    
                                       Barbados
                                    
                                    
                                       Barbados
                                    
                                    
                                       BB
                                    
                                    
                                       BRB
                                    
                                    
                                       BDS
                                    
                                 
                                 
                                    
                                       Belarus
                                    
                                    
                                       Belarus (Weißrussland)
                                    
                                    
                                       BY
                                    
                                    
                                       BLR
                                    
                                    
                                       BY
                                    
                                 
                                 
                                    
                                       Belgium
                                    
                                    
                                       Belgien
                                    
                                    
                                       BE
                                    
                                    
                                       BEL
                                    
                                    
                                       B
                                    
                                 
                                 
                                    
                                       Belize
                                    
                                    
                                       Belize
                                    
                                    
                                       BZ
                                    
                                    
                                       BLZ
                                    
                                    
                                       BZ
                                    
                                 
                                 
                                    
                                       Benin
                                    
                                    
                                       Benin
                                    
                                    
                                       BJ
                                    
                                    
                                       BEN
                                    
                                    
                                       BJ
                                    
                                 
                                 
                                    
                                       Bermuda
                                    
                                    
                                       Bermuda
                                    
                                    
                                       BM
                                    
                                    
                                       BMU
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Bhutan
                                    
                                    
                                       Bhutan
                                    
                                    
                                       BT
                                    
                                    
                                       BTN
                                    
                                    
                                       BHT
                                    
                                 
                                 
                                    
                                       Bolivia
                                    
                                    
                                       Bolivien
                                    
                                    
                                       BO
                                    
                                    
                                       BOL
                                    
                                    
                                       BOL
                                    
                                 
                                 
                                    
                                       Bosnia and Herzegovina
                                    
                                    
                                       Bosnien und Herzegowina
                                    
                                    
                                       BA
                                    
                                    
                                       BIH
                                    
                                    
                                       BIH
                                    
                                 
                                 
                                    
                                       Botswana
                                    
                                    
                                       Botswana
                                    
                                    
                                       BW
                                    
                                    
                                       BWA
                                    
                                    
                                       RB
                                    
                                 
                                 
                                    
                                       Bouvet Island
                                    
                                    
                                       Bouvetinsel
                                    
                                    
                                       BV
                                    
                                    
                                       BVT
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Brazil
                                    
                                    
                                       Brasilien
                                    
                                    
                                       BR
                                    
                                    
                                       BRA
                                    
                                    
                                       BR
                                    
                                 
                                 
                                    
                                       British Indian Ocean Territory
                                    
                                    
                                       Britisches Territorium im Indischen Ozean
                                    
                                    
                                       IO
                                    
                                    
                                       IOT
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       British Virgin Islands
                                    
                                    
                                       Britische Jungferninseln
                                    
                                    
                                       VG
                                    
                                    
                                       VGB
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Brunei Darussalam
                                    
                                    
                                       Brunei Darussalam
                                    
                                    
                                       BN
                                    
                                    
                                       BRN
                                    
                                    
                                       BRU
                                    
                                 
                                 
                                    
                                       Bulgaria
                                    
                                    
                                       Bulgarien
                                    
                                    
                                       BG
                                    
                                    
                                       BGR
                                    
                                    
                                       BG
                                    
                                 
                                 
                                    
                                       Burkina Faso
                                    
                                    
                                       Burkina Faso
                                    
                                    
                                       BF
                                    
                                    
                                       BFA
                                    
                                    
                                       BF
                                    
                                 
                                 
                                    
                                       Burundi
                                    
                                    
                                       Burundi
                                    
                                    
                                       BI
                                    
                                    
                                       BDI
                                    
                                    
                                       RU
                                    
                                 
                                 
                                    
                                       Cambodia
                                    
                                    
                                       Kambodscha
                                    
                                    
                                       KH
                                    
                                    
                                       KHM
                                    
                                    
                                       K
                                    
                                 
                                 
                                    
                                       Cameroon
                                    
                                    
                                       Kamerun
                                    
                                    
                                       CM
                                    
                                    
                                       CMR
                                    
                                    
                                       CAM
                                    
                                 
                                 
                                    
                                       Canada
                                    
                                    
                                       Kanada
                                    
                                    
                                       CA
                                    
                                    
                                       CAN
                                    
                                    
                                       CDN
                                    
                                 
                                 
                                    
                                       Cape Verde
                                    
                                    
                                       Kap Verde
                                    
                                    
                                       CV
                                    
                                    
                                       CPV
                                    
                                    
                                       CV
                                    
                                 
                                 
                                    
                                       Cayman Islands
                                    
                                    
                                       Kaimaninseln
                                    
                                    
                                       KY
                                    
                                    
                                       CYM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Central African Republic
                                    
                                    
                                       Zentralafrikanische Republik
                                    
                                    
                                       CF
                                    
                                    
                                       CAF
                                    
                                    
                                       RCA
                                    
                                 
                                 
                                    
                                       Chad
                                    
                                    
                                       Tschad
                                    
                                    
                                       TD
                                    
                                    
                                       TCD
                                    
                                    
                                       TD
                                    
                                 
                                 
                                    
                                       Chile
                                    
                                    
                                       Chile
                                    
                                    
                                       CL
                                    
                                    
                                       CHL
                                    
                                    
                                       RCH
                                    
                                 
                                 
                                    
                                       China
                                    
                                    
                                       China, Volksrepublik
                                    
                                    
                                       CN
                                    
                                    
                                       CHN
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Christmas Island
                                    
                                    
                                       Weihnachtsinsel
                                    
                                    
                                       CX
                                    
                                    
                                       CXR
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Cocos (Keeling) Islands
                                    
                                    
                                       Kokosinseln
                                    
                                    
                                       CC
                                    
                                    
                                       CCK
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Colombia
                                    
                                    
                                       Kolumbien
                                    
                                    
                                       CO
                                    
                                    
                                       COL
                                    
                                    
                                       CO
                                    
                                 
                                 
                                    
                                       Comoros
                                    
                                    
                                       Komoren
                                    
                                    
                                       KM
                                    
                                    
                                       COM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Congo (Brazzaville)
                                    
                                    
                                       Republik Kongo
                                    
                                    
                                       CG
                                    
                                    
                                       COG
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Congo, Democratic Republic of the
                                    
                                    
                                       Kongo, Demokratische Republik (ehem. Zaire)
                                    
                                    
                                       CD
                                    
                                    
                                       COD
                                    
                                    
                                       CGO
                                    
                                 
                                 
                                    
                                       Cook Islands
                                    
                                    
                                       Cookinseln
                                    
                                    
                                       CK
                                    
                                    
                                       COK
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Costa Rica
                                    
                                    
                                       Costa Rica
                                    
                                    
                                       CR
                                    
                                    
                                       CRI
                                    
                                    
                                       CR
                                    
                                 
                                 
                                    
                                       Côte d'Ivoire
                                    
                                    
                                       Côte d’Ivoire (Elfenbeinküste)
                                    
                                    
                                       CI
                                    
                                    
                                       CIV
                                    
                                    
                                       CI
                                    
                                 
                                 
                                    
                                       Croatia
                                    
                                    
                                       Kroatien
                                    
                                    
                                       HR
                                    
                                    
                                       HRV
                                    
                                    
                                       HR
                                    
                                 
                                 
                                    
                                       Cuba
                                    
                                    
                                       Kuba
                                    
                                    
                                       CU
                                    
                                    
                                       CUB
                                    
                                    
                                       C
                                    
                                 
                                 
                                    
                                       Cyprus
                                    
                                    
                                       Zypern
                                    
                                    
                                       CY
                                    
                                    
                                       CYP
                                    
                                    
                                       CY
                                    
                                 
                                 
                                    
                                       Czech Republic
                                    
                                    
                                       Tschechische Republik
                                    
                                    
                                       CZ
                                    
                                    
                                       CZE
                                    
                                    
                                       CZ
                                    
                                 
                                 
                                    
                                       Denmark
                                    
                                    
                                       Dänemark
                                    
                                    
                                       DK
                                    
                                    
                                       DNK
                                    
                                    
                                       DK
                                    
                                 
                                 
                                    
                                       Djibouti
                                    
                                    
                                       Dschibuti
                                    
                                    
                                       DJ
                                    
                                    
                                       DJI
                                    
                                    
                                       DJI
                                    
                                 
                                 
                                    
                                       Dominica
                                    
                                    
                                       Dominica
                                    
                                    
                                       DM
                                    
                                    
                                       DMA
                                    
                                    
                                       WD
                                    
                                 
                                 
                                    
                                       Dominican Republic
                                    
                                    
                                       Dominikanische Republik
                                    
                                    
                                       DO
                                    
                                    
                                       DOM
                                    
                                    
                                       DOM
                                    
                                 
                                 
                                    
                                       Ecuador
                                    
                                    
                                       Ecuador
                                    
                                    
                                       EC
                                    
                                    
                                       ECU
                                    
                                    
                                       EC
                                    
                                 
                                 
                                    
                                       Egypt
                                    
                                    
                                       Ägypten
                                    
                                    
                                       EG
                                    
                                    
                                       EGY
                                    
                                    
                                       ET
                                    
                                 
                                 
                                    
                                       El Salvador
                                    
                                    
                                       El Salvador
                                    
                                    
                                       SV
                                    
                                    
                                       SLV
                                    
                                    
                                       ES
                                    
                                 
                                 
                                    
                                       Equatorial Guinea
                                    
                                    
                                       Äquatorialguinea
                                    
                                    
                                       GQ
                                    
                                    
                                       GNQ
                                    
                                    
                                       GQ
                                    
                                 
                                 
                                    
                                       Eritrea
                                    
                                    
                                       Eritrea
                                    
                                    
                                       ER
                                    
                                    
                                       ERI
                                    
                                    
                                       ER 
                                    
                                 
                                 
                                    
                                       Estonia
                                    
                                    
                                       Estland
                                    
                                    
                                       EE
                                    
                                    
                                       EST
                                    
                                    
                                       EST
                                    
                                 
                                 
                                    
                                       Ethiopia
                                    
                                    
                                       Äthiopien
                                    
                                    
                                       ET
                                    
                                    
                                       ETH
                                    
                                    
                                       ETH
                                    
                                 
                                 
                                    
                                       Falkland Islands (Malvinas)
                                    
                                    
                                       Falklandinseln
                                    
                                    
                                       FK
                                    
                                    
                                       FLK
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Faroe Islands
                                    
                                    
                                       Färöer
                                    
                                    
                                       FO
                                    
                                    
                                       FRO
                                    
                                    
                                       FO
                                    
                                 
                                 
                                    
                                       Fiji
                                    
                                    
                                       Fidschi
                                    
                                    
                                       FJ
                                    
                                    
                                       FJI
                                    
                                    
                                       FJI
                                    
                                 
                                 
                                    
                                       Finland
                                    
                                    
                                       Finnland (früher SF)
                                    
                                    
                                       FI
                                    
                                    
                                       FIN
                                    
                                    
                                       FIN
                                    
                                 
                                 
                                    
                                       France
                                    
                                    
                                       Frankreich
                                    
                                    
                                       FR
                                    
                                    
                                       FRA
                                    
                                    
                                       F
                                    
                                 
                                 
                                    
                                       French Guiana
                                    
                                    
                                       Französisch-Guayana
                                    
                                    
                                       GF
                                    
                                    
                                       GUF
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       French Polynesia
                                    
                                    
                                       Französisch-Polynesien
                                    
                                    
                                       PF
                                    
                                    
                                       PYF
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       French Southern Territories
                                    
                                    
                                       Französische Süd- und Antarktisgebiete
                                    
                                    
                                       TF
                                    
                                    
                                       ATF
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Gabon
                                    
                                    
                                       Gabun
                                    
                                    
                                       GA
                                    
                                    
                                       GAB
                                    
                                    
                                       G
                                    
                                 
                                 
                                    
                                       Gambia
                                    
                                    
                                       Gambia
                                    
                                    
                                       GM
                                    
                                    
                                       GMB
                                    
                                    
                                       WAG
                                    
                                 
                                 
                                    
                                       Georgia
                                    
                                    
                                       Georgien
                                    
                                    
                                       GE
                                    
                                    
                                       GEO
                                    
                                    
                                       GE
                                    
                                 
                                 
                                    
                                       Germany
                                    
                                    
                                       Deutschland
                                    
                                    
                                       DE
                                    
                                    
                                       DEU
                                    
                                    
                                       D
                                    
                                 
                                 
                                    
                                       Ghana
                                    
                                    
                                       Ghana
                                    
                                    
                                       GH
                                    
                                    
                                       GHA
                                    
                                    
                                       GH
                                    
                                 
                                 
                                    
                                       Gibraltar
                                    
                                    
                                       Gibraltar
                                    
                                    
                                       GI
                                    
                                    
                                       GIB
                                    
                                    
                                       GBZ
                                    
                                 
                                 
                                    
                                       Greece
                                    
                                    
                                       Griechenland
                                    
                                    
                                       GR
                                    
                                    
                                       GRC
                                    
                                    
                                       GR
                                    
                                 
                                 
                                    
                                       Greenland
                                    
                                    
                                       Grönland
                                    
                                    
                                       GL
                                    
                                    
                                       GRL
                                    
                                    
                                       KN
                                    
                                 
                                 
                                    
                                       Grenada
                                    
                                    
                                       Grenada
                                    
                                    
                                       GD
                                    
                                    
                                       GRD
                                    
                                    
                                       WG
                                    
                                 
                                 
                                    
                                       Guadeloupe
                                    
                                    
                                       Guadeloupe
                                    
                                    
                                       GP
                                    
                                    
                                       GLP
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Guam
                                    
                                    
                                       Guam
                                    
                                    
                                       GU
                                    
                                    
                                       GUM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Guatemala
                                    
                                    
                                       Guatemala
                                    
                                    
                                       GT
                                    
                                    
                                       GTM
                                    
                                    
                                       GCA
                                    
                                 
                                 
                                    
                                       Guernsey
                                    
                                    
                                       Guernsey (Kanalinsel)
                                    
                                    
                                       GG
                                    
                                    
                                       GGY
                                    
                                    
                                       GBG
                                    
                                 
                                 
                                    
                                       Guinea
                                    
                                    
                                       Guinea
                                    
                                    
                                       GN
                                    
                                    
                                       GIN
                                    
                                    
                                       RG
                                    
                                 
                                 
                                    
                                       Guinea-Bissau
                                    
                                    
                                       Guinea-Bissau
                                    
                                    
                                       GW
                                    
                                    
                                       GNB
                                    
                                    
                                       GUB
                                    
                                 
                                 
                                    
                                       Guyana
                                    
                                    
                                       Guyana
                                    
                                    
                                       GY
                                    
                                    
                                       GUY
                                    
                                    
                                       GUY
                                    
                                 
                                 
                                    
                                       Haiti
                                    
                                    
                                       Haiti
                                    
                                    
                                       HT
                                    
                                    
                                       HTI
                                    
                                    
                                       RH
                                    
                                 
                                 
                                    
                                       Heard Island and Mcdonald Islands
                                    
                                    
                                       Heard und McDonaldinseln
                                    
                                    
                                       HM
                                    
                                    
                                       HMD
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Holy See (Vatican City State)
                                    
                                    
                                       Vatikanstadt
                                    
                                    
                                       VA
                                    
                                    
                                       VAT
                                    
                                    
                                       V
                                    
                                 
                                 
                                    
                                       Honduras
                                    
                                    
                                       Honduras
                                    
                                    
                                       HN
                                    
                                    
                                       HND
                                    
                                    
                                       HN
                                    
                                 
                                 
                                    
                                       Hong Kong, Special Administrative Region of China
                                    
                                    
                                       Hongkong
                                    
                                    
                                       HK
                                    
                                    
                                       HKG
                                    
                                    
                                       HK
                                    
                                 
                                 
                                    
                                       Hungary
                                    
                                    
                                       Ungarn
                                    
                                    
                                       HU
                                    
                                    
                                       HUN
                                    
                                    
                                       H
                                    
                                 
                                 
                                    
                                       Iceland
                                    
                                    
                                       Island
                                    
                                    
                                       IS
                                    
                                    
                                       ISL
                                    
                                    
                                       IS
                                    
                                 
                                 
                                    
                                       India
                                    
                                    
                                       Indien
                                    
                                    
                                       IN
                                    
                                    
                                       IND
                                    
                                    
                                       IND
                                    
                                 
                                 
                                    
                                       Indonesia
                                    
                                    
                                       Indonesien
                                    
                                    
                                       ID
                                    
                                    
                                       IDN
                                    
                                    
                                       RI
                                    
                                 
                                 
                                    
                                       Iran, Islamic Republic of
                                    
                                    
                                       Iran, Islamische Republik
                                    
                                    
                                       IR
                                    
                                    
                                       IRN
                                    
                                    
                                       IR
                                    
                                 
                                 
                                    
                                       Iraq
                                    
                                    
                                       Irak
                                    
                                    
                                       IQ
                                    
                                    
                                       IRQ
                                    
                                    
                                       IRQ
                                    
                                 
                                 
                                    
                                       Ireland
                                    
                                    
                                       Irland
                                    
                                    
                                       IE
                                    
                                    
                                       IRL
                                    
                                    
                                       IRL
                                    
                                 
                                 
                                    
                                       Isle of Man
                                    
                                    
                                       Insel Man
                                    
                                    
                                       IM
                                    
                                    
                                       IMN
                                    
                                    
                                       GBM
                                    
                                 
                                 
                                    
                                       Israel
                                    
                                    
                                       Israel
                                    
                                    
                                       IL
                                    
                                    
                                       ISR
                                    
                                    
                                       IL
                                    
                                 
                                 
                                    
                                       Italy
                                    
                                    
                                       Italien
                                    
                                    
                                       IT
                                    
                                    
                                       ITA
                                    
                                    
                                       I
                                    
                                 
                                 
                                    
                                       Jamaica
                                    
                                    
                                       Jamaika
                                    
                                    
                                       JM
                                    
                                    
                                       JAM
                                    
                                    
                                       JA
                                    
                                 
                                 
                                    
                                       Japan
                                    
                                    
                                       Japan
                                    
                                    
                                       JP
                                    
                                    
                                       JPN
                                    
                                    
                                       J
                                    
                                 
                                 
                                    
                                       Jersey
                                    
                                    
                                       Jersey (Kanalinsel)
                                    
                                    
                                       JE
                                    
                                    
                                       JEY
                                    
                                    
                                       GBJ
                                    
                                 
                                 
                                    
                                       Jordan
                                    
                                    
                                       Jordanien
                                    
                                    
                                       JO
                                    
                                    
                                       JOR
                                    
                                    
                                       JOR
                                    
                                 
                                 
                                    
                                       Kazakhstan
                                    
                                    
                                       Kasachstan
                                    
                                    
                                       KZ
                                    
                                    
                                       KAZ
                                    
                                    
                                       KZ
                                    
                                 
                                 
                                    
                                       Kenya
                                    
                                    
                                       Kenia
                                    
                                    
                                       KE
                                    
                                    
                                       KEN
                                    
                                    
                                       EAK
                                    
                                 
                                 
                                    
                                       Kiribati
                                    
                                    
                                       Kiribati
                                    
                                    
                                       KI
                                    
                                    
                                       KIR
                                    
                                    
                                       KIR
                                    
                                 
                                 
                                    
                                       Korea, Democratic People's Republic of
                                    
                                    
                                       Korea, Demokratische Volksrepublik (Nordkorea)
                                    
                                    
                                       KP
                                    
                                    
                                       PRK
                                    
                                    
                                       KP
                                    
                                 
                                 
                                    
                                       Korea, Republic of
                                    
                                    
                                       Korea, Republik (Südkorea)
                                    
                                    
                                       KR
                                    
                                    
                                       KOR
                                    
                                    
                                       ROK
                                    
                                 
                                 
                                    
                                       Kuwait
                                    
                                    
                                       Kuwait
                                    
                                    
                                       KW
                                    
                                    
                                       KWT
                                    
                                    
                                       KWT
                                    
                                 
                                 
                                    
                                       Kyrgyzstan
                                    
                                    
                                       Kirgisistan
                                    
                                    
                                       KG
                                    
                                    
                                       KGZ
                                    
                                    
                                       KS
                                    
                                 
                                 
                                    
                                       Lao PDR
                                    
                                    
                                       Laos, Demokratische Volksrepublik
                                    
                                    
                                       LA
                                    
                                    
                                       LAO
                                    
                                    
                                       LAO
                                    
                                 
                                 
                                    
                                       Latvia
                                    
                                    
                                       Lettland
                                    
                                    
                                       LV
                                    
                                    
                                       LVA
                                    
                                    
                                       LV
                                    
                                 
                                 
                                    
                                       Lebanon
                                    
                                    
                                       Libanon
                                    
                                    
                                       LB
                                    
                                    
                                       LBN
                                    
                                    
                                       RL
                                    
                                 
                                 
                                    
                                       Lesotho
                                    
                                    
                                       Lesotho
                                    
                                    
                                       LS
                                    
                                    
                                       LSO
                                    
                                    
                                       LS
                                    
                                 
                                 
                                    
                                       Liberia
                                    
                                    
                                       Liberia
                                    
                                    
                                       LR
                                    
                                    
                                       LBR
                                    
                                    
                                       LB
                                    
                                 
                                 
                                    
                                       Libya
                                    
                                    
                                       Libyen
                                    
                                    
                                       LY
                                    
                                    
                                       LBY
                                    
                                    
                                       LAR
                                    
                                 
                                 
                                    
                                       Liechtenstein
                                    
                                    
                                       Liechtenstein
                                    
                                    
                                       LI
                                    
                                    
                                       LIE
                                    
                                    
                                       FL
                                    
                                 
                                 
                                    
                                       Lithuania
                                    
                                    
                                       Litauen
                                    
                                    
                                       LT
                                    
                                    
                                       LTU
                                    
                                    
                                       LT
                                    
                                 
                                 
                                    
                                       Luxembourg
                                    
                                    
                                       Luxemburg
                                    
                                    
                                       LU
                                    
                                    
                                       LUX
                                    
                                    
                                       L
                                    
                                 
                                 
                                    
                                       Macao, Special Administrative Region of China
                                    
                                    
                                       Macau
                                    
                                    
                                       MO
                                    
                                    
                                       MAC
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Macedonia, Republic of
                                    
                                    
                                       Mazedonien
                                    
                                    
                                       MK
                                    
                                    
                                       MKD
                                    
                                    
                                       MK
                                    
                                 
                                 
                                    
                                       Madagascar
                                    
                                    
                                       Madagaskar
                                    
                                    
                                       MG
                                    
                                    
                                       MDG
                                    
                                    
                                       RM
                                    
                                 
                                 
                                    
                                       Malawi
                                    
                                    
                                       Malawi
                                    
                                    
                                       MW
                                    
                                    
                                       MWI
                                    
                                    
                                       MW
                                    
                                 
                                 
                                    
                                       Malaysia
                                    
                                    
                                       Malaysia
                                    
                                    
                                       MY
                                    
                                    
                                       MYS
                                    
                                    
                                       MAL
                                    
                                 
                                 
                                    
                                       Maldives
                                    
                                    
                                       Malediven
                                    
                                    
                                       MV
                                    
                                    
                                       MDV
                                    
                                    
                                       MV
                                    
                                 
                                 
                                    
                                       Mali
                                    
                                    
                                       Mali
                                    
                                    
                                       ML
                                    
                                    
                                       MLI
                                    
                                    
                                       RMM
                                    
                                 
                                 
                                    
                                       Malta
                                    
                                    
                                       Malta
                                    
                                    
                                       MT
                                    
                                    
                                       MLT
                                    
                                    
                                       M
                                    
                                 
                                 
                                    
                                       Marshall Islands
                                    
                                    
                                       Marshallinseln
                                    
                                    
                                       MH
                                    
                                    
                                       MHL
                                    
                                    
                                       MH
                                    
                                 
                                 
                                    
                                       Martinique
                                    
                                    
                                       Martinique
                                    
                                    
                                       MQ
                                    
                                    
                                       MTQ
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Mauritania
                                    
                                    
                                       Mauretanien
                                    
                                    
                                       MR
                                    
                                    
                                       MRT
                                    
                                    
                                       RIM
                                    
                                 
                                 
                                    
                                       Mauritius
                                    
                                    
                                       Mauritius
                                    
                                    
                                       MU
                                    
                                    
                                       MUS
                                    
                                    
                                       MS
                                    
                                 
                                 
                                    
                                       Mayotte
                                    
                                    
                                       Namibia
                                    
                                    
                                       NA
                                    
                                    
                                       NAM
                                    
                                    
                                       NAM
                                    
                                 
                                 
                                    
                                       Mexico
                                    
                                    
                                       Mexiko
                                    
                                    
                                       MX
                                    
                                    
                                       MEX
                                    
                                    
                                       MEX
                                    
                                 
                                 
                                    
                                       Micronesia, Federated States of
                                    
                                    
                                       Mikronesien
                                    
                                    
                                       FM
                                    
                                    
                                       FSM
                                    
                                    
                                       FSM
                                    
                                 
                                 
                                    
                                       Moldova
                                    
                                    
                                       Moldawien (Republik Moldau)
                                    
                                    
                                       MD
                                    
                                    
                                       MDA
                                    
                                    
                                       MD
                                    
                                 
                                 
                                    
                                       Monaco
                                    
                                    
                                       Monaco
                                    
                                    
                                       MC
                                    
                                    
                                       MCO
                                    
                                    
                                       MC
                                    
                                 
                                 
                                    
                                       Mongolia
                                    
                                    
                                       Mongolei
                                    
                                    
                                       MN
                                    
                                    
                                       MNG
                                    
                                    
                                       MGL
                                    
                                 
                                 
                                    
                                       Montenegro
                                    
                                    
                                       Montenegro
                                    
                                    
                                       ME
                                    
                                    
                                       MNE
                                    
                                    
                                       MNE
                                    
                                 
                                 
                                    
                                       Montserrat
                                    
                                    
                                       Montserrat
                                    
                                    
                                       MS
                                    
                                    
                                       MSR
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Morocco
                                    
                                    
                                       Marokko
                                    
                                    
                                       MA
                                    
                                    
                                       MAR
                                    
                                    
                                       MA
                                    
                                 
                                 
                                    
                                       Mozambique
                                    
                                    
                                       Mosambik
                                    
                                    
                                       MZ
                                    
                                    
                                       MOZ
                                    
                                    
                                       MOC
                                    
                                 
                                 
                                    
                                       Myanmar
                                    
                                    
                                       Myanmar (Burma)
                                    
                                    
                                       MM
                                    
                                    
                                       MMR
                                    
                                    
                                       Mya
                                    
                                 
                                 
                                    
                                       Namibia
                                    
                                    
                                       Neukaledonien
                                    
                                    
                                       NC
                                    
                                    
                                       NCL
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Nauru
                                    
                                    
                                       Neutrale Zone (Saudi-Arabien und Irak bis 1993)
                                    
                                    
                                       NT
                                    
                                    
                                       NTZ
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Nepal
                                    
                                    
                                       Nauru
                                    
                                    
                                       NR
                                    
                                    
                                       NRU
                                    
                                    
                                       NAU
                                    
                                 
                                 
                                    
                                       Norway
                                    
                                    
                                       Norwegen
                                    
                                    
                                       NO
                                    
                                    
                                       NOR
                                    
                                    
                                       N
                                    
                                 
                                 
                                    
                                       Netherlands Antilles
                                    
                                    
                                       Niederländische Antillen (historisch)
                                    
                                    
                                       AN
                                    
                                    
                                       ANT
                                    
                                    
                                       NA
                                    
                                 
                                 
                                    
                                       New Caledonia
                                    
                                    
                                       Niger
                                    
                                    
                                       NE
                                    
                                    
                                       NER
                                    
                                    
                                       RN
                                    
                                 
                                 
                                    
                                       New Zealand
                                    
                                    
                                       Neuseeland
                                    
                                    
                                       NZ
                                    
                                    
                                       NZL
                                    
                                    
                                       NZ
                                    
                                 
                                 
                                    
                                       Nicaragua
                                    
                                    
                                       Niue
                                    
                                    
                                       NU
                                    
                                    
                                       NIU
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Niger
                                    
                                    
                                       Norfolkinsel
                                    
                                    
                                       NF
                                    
                                    
                                       NFK
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Nigeria
                                    
                                    
                                       Nicaragua
                                    
                                    
                                       NI
                                    
                                    
                                       NIC
                                    
                                    
                                       Nic
                                    
                                 
                                 
                                    
                                       Niue
                                    
                                    
                                       Niederlande
                                    
                                    
                                       NL
                                    
                                    
                                       NLD
                                    
                                    
                                       NL
                                    
                                 
                                 
                                    
                                       Norfolk Island
                                    
                                    
                                       Nigeria
                                    
                                    
                                       NG
                                    
                                    
                                       NGA
                                    
                                    
                                       NGR
                                    
                                 
                                 
                                    
                                       Northern Mariana Islands
                                    
                                    
                                       Nördliche Marianen
                                    
                                    
                                       MP
                                    
                                    
                                       MNP
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Norway
                                    
                                    
                                       Nepal
                                    
                                    
                                       NP
                                    
                                    
                                       NPL
                                    
                                    
                                       NEP
                                    
                                 
                                 
                                    
                                       Oman
                                    
                                    
                                       Oman
                                    
                                    
                                       OM
                                    
                                    
                                       OMN
                                    
                                    
                                       OM
                                    
                                 
                                 
                                    
                                       Pakistan
                                    
                                    
                                       Pakistan
                                    
                                    
                                       PK
                                    
                                    
                                       PAK
                                    
                                    
                                       PK
                                    
                                 
                                 
                                    
                                       Palau
                                    
                                    
                                       Palau
                                    
                                    
                                       PW
                                    
                                    
                                       PLW
                                    
                                    
                                       PAL
                                    
                                 
                                 
                                    
                                       Palestinian Territory, Occupied
                                    
                                    
                                       Palästina
                                    
                                    
                                       PS
                                    
                                    
                                       PSE
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Panama
                                    
                                    
                                       Panama
                                    
                                    
                                       PA
                                    
                                    
                                       PAN
                                    
                                    
                                       PA
                                    
                                 
                                 
                                    
                                       Papua New Guinea
                                    
                                    
                                       Papua-Neuguinea
                                    
                                    
                                       PG
                                    
                                    
                                       PNG
                                    
                                    
                                       PNG
                                    
                                 
                                 
                                    
                                       Paraguay
                                    
                                    
                                       Paraguay
                                    
                                    
                                       PY
                                    
                                    
                                       PRY
                                    
                                    
                                       PY
                                    
                                 
                                 
                                    
                                       Peru
                                    
                                    
                                       Peru
                                    
                                    
                                       PE
                                    
                                    
                                       PER
                                    
                                    
                                       PE
                                    
                                 
                                 
                                    
                                       Philippines
                                    
                                    
                                       Philippinen
                                    
                                    
                                       PH
                                    
                                    
                                       PHL
                                    
                                    
                                       RP
                                    
                                 
                                 
                                    
                                       Pitcairn
                                    
                                    
                                       Pitcairninseln
                                    
                                    
                                       PN
                                    
                                    
                                       PCN
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Poland
                                    
                                    
                                       Polen
                                    
                                    
                                       PL
                                    
                                    
                                       POL
                                    
                                    
                                       PL
                                    
                                 
                                 
                                    
                                       Portugal
                                    
                                    
                                       Portugal
                                    
                                    
                                       PT
                                    
                                    
                                       PRT
                                    
                                    
                                       P
                                    
                                 
                                 
                                    
                                       Puerto Rico
                                    
                                    
                                       Puerto Rico
                                    
                                    
                                       PR
                                    
                                    
                                       PRI
                                    
                                    
                                       PRI
                                    
                                 
                                 
                                    
                                       Qatar
                                    
                                    
                                       Katar
                                    
                                    
                                       QA
                                    
                                    
                                       QAT
                                    
                                    
                                       Q
                                    
                                 
                                 
                                    
                                       Réunion
                                    
                                    
                                       Réunion
                                    
                                    
                                       RE
                                    
                                    
                                       REU
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Romania
                                    
                                    
                                       Rumänien
                                    
                                    
                                       RO
                                    
                                    
                                       ROU
                                    
                                    
                                       RO
                                    
                                 
                                 
                                    
                                       Russian Federation
                                    
                                    
                                       Russische Föderation
                                    
                                    
                                       RU
                                    
                                    
                                       RUS
                                    
                                    
                                       RUS
                                    
                                 
                                 
                                    
                                       Rwanda
                                    
                                    
                                       Ruanda
                                    
                                    
                                       RW
                                    
                                    
                                       RWA
                                    
                                    
                                       RWA
                                    
                                 
                                 
                                    
                                       Saint Helena
                                    
                                    
                                       St. Helena
                                    
                                    
                                       SH
                                    
                                    
                                       SHN
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Saint Kitts and Nevis
                                    
                                    
                                       St. Kitts und Nevis
                                    
                                    
                                       KN
                                    
                                    
                                       KNA
                                    
                                    
                                       KANN
                                    
                                 
                                 
                                    
                                       Saint Lucia
                                    
                                    
                                       St. Lucia
                                    
                                    
                                       LC
                                    
                                    
                                       LCA
                                    
                                    
                                       WL
                                    
                                 
                                 
                                    
                                       Saint Pierre and Miquelon
                                    
                                    
                                       Saint-Pierre und Miquelon
                                    
                                    
                                       PM
                                    
                                    
                                       SPM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Saint Vincent and Grenadines
                                    
                                    
                                       St. Vincent und die Grenadinen
                                    
                                    
                                       VC
                                    
                                    
                                       VCT
                                    
                                    
                                       WV
                                    
                                 
                                 
                                    
                                       Saint-Barthélemy
                                    
                                    
                                       Saint-Barthélemy
                                    
                                    
                                       BL
                                    
                                    
                                       BLM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Saint-Martin (French part)
                                    
                                    
                                       Saint-Martin (franz. Teil)
                                    
                                    
                                       MF
                                    
                                    
                                       MAF
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Samoa
                                    
                                    
                                       Samoa
                                    
                                    
                                       WS
                                    
                                    
                                       WSM
                                    
                                    
                                       WS
                                    
                                 
                                 
                                    
                                       San Marino
                                    
                                    
                                       San Marino
                                    
                                    
                                       SM
                                    
                                    
                                       SMR
                                    
                                    
                                       RSM
                                    
                                 
                                 
                                    
                                       Sao Tome and Principe
                                    
                                    
                                       Sao Tome u. Principe
                                    
                                    
                                       ST
                                    
                                    
                                       STP
                                    
                                    
                                       STP
                                    
                                 
                                 
                                    
                                       Saudi Arabia
                                    
                                    
                                       Saudi-Arabien
                                    
                                    
                                       SA
                                    
                                    
                                       SAU
                                    
                                    
                                       KSA
                                    
                                 
                                 
                                    
                                       Senegal
                                    
                                    
                                       Senegal
                                    
                                    
                                       SN
                                    
                                    
                                       SEN
                                    
                                    
                                       SN
                                    
                                 
                                 
                                    
                                       Serbia
                                    
                                    
                                       Serbien
                                    
                                    
                                       RS
                                    
                                    
                                       SRB
                                    
                                    
                                       SRB
                                    
                                 
                                 
                                    
                                       Seychelles
                                    
                                    
                                       Seychellen
                                    
                                    
                                       SC
                                    
                                    
                                       SYC
                                    
                                    
                                       SY
                                    
                                 
                                 
                                    
                                       Sierra Leone
                                    
                                    
                                       Sierra Leone
                                    
                                    
                                       SL
                                    
                                    
                                       SLE
                                    
                                    
                                       WAL
                                    
                                 
                                 
                                    
                                       Singapore
                                    
                                    
                                       Singapur
                                    
                                    
                                       SG
                                    
                                    
                                       SGP
                                    
                                    
                                       SGP
                                    
                                 
                                 
                                    
                                       Slovakia
                                    
                                    
                                       Slowakei
                                    
                                    
                                       SK
                                    
                                    
                                       SVK
                                    
                                    
                                       SK
                                    
                                 
                                 
                                    
                                       Slovenia
                                    
                                    
                                       Slowenien
                                    
                                    
                                       SI
                                    
                                    
                                       SVN
                                    
                                    
                                       SLO
                                    
                                 
                                 
                                    
                                       Solomon Islands
                                    
                                    
                                       Salomonen
                                    
                                    
                                       SB
                                    
                                    
                                       SLB
                                    
                                    
                                       SOL
                                    
                                 
                                 
                                    
                                       Somalia
                                    
                                    
                                       Somalia
                                    
                                    
                                       SO
                                    
                                    
                                       SOM
                                    
                                    
                                       SO
                                    
                                 
                                 
                                    
                                       South Africa
                                    
                                    
                                       Südafrika (früher SAU)
                                    
                                    
                                       ZA
                                    
                                    
                                       ZAF
                                    
                                    
                                       ZA
                                    
                                 
                                 
                                    
                                       South Georgia and the South Sandwich Islands
                                    
                                    
                                       Südgeorgien und die Südlichen Sandwichinseln
                                    
                                    
                                       GS
                                    
                                    
                                       SGS
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       South Sudan
                                    
                                    
                                       Südsudan
                                    
                                    
                                       SS
                                    
                                    
                                       SSD
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Spain
                                    
                                    
                                       Spanien
                                    
                                    
                                       ES
                                    
                                    
                                       ESP
                                    
                                    
                                       E
                                    
                                 
                                 
                                    
                                       Sri Lanka
                                    
                                    
                                       Sri Lanka
                                    
                                    
                                       LK
                                    
                                    
                                       LKA
                                    
                                    
                                       CL
                                    
                                 
                                 
                                    
                                       Sudan
                                    
                                    
                                       Sudan
                                    
                                    
                                       SD
                                    
                                    
                                       SDN
                                    
                                    
                                       SUD
                                    
                                 
                                 
                                    
                                       Suriname *
                                    
                                    
                                       Suriname
                                    
                                    
                                       SR
                                    
                                    
                                       SUR
                                    
                                    
                                       SME
                                    
                                 
                                 
                                    
                                       Svalbard and Jan Mayen Islands
                                    
                                    
                                       Svalbard und Jan Mayen
                                    
                                    
                                       SJ
                                    
                                    
                                       SJM
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Swaziland
                                    
                                    
                                       Swasiland
                                    
                                    
                                       SZ
                                    
                                    
                                       SWZ
                                    
                                    
                                       SD
                                    
                                 
                                 
                                    
                                       Sweden
                                    
                                    
                                       Schweden
                                    
                                    
                                       SE
                                    
                                    
                                       SWE
                                    
                                    
                                       S
                                    
                                 
                                 
                                    
                                       Switzerland
                                    
                                    
                                       Schweiz (Confoederatio Helvetica)
                                    
                                    
                                       CH
                                    
                                    
                                       CHE
                                    
                                    
                                       CH
                                    
                                 
                                 
                                    
                                       Syrian Arab Republic (Syria)
                                    
                                    
                                       Syrien, Arabische Republik
                                    
                                    
                                       SY
                                    
                                    
                                       SYR
                                    
                                    
                                       SYR
                                    
                                 
                                 
                                    
                                       Taiwan, Republic of China
                                    
                                    
                                       Republik China (Taiwan)
                                    
                                    
                                       TW
                                    
                                    
                                       TWN
                                    
                                    
                                       RC
                                    
                                 
                                 
                                    
                                       Tajikistan
                                    
                                    
                                       Tadschikistan
                                    
                                    
                                       TJ
                                    
                                    
                                       TJK
                                    
                                    
                                       TJ
                                    
                                 
                                 
                                    
                                       Tanzania *, United Republic of
                                    
                                    
                                       Tansania, Vereinigte Republik
                                    
                                    
                                       TZ
                                    
                                    
                                       TZA
                                    
                                    
                                       EAT
                                    
                                 
                                 
                                    
                                       Thailand
                                    
                                    
                                       Thailand
                                    
                                    
                                       TH
                                    
                                    
                                       THA
                                    
                                    
                                       T
                                    
                                 
                                 
                                    
                                       Timor-Leste
                                    
                                    
                                       Osttimor (Timor-Leste)
                                    
                                    
                                       TL
                                    
                                    
                                       TLS
                                    
                                    
                                       TL
                                    
                                 
                                 
                                    
                                       Togo
                                    
                                    
                                       Togo
                                    
                                    
                                       TG
                                    
                                    
                                       TGO
                                    
                                    
                                       TG
                                    
                                 
                                 
                                    
                                       Tokelau
                                    
                                    
                                       Tokelau
                                    
                                    
                                       TK
                                    
                                    
                                       TKL
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Tonga
                                    
                                    
                                       Tonga
                                    
                                    
                                       TO
                                    
                                    
                                       TON
                                    
                                    
                                       TON
                                    
                                 
                                 
                                    
                                       Trinidad and Tobago
                                    
                                    
                                       Trinidad und Tobago
                                    
                                    
                                       TT
                                    
                                    
                                       TTO
                                    
                                    
                                       TT
                                    
                                 
                                 
                                    
                                       Tunisia
                                    
                                    
                                       Tunesien
                                    
                                    
                                       TN
                                    
                                    
                                       TUN
                                    
                                    
                                       TN
                                    
                                 
                                 
                                    
                                       Turkey
                                    
                                    
                                       Türkei
                                    
                                    
                                       TR
                                    
                                    
                                       TUR
                                    
                                    
                                       TR
                                    
                                 
                                 
                                    
                                       Turkmenistan
                                    
                                    
                                       Turkmenistan
                                    
                                    
                                       TM
                                    
                                    
                                       TKM
                                    
                                    
                                       TM
                                    
                                 
                                 
                                    
                                       Turks and Caicos Islands
                                    
                                    
                                       Turks- und Caicosinseln
                                    
                                    
                                       TC
                                    
                                    
                                       TCA
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Tuvalu
                                    
                                    
                                       Tuvalu
                                    
                                    
                                       TV
                                    
                                    
                                       TUV
                                    
                                    
                                       TUV
                                    
                                 
                                 
                                    
                                       Uganda
                                    
                                    
                                       Uganda
                                    
                                    
                                       UG
                                    
                                    
                                       UGA
                                    
                                    
                                       EAU
                                    
                                 
                                 
                                    
                                       Ukraine
                                    
                                    
                                       Ukraine
                                    
                                    
                                       UA
                                    
                                    
                                       UKR
                                    
                                    
                                       UA
                                    
                                 
                                 
                                    
                                       United Arab Emirates
                                    
                                    
                                       Vereinigte Arabische Emirate
                                    
                                    
                                       AE
                                    
                                    
                                       ARE
                                    
                                    
                                       UAE
                                    
                                 
                                 
                                    
                                       United Kingdom
                                    
                                    
                                       Vereinigtes Königreich Großbritannien und Nordirland
                                    
                                    
                                       GB (und UK[1])
                                    
                                    
                                       GBR
                                    
                                    
                                       GB
                                    
                                 
                                 
                                    
                                       United States Minor Outlying Islands
                                    
                                    
                                       United States Minor Outlying Islands
                                    
                                    
                                       UM
                                    
                                    
                                       UMI
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       United States of America
                                    
                                    
                                       USA (früher US)
                                    
                                    
                                       US
                                    
                                    
                                       USA
                                    
                                    
                                       USA
                                    
                                 
                                 
                                    
                                       Uruguay
                                    
                                    
                                       Uruguay
                                    
                                    
                                       UY
                                    
                                    
                                       URY
                                    
                                    
                                       ROU
                                    
                                 
                                 
                                    
                                       Uzbekistan
                                    
                                    
                                       Usbekistan
                                    
                                    
                                       UZ
                                    
                                    
                                       UZB
                                    
                                    
                                       UZ
                                    
                                 
                                 
                                    
                                       Vanuatu
                                    
                                    
                                       Vanuatu
                                    
                                    
                                       VU
                                    
                                    
                                       VUT
                                    
                                    
                                       VAN
                                    
                                 
                                 
                                    
                                       Venezuela (Bolivarian Republic of)
                                    
                                    
                                       Venezuela
                                    
                                    
                                       VE
                                    
                                    
                                       VEN
                                    
                                    
                                       YV
                                    
                                 
                                 
                                    
                                       Viet Nam
                                    
                                    
                                       Vietnam
                                    
                                    
                                       VN
                                    
                                    
                                       VNM
                                    
                                    
                                       VN
                                    
                                 
                                 
                                    
                                       Virgin Islands, US
                                    
                                    
                                       Amerikanische Jungferninseln
                                    
                                    
                                       VI
                                    
                                    
                                       VIR
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Wallis and Futuna Islands
                                    
                                    
                                       Wallis und Futuna
                                    
                                    
                                       WF
                                    
                                    
                                       WLF
                                    
                                    
                                       -
                                    
                                 
                                 
                                    
                                       Western Sahara
                                    
                                    
                                       Westsahara
                                    
                                    
                                       EH
                                    
                                    
                                       ESH
                                    
                                    
                                        
                                    
                                 
                                 
                                    
                                       Yemen
                                    
                                    
                                       Jemen
                                    
                                    
                                       YE
                                    
                                    
                                       YEM
                                    
                                    
                                       YEM
                                    
                                 
                                 
                                    
                                       Zambia
                                    
                                    
                                       Sambia
                                    
                                    
                                       ZM
                                    
                                    
                                       ZMB
                                    
                                    
                                       Z
                                    
                                 
                                 
                                    
                                       Zimbabwe
                                    
                                    
                                       Simbabwe (früher RSR)
                                    
                                    
                                       ZW
                                    
                                    
                                       ZWE
                                    
                                    
                                       ZW
                                    
                                 
                                 
                                    
                                       
                                    
                                    
                                       verschiedene Zielländer
                                    
                                    
                                       -
                                    
                                    
                                       -
                                    
                                    
                                       ZZA
                                    
                                 
                                 
                                    
                                       
                                    
                                    
                                       nicht aufgeführtes Land
                                    
                                    
                                       -
                                    
                                    
                                       -
                                    
                                    
                                       ZZZ
                                    
                                 
                              
                           
                        
                        
                        
                     
                  
               
               
                  
               
            
            
               
                  Format
               
               
                  String
               
               
                  Ausgabe-Dateiformat.Aktuell nur PDF möglich.
               
               
                  PDF
               
               
                  X
               
            
            
               
                  ExportProduct
               
               
                  String
               
               
                  productName (Pflicht)priceTypeindicationOfValueoriginalPricewithEquipmentListequipmentInProtocoloriginalPriceInProtocolwithBodiesbodiesInProtocol
               
               
                  siehe nachfolgend
               
               
                  X
               
            
            
               
                  ExportProductAddOns
               
               
                  String
               
               
                  Nur SilverDAT 3 valuateExpert/valuateExpertPlusPartner:product (Pflicht)withEquipmentReportwithValueDecreasewithValueIncreasewithRepairCostwithValueIncreaseDetailswithRepairCostsDetailsvalueIndicationtaxvalueprintOption
               
               
                  siehe nachfolgend  ExportProductAddOns
               
               
                  
               
            
            
               
                  ExportCertificateAddOns
               
               
                  String
               
               
                  Nur SilverDAT 3 valuateExpert/valuateExpertPlusPartner:
                  additionalSheetattachmentDescriptioncertificateBackgroundcommentsdescriptionnrOfAttachmentstotalPagesePrint
               
               
                  siehe Urkundenausdrucke
                  
                     
                        Der Parameter ExportCertificateAddOns kann zusätzlich genutzt werden zu ExportProduct und ExportProductAddOns. Die CertificateId wird nur ausgegeben, wenn ExportCertificateAddOns mit korrekten Werten belegt worden ist. Den Parameter CertificateId benötigen Sie für die Methode getCertificate.
                        Parameter vxs:ExportCertificateAddOns mit folgende Attributen
                        
                           
                              
                                 
                                    
                                       Attribut
                                    
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                 
                                 
                                    
                                       additionalSheet
                                    
                                    
                                       true, false
                                    
                                    
                                       Mit dieser Option aktivieren Sie den zusätzlichen Druck. Diese Seite beinhaltet die
                                          Hinweise für den Auftraggeber. Kann nur gesetzt werden, wenn newVersion auf true gesetzt ist.
                                    
                                 
                                 
                                    
                                       ePrint
                                    
                                    
                                       true, false
                                    
                                    
                                       Mit dieser Option aktivieren Sie den Druck mit Hintergrund. Dies benötigen Sie, falls
                                          die entsprechende Vorlage (Druckerpapier) für die Urkunde nicht verfügbar ist und
                                          auf normalem Papier gedruckt werden soll.
                                    
                                 
                                 
                                    
                                       attachmentDescription
                                    
                                    
                                       String
                                    
                                    
                                       Anhangbeschreibung
                                    
                                 
                                 
                                    
                                       comments
                                    
                                    
                                       String
                                    
                                    
                                       Kommentar
                                    
                                 
                                 
                                    
                                       description
                                    
                                    
                                       String
                                    
                                    
                                       Beschreibung
                                    
                                 
                                 
                                    
                                       certificateBackground
                                    
                                    
                                       String
                                    
                                    
                                       noch nicht verfügbar
                                    
                                 
                                 
                                    
                                       nrOfAttachments
                                    
                                    
                                       String
                                    
                                    
                                       noch nicht verfügbar
                                    
                                 
                                 
                                    
                                       totalPages
                                    
                                    
                                       String
                                    
                                    
                                       noch nicht verfügbar
                                    
                                 
                              
                           
                        
                        
                     
                  
               
               
                  
               
            
         
      
   
   
   Übersicht der möglichen Attribute und deren Werte für das ExportProduct-Element
   
      
         
            
               
                  Attribut
               
               
                  Wert
               
               
                  Beschreibung
               
               
                  Default
               
               
                  anwendbar mit Produkt
               
            
            
               
                  priceType
               
               
                  purchase
               
               
                  Preisangabe als Einkaufspreis
               
               
                  X
               
               
                  GebrauchtfahrzeugbewertungStichtagsbewertungRestwertprognoseGebrauchtfahrzeugRestwertprognose Neufahrzeug
               
            
            
               
                  sales
               
               
                  Preisangabe als Verkaufspreis
               
               
                  
               
            
            
               
                  purchaseAndSales
               
               
                  Preisangabe als Verkaufspreis und Einkaufspreis 
               
               
                  
               
               
                  BewertungsgutachtenSchätzurkundeGrundüberprüfungLeasingrückgabe
               
            
            
               
                  indicationOfValue
               
               
                  gross
               
               
                  Wertangaben in brutto
               
               
                  X
               
               
                  GebrauchtfahrzeugbewertungStichtagsbewertungRestwertprognoseGebrauchtfahrzeugRestwertprognose Neufahrzeug
               
            
            
               
                  net
               
               
                  Wertangaben in netto
               
               
                  
               
            
            
               
                  productVariant
               
               
                  historic
               
               
                  Stichtagsbezogene Bewertung
               
               
                  
               
               
                  Stichtagsbewertung
               
            
            
               
                  originalPrice
               
               
                  true, false
               
               
                  mit Listenneupreis
               
               
                  
               
               
                  GebrauchtfahrzeugbewertungStichtagsbewertung
               
            
            
               
                  withEquipmentList
               
               
                  true, false
               
               
                  mit Ausstattungsliste
               
               
                  
               
               
                  GebrauchtfahrzeugbewertungStichtagsbewertung
               
            
            
               
                  withBodies
               
               
                  true, false
               
               
                  mit Aufbauten
               
               
                  X
               
               
                  Gebrauchtfahrzeugbewertung
               
            
            
               
                  equipmentInProtocol
               
               
                  true, false
               
               
                  mit Ausstattungsliste
               
               
                  
               
               
                  Protokoll Gebrauchtfahrzeugbewertung
               
            
            
               
                  originalPriceInProtocol 
               
               
                  true, false
               
               
                  mit Listenneupreis
               
               
                  
               
               
                  Protokoll Gebrauchtfahrzeugbewertung
               
            
            
               
                  bodiesInProtocol
               
               
                  true, false
               
               
                  inklusive Aufbauten
               
               
                  
               
               
                  Protokoll Gebrauchtfahrzeugbewertung
               
            
         
      
   
   
   Übersicht der möglichen Attribute und deren Werte für das ExportProductAddOns-Element
   Bitte auf den jeweiligen Ausdruck klicken, damit mehr Informationen zu sehen sind.
   
      
         Protokoll
         
            
               Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
               Parameter vxs:ExportProduct mit folgenden Attributen
               
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Vorbedingung
                           
                        
                        
                           
                              productName
                           
                           
                              ProtocolForExpert 
                           
                           
                              Protokoll
                           
                           
                              X
                           
                        
                     
                  
               
               Parameter vxs:ExportProductAddOns mit folgenden Attributen
               
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Vorbedingung
                           
                        
                        
                           
                              product
                           
                           
                              VALUATION,
                              BASECHECK,
                              LEASING_RETURN,
                              CONDITION_REPORT,
                              ESTIMATION_CERTIFICATE
                              VALUATION_EXPERTISE
                           
                           
                              für alle Produkte verfügbar. Auswahl des Produkts.
                           
                           
                              
                           
                        
                        
                           
                              withEquipmentReport
                           
                           
                              true, false
                           
                           
                              Ausstattungsbericht
                           
                           
                              Ausstattungen müssen in der Ausstattungsmaske oder mit createDossier gesetzt werden.
                           
                        
                        
                           
                              withValueDecrease
                           
                           
                              true, false
                           
                           
                              Wertminderung
                           
                           
                              Die Daten müssen auf der Zustandsmaske oder mit setConditionDetails gesetzt werden
                           
                        
                        
                           
                              withValueIncrease
                           
                           
                              true, false
                           
                           
                              Werterhöhung
                           
                           
                              Die Daten müssen auf der Zustandsmaske oder mit setConditionDetails gesetzt werden
                           
                        
                        
                           
                              withRepairCosts
                           
                           
                              true, false
                           
                           
                              Reparaturkosten
                           
                           
                              Die Daten müssen auf der Zustandsmaske oder mit setConditionDetails gesetzt werden
                           
                        
                        
                           
                              withValueIncreaseDetails
                           
                           
                              true, false
                           
                           
                              Werterhöhungsdetails
                           
                           
                              Das Attribut withValueIncrease muss auf true gesetzt sein
                           
                        
                        
                           
                              withRepairCostsDetails
                           
                           
                              true, false
                           
                           
                              Reparaturkostendetails
                           
                           
                              Das Attribut withRepairCosts muss auf true gesetzt sein
                           
                        
                        
                           
                              withTruckBodies
                           
                           
                              true, false
                           
                           
                              LKW- Aufbauten
                           
                        
                        
                           
                              value
                              
                           
                           
                              DAT
                           
                           
                              gemäß DAT
                           
                           
                              
                           
                        
                        
                           
                              EXPERT
                           
                           
                              gemäß Festlegung der Sachverständiger
                           
                           
                              Geben Sie mit setValueDefinition den Sachverständiger Wert an.
                           
                        
                        
                           
                              printOption
                              
                           
                           
                              PREVIEW
                           
                           
                              Vorschau (kostenloser Ausdruck), Probedruck
                           
                           
                              
                           
                        
                        
                           
                              ACTUALPRINT
                           
                           
                              Kostenpflichtiger Echtdruck
                           
                           
                              
                           
                        
                     
                  
               
               
               Request exportDossierN Protokoll
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct productName="ProtocolForExpert " />
         <ExportProductAddOns printOption="ACTUALPRINT" />
         <ExportCertificateAddOns ePrint="true" />
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

               
            
         
      
      
         Gebrauchtwagenbewertung
         
            
               Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
               Gebrauchtwagenbewertungsausdruck
               Parameter vxs:ExportProduct mit folgenden Attributen
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Pflicht
                           
                        
                        
                           
                              productName
                           
                           
                              UsedVehicleEvaluationForValuateExpert
                           
                           
                              Gebrauchtwagenbewertung
                           
                           
                              X
                           
                        
                     
                  
               
               Parameter vxs:ExportProductAddOns mit folgenden Attributen
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Bedingung
                           
                        
                        
                           
                              product
                           
                           
                              VALUATION
                           
                           
                              Wertermittlung
                           
                           
                              
                           
                        
                        
                           
                              valueIndication
                              
                           
                           
                              ValuesDealerProcurementPrice
                           
                           
                              Einkaufspreis
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ValuesDealerSalesPrice
                           
                           
                              Verkaufspreis
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ValuesDealerProcurementPriceAndDealerSalesPrice
                           
                           
                              Einkaufspreis und Verkaufspreis
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ReplacementValue
                           
                           
                              Wiederbeschaffungswert
                           
                           
                              
                           
                        
                        
                           
                              ActualCashValue
                           
                           
                              Zeitwert
                           
                           
                              
                           
                        
                        
                           
                              ValueAccordingToMarket
                           
                           
                              Marktwert
                           
                           
                              
                           
                        
                        
                           
                              tax
                              
                           
                           
                              DIFFERENCE
                           
                           
                              Differenzbesteuert (inkl. Anteil MwSt)
                           
                           
                              Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                           
                        
                        
                           
                              DIFFERENCE_TAX_AVG_VAT
                           
                           
                              Differenzbesteuert (durchschnittlicher Anteil MwSt.)
                           
                           
                              Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                           
                        
                        
                           
                              PRIVATE
                           
                           
                              Privatmarkt (MwSt neutral)
                           
                           
                              Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist. 
                           
                        
                        
                           
                              RULE
                           
                           
                              Besteuerungsart: Regelbesteuerung
                           
                           
                              
                           
                        
                        
                           
                              value
                              
                           
                           
                              DAT
                           
                           
                              gemäß DAT
                           
                           
                              
                           
                        
                        
                           
                              EXPERT
                           
                           
                              gemäß Festlegung der Sachverständiger
                           
                           
                              Geben Sie mit setValueDefinition den Sachverständiger Wert an.
                           
                        
                        
                           
                              printOption
                              
                           
                           
                              PREVIEW
                           
                           
                              Vorschau (kostenloser Ausdruck)
                           
                           
                              
                           
                        
                        
                           
                              ACTUALPRINT
                           
                           
                              Kostenpflichtiger Echtdruck
                           
                           
                              
                           
                        
                     
                  
               
               
               Request exportDossierN Gebrauchtwagenbewertung 
               
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>123456789</DossierId>
         <Locale country="DE" datCountryIndicator="DE" language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="UsedVehicleEvaluationForValuateExpert"/>
         <!--Optional:-->
         <ExportProductAddOns printOption="ACTUALPRINT" product="VALUATION" tax="DIFFERENCE" value="DAT" valueIndication="ReplacementValue"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

            
         
      
      
         Checkliste Sonderausstattungen
         
            
               Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
               Parameter vxs:ExportProduct mit folgenden Attributen
               
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Vorbedingung
                           
                        
                        
                           
                              productName
                           
                           
                              OptionalEquipmentChecklist
                           
                           
                              Checkliste Sonderausstattungen
                           
                           
                              X
                           
                        
                     
                  
               
               Parameter vxs:ExportProductAddOns mit folgenden Attributen
               
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Vorbedingung
                           
                        
                        
                           
                              product
                           
                           
                              VALUATION,
                              BASECHECK,
                              LEASING_RETURN,
                              CONDITION_REPORT,
                              ESTIMATION_CERTIFICATE
                              VALUATION_EXPERTISE
                           
                           
                              für alle Produkte verfügbar. Auswahl des Produkts.
                           
                           
                              
                           
                        
                        
                           
                              printOption
                              
                           
                           
                              PREVIEW
                           
                           
                              Vorschau (kostenloser Ausdruck), Probedruck
                           
                           
                              
                           
                        
                        
                           
                              ACTUALPRINT
                           
                           
                              Kostenpflichtiger Echtdruck
                           
                           
                              
                           
                        
                     
                  
               
               
               Request exportDossierN Checkliste Sonderausstattungen
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale country="DE" datCountryIndicator="de" language="de_DE"/>
         <Format>pdf</Format>
         <ExportProduct productName="OptionalEquipmentChecklist"/>
         <ExportProductAddOns printOption="ACTUALPRINT" product="VALUATION"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

               
            
         
      
      
         Fahrzeugdaten
         
            
               Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
               Parameter vxs:ExportProduct mit folgenden Attributen
               
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Vorbedingung
                           
                        
                        
                           
                              productName
                           
                           
                              VehicleData
                           
                           
                              Fahrzeugdaten
                           
                           
                              X
                           
                        
                     
                  
               
               Parameter vxs:ExportProductAddOns mit folgenden Attributen
               
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Vorbedingung
                           
                        
                        
                           
                              product
                           
                           
                              VALUATION,
                              BASECHECK,
                              LEASING_RETURN,
                              CONDITION_REPORT,
                              ESTIMATION_CERTIFICATE
                              VALUATION_EXPERTISE
                           
                           
                              für alle Produkte verfügbar. Auswahl des Produkts.
                           
                           
                              
                           
                        
                        
                           
                              printOption
                              
                           
                           
                              PREVIEW
                           
                           
                              Vorschau (kostenloser Ausdruck), Probedruck
                           
                           
                              
                           
                        
                        
                           
                              ACTUALPRINT
                           
                           
                              Kostenpflichtiger Echtdruck
                           
                           
                              
                           
                        
                     
                  
               
               
               Request exportDossierN Fahrzeugdaten
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale country="DE" datCountryIndicator="DE" language="de"/>
         <Format>pdf</Format>
         <ExportProduct productName="VehicleData" productVariant="overwrite"/>
         <ExportProductAddOns printOption="ACTUALPRINT" product="VALUATION"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

               
            
         
      
      
         Grundüberprüfung
         
            
               Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
               Grundüberprüfungsausdruck
               Bitte beachten Sie beim Erstellen der Ausdrucke für die Grundüberprüfung, dass immer
                  zuerst die neue Urkunde productName="BaseCheckReportNew" ausgedruckt wird. 
               Alle eventuell benötigten weiteren Seiten müssen mittels eines zweiten Aufrufs der
                  Funktion exportDossierN erzeugt werden, wobei hier die Option productName="BaseCheckReport" zu verwenden ist. 
               Parameter vxs:ExportProduct mit folgenden Attributen
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Pflicht
                           
                        
                        
                           
                              productName
                              
                           
                           
                              BaseCheckReportNew
                           
                           
                              Urkunde der Grundüberprüfung
                           
                           
                              X
                              
                           
                        
                        
                           
                              BaseCheckReport
                           
                           
                              Anhang der Grundüberprüfung
                           
                        
                     
                  
               
               Parameter vxs:ExportProductAddOns mit folgenden Attributen
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Bedingung
                           
                        
                        
                           
                              product
                           
                           
                              BASECHECK
                           
                           
                              Grundüberprüfung
                           
                           
                              Geben Sie mit setProductCheckDetailsList die Grundüberprüfungsinformation an.
                           
                        
                        
                           
                              layout
                              
                           
                           
                              ListLayoutWithoutPictures
                           
                           
                              Layout ohne Bilder
                           
                           
                              
                           
                        
                        
                           
                              ListLayoutWithPictures
                           
                           
                              Layout mit Bildern
                           
                           
                              
                           
                        
                        
                           
                              ExtendedLayout
                           
                           
                              Erweitertes Layout
                           
                           
                              
                           
                        
                        
                           
                              SpecialLayout
                           
                           
                              Speziallayout
                           
                           
                              
                           
                        
                        
                           
                              valueIndication
                              
                           
                           
                              WithoutValue
                           
                           
                              Keine Presiangaben
                           
                           
                              
                           
                        
                        
                           
                              ValuesDealerProcurementPrice
                           
                           
                              Einkaufspreis
                           
                           
                              Geben Sie mit setBaseCheckValueDefinition den Sachverständiger Wert an und setzen Sie den Attribut value auf EXPERT.
                           
                        
                        
                           
                              ValuesDealerSalesPrice
                           
                           
                              Verkaufspreis
                           
                           
                              Geben Sie mit setBaseCheckValueDefinition den Sachverständiger Wert an und setzen Sie den Attribut value auf EXPERT.
                           
                        
                        
                           
                              ValuesDealerProcurementPriceAndDealerSalesPrice
                           
                           
                              Einkaufspreis und Verkaufspreis
                           
                           
                              Geben Sie mit setBaseCheckValueDefinition den Sachverständiger Wert an und setzen Sie den Attribut value auf EXPERT.
                           
                        
                        
                           
                              value
                              
                           
                           
                              DAT
                           
                           
                              gemäß DAT
                           
                           
                              
                           
                        
                        
                           
                              EXPERT
                           
                           
                              gemäß Festlegung der Sachverständiger
                           
                           
                              
                           
                        
                        
                           
                              printOption
                              
                           
                           
                              PREVIEW
                           
                           
                              Vorschau (kostenloser Ausdruck)
                           
                           
                              
                           
                        
                        
                           
                              ACTUALPRINT
                           
                           
                              Kostenpflichtiger Echtdruck
                           
                           
                              
                           
                        
                        
                           
                              withConditionComments
                              
                           
                           
                              1 (true)
                           
                           
                              Ausdruck mit Anhang Fahrzeugzustandsbemerkungen
                           
                           
                              
                           
                        
                        
                           
                              0 (false)
                           
                           
                              Ausdruck ohne Anhang Fahrzeugzustandsbemerkungen
                           
                           
                              
                           
                        
                     
                  
               
               
               Request exportDossierN zum Erzeugen der Urkunde 
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="BaseCheckReportNew"/>
         <!—Beispiel: layout="Listenlayout ohne Bilder" und ohne Wertangabe, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="WithoutValue" printOption="PREVIEW" product="BASECHECK"/>
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
               
               
               Request exportDossierN zum Erzeugen der weiteren Seiten 
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="BaseCheckReport" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und ohne Wertangabe, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="WithoutValue" printOption="PREVIEW" product="BASECHECK" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

            
         
      
      
         Leasingrückgabe
         
            
               Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
               Leasingrückgabeausdruck
               Bitte beachten Sie beim Erstellen der Ausdrucke für die Leasingrückgabe, dass immer
                  zuerst die neue Urkunde productName="LeasingReturnReportNew" ausgedruckt wird. 
               Alle eventuell benötigten weiteren Seiten müssen mittels eines zweiten Aufrufs der
                  Funktion exportDossierN erzeugt werden, wobei hier die Option productName=LeasingReturnReport" zu verwenden ist. 
               Parameter vxs:ExportProduct mit folgenden Attributen
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Pflicht
                           
                        
                        
                           
                              productName
                              
                           
                           
                              LeasingReturnReportNew
                           
                           
                              Urkunde der Leasingrückgabe
                           
                           
                              X
                              
                           
                        
                        
                           
                              LeasingReturnReport
                           
                           
                              Anhang der Leasingrückgabe
                           
                        
                     
                  
               
               Parameter vxs:ExportProductAddOns mit folgenden Attributen
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Bedingung
                           
                        
                        
                           
                              product
                           
                           
                              LEASING_RETURN
                           
                           
                              Leasingrückgabe
                           
                           
                              Geben Sie mit setProductCheckDetailsList die Leasingrückgabeinformation an
                           
                        
                        
                           
                              layout
                              
                           
                           
                              ListLayoutWithoutPictures
                           
                           
                              Layout ohne Bilder
                           
                           
                              
                           
                        
                        
                           
                              ListLayoutWithPictures
                           
                           
                              Layout mit Bilder
                           
                           
                              
                           
                        
                        
                           
                              ExtendedLayout
                           
                           
                              Erweitertes Layout
                           
                           
                              
                           
                        
                        
                           
                              SpecialLayout
                           
                           
                              Speziallayout
                           
                           
                              
                           
                        
                        
                           
                              valueIndication
                              
                           
                           
                              WithoutValue
                           
                           
                              Ohne Verkaufs oder Einkaufspreis
                           
                           
                              
                           
                        
                        
                           
                              ValuesDealerProcurementPrice
                           
                           
                              Einkaufspreis
                           
                           
                              Geben Sie mit setLeasingReturnValueDefinition den Sachverständiger Wert an und setzen Sie das Attribut value auf EXPERT.
                           
                        
                        
                           
                              ValuesDealerSalesPrice
                           
                           
                              Verkaufspreis
                           
                           
                              Geben Sie mit setLeasingReturnValueDefinition den Sachverständiger Wert an und setzen Sie das Attribut value auf EXPERT.
                           
                        
                        
                           
                              ValuesDealerProcurementPriceAndDealerSalesPrice
                           
                           
                              Einkaufspreis und Verkaufspreis
                           
                           
                              Geben Sie mit setLeasingReturnValueDefinition den Sachverständiger Wert an und setzen Sie das Attribut value auf EXPERT.
                           
                        
                        
                           
                              value
                              
                           
                           
                              DAT
                           
                           
                              gemäß DAT
                           
                           
                              
                           
                        
                        
                           
                              EXPERT
                           
                           
                              gemäß Festlegung der Sachverständiger
                           
                           
                              
                           
                        
                        
                           
                              printOption
                              
                           
                           
                              PREVIEW
                           
                           
                              Vorschau (kostenloser Ausdruck)
                           
                           
                              
                           
                        
                        
                           
                              ACTUALPRINT
                           
                           
                              Kostenpflichtiger Echtdruck
                           
                           
                              
                              
                           
                        
                        
                           
                              withConditionComments
                              
                           
                           
                              1 (true)
                           
                           
                              Ausdruck mit Anhang Fahrzeugzustandsbemerkungen
                           
                           
                              
                           
                        
                        
                           
                              0 (false)
                           
                           
                              Ausdruck ohne Anhang Fahrzeugzustandsbemerkungen
                           
                           
                              
                           
                        
                     
                  
               
               
               Request exportDossierN zum Erzeugen der Urkunde
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="LeasingReturnReportNew" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und ohne Wertangabe, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="WithoutValue" printOption="PREVIEW" product="LEASING_RETURN" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

               Request exportDossierN zum Erzeugen der weiteren Seiten
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="LeasingReturnReport" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und ohne Wertangabe, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="WithoutValue" printOption="PREVIEW" product="LEASING_RETURN" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

            
         
      
      
         Zustandsbericht
         
            
               Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
               Zustandsberichtausdruck
               Bitte beachten Sie beim Erstellen der Ausdrucke für den Zustandsbericht, dass immer
                  zuerst die neue Urkunde productName="ConditionReportNew" ausgedruckt wird. 
               Alle eventuell benötigten weiteren Seiten müssen mittels eines zweiten Aufrufs der
                  Funktion exportDossierN erzeugt werden, wobei hier die Option productName="ConditionReport" zu verwenden ist. 
               Parameter vxs:ExportProduct mit folgenden Attributen
               
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Bedingung
                           
                        
                        
                           
                              productName
                              
                           
                           
                              ConditionReportNew
                           
                           
                              Urkunde des Zustandsberichts
                           
                           
                              X
                              
                           
                        
                        
                           
                              ConditionReport
                           
                           
                              Anhang des Zustandsberichts
                           
                        
                     
                  
               
               Parameter vxs:ExportProductAddOns mit folgenden Attributen
               
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Bedingung
                           
                        
                        
                           
                              product
                           
                           
                              CONDITION_REPORT
                           
                           
                              Zustandsbericht
                           
                           
                              Geben Sie mit setConditionDetails die Zustandsdetails an.
                           
                        
                        
                           
                              layout
                              
                           
                           
                              ListLayoutWithoutPictures
                           
                           
                              Layout ohne Bilder
                           
                           
                              
                           
                        
                        
                           
                              ListLayoutWithPictures
                           
                           
                              Layout mit Bilder
                           
                           
                              
                           
                        
                        
                           
                              value
                              
                           
                           
                              DAT
                           
                           
                              gemäß DAT
                           
                           
                              
                           
                        
                        
                           
                              EXPERT
                           
                           
                              gemäß Festlegung der Sachverständiger
                           
                           
                              Geben Sie mit setConditionReportValueDefinition den Sachverständiger Wert an.
                           
                        
                        
                           
                              printOption
                              
                           
                           
                              PREVIEW
                           
                           
                              Vorschau (kostenloser Ausdruck)
                           
                           
                              
                           
                        
                        
                           
                              ACTUALPRINT
                           
                           
                              Kostenpflichtiger Echtdruck
                           
                           
                              
                           
                        
                        
                           
                              withConditionComments
                              
                           
                           
                              1 (true)
                           
                           
                              Ausdruck mit Anhang Fahrzeugzustandsbemerkungen
                           
                           
                              
                           
                        
                        
                           
                              0 (false)
                           
                           
                              Ausdruck ohne Anhang Fahrzeugzustandsbemerkungen
                           
                           
                              
                           
                        
                     
                  
               
               
               Request exportDossierN zum Erzeugen der Urkunde
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="ConditionReportNew" />
         <!—Beispiel: layout="Listenlayout ohne Bilder", Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" printOption="PREVIEW" product="CONDITION_REPORT"/>
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
               Request exportDossierN zum Erzeugen der weiteren Seiten 
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="ConditionReport" />
         <!—Beispiel: layout="Listenlayout ohne Bilder", Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" printOption="PREVIEW" product="CONDITION_REPORT"/>
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
            
         
      
      
         Bewertungsgutachten
         
            
               Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
               Bewertungsgutachtenausdruck
               Bitte beachten Sie beim Erstellen der Ausdrucke für das Bewertungsgutachten, dass
                  immer zuerst die neue Urkunde productName="ValuationExpertiseNew" ausgedruckt wird. 
               Alle eventuell benötigten weiteren Seiten müssen mittels eines zweiten Aufrufs der
                  Funktion exportDossierN erzeugt werden, wobei hier die Option productName="ValuationExpertise" zu verwenden ist. 
               Parameter vxs:ExportProduct mit folgenden Attributen
               
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Pflicht
                           
                        
                        
                           
                              productName
                              
                           
                           
                              ValuationExpertiseNew
                           
                           
                              Urkunde des Bewertungsgutachtens
                           
                           
                              X
                              
                           
                        
                        
                           
                              ValuationExpertise
                           
                           
                              Anhang des Bewertungsgutachtens 
                           
                        
                     
                  
               
               Parameter vxs:ExportProductAddOns mit folgenden Attributen
               
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Bedingung
                           
                        
                        
                           
                              product
                           
                           
                              VALUATION_EXPERTISE
                           
                           
                              Bewertungsgutachten
                           
                           
                              Geben Sie mit setValuationExpertiseSpecialAssesmentsDetails die Bewertungsgutachteninformationen an.
                           
                        
                        
                           
                              valueIndication
                              
                           
                           
                              ValuesDealerProcurementPrice
                           
                           
                              Einkaufspreis
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ValuesDealerSalesPrice
                           
                           
                              Verkaufspreis
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ValuesDealerProcurementPriceAndDealerSalesPrice
                           
                           
                              Einkaufspreis und Verkaufspreis
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ReplacementValue
                           
                           
                              Wiederbeschaffungswert
                           
                           
                              
                           
                        
                        
                           
                              ActualCashValue
                           
                           
                              Zeitwert
                           
                           
                              
                           
                        
                        
                           
                              ValueAccordingToMarket
                           
                           
                              Marktwert
                           
                           
                              
                           
                        
                        
                           
                              tax
                              
                           
                           
                              DIFFERENCE
                           
                           
                              Differenzbesteuert (inkl. Anteil MwSt)
                           
                           
                              Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                           
                        
                        
                           
                              DIFFERENCE_TAX_AVG_VAT
                           
                           
                              Differenzbesteuert (durchschnittlicher Anteil MwSt.)
                           
                           
                              Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                           
                        
                        
                           
                              PRIVATE
                           
                           
                              Privatmarkt (MwSt neutral)
                           
                           
                              Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist. 
                           
                        
                        
                           
                              RULE
                           
                           
                              Besteuerungsart: Regelbesteuerung
                           
                           
                              
                           
                        
                        
                           
                              value
                              
                           
                           
                              DAT
                           
                           
                              gemäß DAT
                           
                           
                              
                           
                        
                        
                           
                              EXPERT
                           
                           
                              gemäß Festlegung der Sachverständiger
                           
                           
                              Geben Sie mit setValuationExpertiseValueDefinition den Sachverständiger Wert an.
                           
                        
                        
                           
                              printOption
                              
                           
                           
                              PREVIEW
                           
                           
                              Vorschau (kostenloser Ausdruck)
                           
                           
                              
                           
                        
                        
                           
                              ACTUALPRINT
                           
                           
                              Kostenpflichtiger Echtdruck
                           
                           
                              
                           
                        
                        
                           
                              withConditionComments
                              
                           
                           
                              1 (true)
                           
                           
                              Ausdruck mit Anhang Fahrzeugzustandsbemerkungen
                           
                           
                              
                           
                        
                        
                           
                              0 (false)
                           
                           
                              Ausdruck ohne Anhang Fahrzeugzustandsbemerkungen
                           
                           
                              
                           
                        
                     
                  
               
               
               Request exportDossierN zum Erzeugen der Urkunde 
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="ValuationExpertiseNew" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und Wiederbeschaffungswert, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="ReplacementValue" printOption="PREVIEW" product="VALUATION_EXPERTISE" value="DAT" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
               Request exportDossierN zum Erzeugen der weiteren Seiten 
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="ValuationExpertise" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und Wiederbeschaffungswert, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="ReplacementValue" printOption="PREVIEW" product="VALUATION_EXPERTISE" value="DAT" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
            
         
      
      
         Schätzurkunde
         
            
               Siehe auf Seite Parameter exportDossierN für zusätzliche Attribute für ExportProduct.
               Schätzurkundeausdruck
               Bitte beachten Sie beim Erstellen der Ausdrucke für die Schätzurkunde, dass immer
                  zuerst die neue Urkunde productName="EstimationCertificateNew" ausgedruckt wird. 
               Alle eventuell benötigten weiteren Seiten müssen mittels eines zweiten Aufrufs der
                  Funktion exportDossierN erzeugt werden, wobei hier die Option productName="EstimationCertificate" zu verwenden ist. 
               Parameter vxs:ExportProduct mit folgenden Attributen
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Bedingung
                           
                        
                        
                           
                              productName
                              
                           
                           
                              EstimationCertificateNew
                           
                           
                              Urkunde der Schätzurkunde
                           
                           
                              X
                              
                           
                        
                        
                           
                              EstimationCertificate
                           
                           
                              Anhang der Schätzurkunde
                           
                        
                     
                  
               
               Parameter vxs:ExportProductAddOns mit folgenden Attributen
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                           
                              Bedingung
                           
                        
                        
                           
                              product
                           
                           
                              ESTIMATION_CERTIFICATE
                           
                           
                              Schätzurkunde
                           
                           
                              Geben Sie mit setEstimationCertificateSpecialAssesmentsDetails die Schätzurkundeinformationen an
                           
                        
                        
                           
                              valueIndication
                              
                           
                           
                              ValuesDealerProcurementPrice
                           
                           
                              Einkaufspreis
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ValuesDealerSalesPrice
                           
                           
                              Verkaufspreis
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ValuesDealerProcurementPriceAndDealerSalesPrice
                           
                           
                              Einkaufspreis und Verkaufspreis
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ValuesDealerProcurementPrice
                           
                           
                              Wiederbeschaffungswert
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ValuesDealerSalesPrice
                           
                           
                              Zeitwert
                           
                           
                              Sie können mit setBaseCheckValueDefinition den Wert des Sachverständigen setzen und mittels des Attributs value=EXPERT diesen Wert ausgeben.
                           
                        
                        
                           
                              ValueAccordingToMarket
                           
                           
                              Marktwert
                           
                           
                              
                           
                        
                        
                           
                              tax
                              
                           
                           
                              DIFFERENCE
                           
                           
                              Differenzbesteuert (inkl. Anteil MwSt)
                           
                           
                              Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                           
                        
                        
                           
                              DIFFERENCE_TAX_AVG_VAT
                           
                           
                              Differenzbesteuert (durchschnittlicher Anteil MwSt.)
                           
                           
                              Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist und die Besteuerungsart auf Differenz gesetzt ist
                           
                        
                        
                           
                              PRIVATE
                           
                           
                              Privatmarkt (MwSt neutral)
                           
                           
                              Kann nur gesetzt werden, wenn das Attribut valueIndication auf ReplacementValue oder ValueAccordingToMarket gesetzt ist. 
                           
                        
                        
                           
                              RULE
                           
                           
                              Besteuerungsart: Regelbesteuerung
                           
                           
                              
                           
                        
                        
                           
                              value
                              
                           
                           
                              DAT
                           
                           
                              gemäß DAT
                           
                           
                              
                           
                        
                        
                           
                              EXPERT
                           
                           
                              gemäß Festlegung der Sachverständiger
                           
                           
                              
                           
                        
                        
                           
                              printOption
                              
                           
                           
                              PREVIEW
                           
                           
                              Vorschau (kostenloser Ausdruck)
                           
                           
                              
                           
                        
                        
                           
                              ACTUALPRINT
                           
                           
                              Kostenpflichtiger Echtdruck
                           
                           
                              
                           
                        
                        
                           
                              withConditionComments
                              
                           
                           
                              1 (true)
                           
                           
                              Ausdruck mit Anhang Fahrzeugzustandsbemerkungen
                           
                           
                              
                           
                        
                        
                           
                              0 (false)
                           
                           
                              Ausdruck ohne Anhang Fahrzeugzustandsbemerkungen
                           
                           
                              
                           
                        
                     
                  
               
               
               Request exportDossierN zum Erzeugen der Urkunde 
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="EstimationCertificateNew" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und Wiederbeschaffungswert, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="ReplacementValue" printOption="PREVIEW" product="ESTIMATION_CERTIFICATE" value="DAT" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
               Request exportDossierN zum Erzeugen der weiteren Seiten
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234567</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct indicationOfValue="net" priceType="purchase" productName="EstimationCertificate" />
         <!—Beispiel: layout="Listenlayout ohne Bilder" und Wiederbeschaffungswert, Probedruck -->
         <ExportProductAddOns layout="ListLayoutWithoutPictures" valueIndication="ReplacementValue" printOption="PREVIEW" product="ESTIMATION_CERTIFICATE" value="DAT" />
         <!--Optional:-->
         <ExportCertificateAddOns ePrint="true"/>
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>
            
         
      
      
         Urkunde
         
            
               Der Parameter ExportCertificateAddOns kann zusätzlich genutzt werden zu ExportProduct und ExportProductAddOns. Die CertificateId wird nur ausgegeben, wenn ExportCertificateAddOns mit korrekten Werten belegt worden ist. Den Parameter CertificateId benötigen Sie für die Methode getCertificate.
               Parameter vxs:ExportCertificateAddOns mit folgende Attributen
               
                  
                     
                        
                           
                              Attribut
                           
                           
                              Wert
                           
                           
                              Beschreibung
                           
                        
                        
                           
                              additionalSheet
                           
                           
                              true, false
                           
                           
                              Mit dieser Option aktivieren Sie den zusätzlichen Druck. Diese Seite beinhaltet die
                                 Hinweise für den Auftraggeber. Kann nur gesetzt werden, wenn newVersion auf true gesetzt ist.
                           
                        
                        
                           
                              ePrint
                           
                           
                              true, false
                           
                           
                              Mit dieser Option aktivieren Sie den Druck mit Hintergrund. Dies benötigen Sie, falls
                                 die entsprechende Vorlage (Druckerpapier) für die Urkunde nicht verfügbar ist und
                                 auf normalem Papier gedruckt werden soll.
                           
                        
                        
                           
                              attachmentDescription
                           
                           
                              String
                           
                           
                              Anhangbeschreibung
                           
                        
                        
                           
                              comments
                           
                           
                              String
                           
                           
                              Kommentar
                           
                        
                        
                           
                              description
                           
                           
                              String
                           
                           
                              Beschreibung
                           
                        
                        
                           
                              certificateBackground
                           
                           
                              String
                           
                           
                              noch nicht verfügbar
                           
                        
                        
                           
                              nrOfAttachments
                           
                           
                              String
                           
                           
                              noch nicht verfügbar
                           
                        
                        
                           
                              totalPages
                           
                           
                              String
                           
                           
                              noch nicht verfügbar
                           
                        
                     
                  
               
               
            
         
      
      
         BAFA Gutachten
         
            
               Mit Hilfe der Funktion exportDossierN erstellen Sie das Gutachten zur Förderung für gebrauchte Fahrzeuge entsprechend den
                  Vorgaben des Bundesamt für Wirtschaft und Ausfuhrkontrolle (BAFA). 
               Übersicht
               
                  
                     
                        
                           
                              Wert
                           
                           
                              Produkt Beschreibung
                           
                           
                              Format 
                           
                           
                              In folgenden Produkten enthalten
                           
                        
                        
                           
                              bafaGutachtenReport
                           
                           
                              BAFA Gutachten
                           
                           
                              PDF
                           
                           
                              SilverDAT 3 valuateExpertPlusPartner
                           
                        
                     
                  
               
               
               Überblick der Parameter und deren Attribute
               
                  
                     
                        
                           
                              Parameter
                           
                           
                              Datentyp
                           
                           
                              Beschreibung
                           
                           
                              Schreibweise
                           
                           
                              Pflicht
                           
                        
                        
                           
                              DossierId
                           
                           
                              Long
                           
                           
                              EindeutigeVorgangskennung
                           
                           
                              numerisch
                           
                           
                              X
                           
                        
                        
                           
                              Locale
                           
                           
                              Locale
                           
                           
                              Beispiel: <Locale country="DE"datCountryIndicator="DE" language="de"/>
                           
                           
                              ISO 3166 ALPHA-2:
                              country¹,datCountryIndicator¹
                           
                           
                              X
                           
                        
                        
                           
                              Format
                           
                           
                              String
                           
                           
                              Ausgabe-Dateiformat.Aktuell nur PDF möglich.
                           
                           
                              PDF
                           
                           
                              X
                           
                        
                        
                           
                              ExportProduct
                           
                           
                              String
                           
                           
                              productName (Pflicht)
                           
                           
                              bafaGutachtenReport
                           
                           
                              X
                           
                        
                        
                           
                              ExportProductAddOns
                           
                           
                              String
                           
                           
                              printOption
                           
                           
                              ACTUALPRINT=Kostenpflichtiger EchtdruckPREVIEW=Vorschau (kostenloser Ausdruck), Probedruck
                           
                           
                              
                           
                        
                        
                           
                              ExportCertificateAddOns
                           
                           
                              String
                           
                           
                              ePrint
                              Mit dieser Option aktivieren Sie den Druck mit Hintergrund. Dies benötigen Sie, falls
                                 die entsprechende Vorlage (Druckerpapier) für die Urkunde nicht verfügbar ist und
                                 auf normalen Papier gedruckt werden soll.
                           
                           
                              true=Mit Hintergrundfalse=Blanko für Vordruck
                           
                           
                              
                           
                        
                     
                  
               
               
               Request exportDossierN BAFA
               
               <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:exportDossierN>
         <DossierId>1234</DossierId>
         <Locale language="de"/>
         <Format>pdf</Format>
         <ExportProduct productName="bafaGutachtenReport" />
         <ExportProductAddOns printOption="ACTUALPRINT" />
         <ExportCertificateAddOns ePrint="true" />
      </dos:exportDossierN>
   </soapenv:Body>
</soapenv:Envelope>

               
            
         
      
   
   Mittels der Methode setOrderOpeningDetails und setConditionDetails können weitere Details zum Ausdruck hinzugefügt werden.
   ¹Siehe Popup-Fenster
