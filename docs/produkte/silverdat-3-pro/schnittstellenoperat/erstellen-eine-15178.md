---
title: "Erstellen einer neuen Bewertung in der Anwendung"
topic_id: "15178"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Erstellen einer neuen Bewertung in der Anwendung"
---

# Erstellen einer neuen Bewertung in der Anwendung

Mit der Funktion createValuationN erstellen Sie einen neuen Vorgang oder aktualisieren einen existierenden Vorgang.
      Hierbei legen Sie entweder einen neuen Auftrag an, oder Sie speichern eine neue Bewertung
      zu einem bestehenden Auftrag. In diesem Fall darf der betreffende Auftrag noch keine
      Bewertung enthalten. Einem existierenden Auftrag wird eine Bewertung hinzugefügt,
      wenn dieselbe ContractId bei Vorgängen verwendet wird.
   Um einen neuen Vorgang zu erstellen, benötigen Sie mindestens den Auftragstyp (contractType), sowie den Netzwerktyp (networkType) und das Dossier Element. Zusätzlich können Sie noch die Vorlagen ID (templateId) mit Vorlagendaten (templateData) übergeben. 
   Variante mit unvollständiger Fahrzeugidentifikation
   Die Funktion createValuationN unterstützt die Variante mit unvollständiger Fahrzeugidentifikation. Bei dieser Variante
      erstellen Sie einen neuen Vorgang in der Anwendung ohne vorher das Fahrzeug eindeutig
      zu identifizieren. 
   Voraussetzungen:
   
      
         Das Element Coverage muss gesetzt sein und den Wert NOVALUATIONRESULT oder NONE enthalten.
      
      
         Der Request darf keine oder nur eine unvollständige Fahrzeugidentifikation beinhalten.
            
      
   
   Siehe im Kapitel "Request createValuationN Variante mit unvollständiger Fahrzeugidentifikation"
   Request
   Das nachfolgende Beispiel zeigt einen Request mit den Pflichtfeldern, die im Standardfall mindestens benötigt werden. 
   Beispiel:
   
         <val:createValuationN>
         <contractType>bundle_valuation</contractType>
         <networkType>DAT</networkType>
         <vxs:Dossier>
            <vxs:Name>MyValuation</vxs:Name>
            <vxs:Country>DE</vxs:Country>
            <vxs:Language>de_DE</vxs:Language>
            <vxs:Currency>EUR</vxs:Currency>
            <vxs:Vehicle>
               <vxs:DatECode>019051080040002</vxs:DatECode>
               <vxs:Container>DE002</vxs:Container>
               <vxs:ConstructionTime>5419</vxs:ConstructionTime>
               <vxs:InitialRegistration>2015-01-01</vxs:InitialRegistration>
               <vxs:MileageEstimated>50000</vxs:MileageEstimated>
               <vxs:Country>DE</vxs:Country>
            </vxs:Vehicle>
         </vxs:Dossier>
      </val:createValuationN>

   Rückgabe
   Im Erfolgsfall wird der Vorgang als VXS zurückgegeben, andernfalls wird eine Fehlermeldung zurückgegeben. Die Beschreibung
      der Response-Elemente finden Sie im Kapitel VXS. In der Rückgabe finden Sie den Parameter DossierId den Sie nachfolgend für die weitere Funktionen benötigen. Die Identifikationsnummer
      DossierId ist identisch mit der contractID die Sie zum Beispiel in der Funktion getValuationN benötigen. Sie erkennen einen Response der Variante mit unvollständiger Fahrzeugidentifikation
      anhand des Werts incompleteValuation im Attribut type des Elements VXS.
   Parameter
   Es werden nur die nachfolgend beschriebenen Parameter unterstützt, nicht aufgeführte
      Parameter führen zu Fehlern oder werden ignoriert. 
   Aufgrund der Tatsache das ein myclaim Anwender in verschiedenen Netzen Teilhaber sein kann, wird durch das Setzen des Parameters
      networkType bestimmt in welches Netz ein Auftrag erstellt werden soll. Soll beispielsweise ein
      Auftrag in das SD3 Netz erstellt werden so bekommt der Parameter networkType den Wert DAT. Da myclaim mittlerweile eine große Anzahl an verschiedenen Netzen beinhaltet, können
      die entsprechenden Netzwerktypen falls nicht bekannt bei der DAT erfragt werden.
   Standardfall
   Request createValuationN
   
      
         
            
               
                  Name
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  contractType
               
               
                  String
               
               
                  Auftragstypen
               
               
                  bundle_valuation
               
               
                  X
               
            
            
               
                  networkType
               
               
                  String
               
               
                  Netzwerktypen
               
               
                  Konstante eines bestimmten myclaim Netzes
                   DAT für SD3
               
               
                  X
               
            
            
               
                  vxs:Dossier
               
               
                  Dossier
               
               
                  Element das die Vehicle eXchange Struktur (VXS) beinhaltet
               
               
                  
               
               
                  X
               
            
            
               
                  Coverage
                  
                     
                        Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.
                        
                        
                           
                              
                                 
                                    
                                       Wert
                                    
                                    
                                       Datenumfang
                                    
                                 
                                 
                                    
                                       MARKETPLACEEXPORT
                                    
                                    
                                       Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO).
                                    
                                 
                                 
                                    
                                       EXTENDEDBYTRADING
                                    
                                    
                                       Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO).
                                    
                                 
                                 
                                    
                                       COMPLETE
                                    
                                    
                                       Defaultwert;  Standard Datenumfang für die Datenrückgabe
                                    
                                 
                                 
                                    
                                       NOVALUATIONRESULT
                                    
                                    
                                       Datenrückgabe ohne die Unterelemente Valuation und VAT
                                    
                                 
                                 
                                    
                                       ENRICHED
                                    
                                    
                                       Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen
                                    
                                 
                                 
                                    
                                       BASE
                                    
                                    
                                       Datenrückgabe ganz ohne Benennungen
                                    
                                 
                                 
                                    
                                       SIMPLE
                                    
                                    
                                       Bei diesem Wert entfallen zusätzlich bestimmte  Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder,  RegistratinData, Engine, Equipment oder TechInfo.
                                    
                                 
                                 
                                    
                                       NONE
                                    
                                    
                                       Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. 
                                    
                                 
                              
                           
                        
                     
                  
               
               
                  String
               
               
                  Steuerung des Umfangs der Datenrückgabe
               
               
                  Coverage
                  
                     
                        Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.
                        
                        
                           
                              
                                 
                                    
                                       Wert
                                    
                                    
                                       Datenumfang
                                    
                                 
                                 
                                    
                                       MARKETPLACEEXPORT
                                    
                                    
                                       Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO).
                                    
                                 
                                 
                                    
                                       EXTENDEDBYTRADING
                                    
                                    
                                       Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO).
                                    
                                 
                                 
                                    
                                       COMPLETE
                                    
                                    
                                       Defaultwert;  Standard Datenumfang für die Datenrückgabe
                                    
                                 
                                 
                                    
                                       NOVALUATIONRESULT
                                    
                                    
                                       Datenrückgabe ohne die Unterelemente Valuation und VAT
                                    
                                 
                                 
                                    
                                       ENRICHED
                                    
                                    
                                       Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen
                                    
                                 
                                 
                                    
                                       BASE
                                    
                                    
                                       Datenrückgabe ganz ohne Benennungen
                                    
                                 
                                 
                                    
                                       SIMPLE
                                    
                                    
                                       Bei diesem Wert entfallen zusätzlich bestimmte  Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder,  RegistratinData, Engine, Equipment oder TechInfo.
                                    
                                 
                                 
                                    
                                       NONE
                                    
                                    
                                       Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. 
                                    
                                 
                              
                           
                        
                     
                  
               
               
                  
               
            
            
               
                  templateId
               
               
                  Long
               
               
                  ID der Auftragsvorlage
               
               
                  
               
               
                  
               
            
            
               
                  templateData
               
               
                  HashMap<String, Object>
               
               
                  Benutzerdefinierte Vorlagendaten
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:Dossier
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:Language
                  
                     
                        
                           
                              
                                 
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                 
                                 
                                    
                                       ca_ES
                                    
                                    
                                       Katalanisch Spanien 
                                    
                                 
                                 
                                    
                                       cs_CZ
                                    
                                    
                                       Tschechisch Tschechien 
                                    
                                 
                                 
                                    
                                       de_AT
                                    
                                    
                                       deutsch Österreich 
                                    
                                 
                                 
                                    
                                       de_CH
                                    
                                    
                                       Deutsch Schweiz 
                                    
                                 
                                 
                                    
                                       de_DE
                                    
                                    
                                       Deutsch Deutschland 
                                    
                                 
                                 
                                    
                                       el_GR
                                    
                                    
                                       Griechisch Griechenland 
                                    
                                 
                                 
                                    
                                       en_GB
                                    
                                    
                                       Englisch Grossbrittanien 
                                    
                                 
                                 
                                    
                                       en_US
                                    
                                    
                                       Englisch USA 
                                    
                                 
                                 
                                    
                                       es_ES
                                    
                                    
                                       Spanisch Spanien 
                                    
                                 
                                 
                                    
                                       fr_CH
                                    
                                    
                                       Französisch Schweiz 
                                    
                                 
                                 
                                    
                                       fr_FR
                                    
                                    
                                       Französisch Frankreich 
                                    
                                 
                                 
                                    
                                       hu_HU
                                    
                                    
                                       Ungarisch Ungarn 
                                    
                                 
                                 
                                    
                                       it_CH
                                    
                                    
                                       Italienisch Schweiz 
                                    
                                 
                                 
                                    
                                       it_IT
                                    
                                    
                                       Italienisch Italien 
                                    
                                 
                                 
                                    
                                       nl_NL
                                    
                                    
                                       Niederländisch Niederlande
                                    
                                 
                                 
                                    
                                       pl_PL
                                    
                                    
                                       Polnisch Polen 
                                    
                                 
                                 
                                    
                                       ro_RO
                                    
                                    
                                       Rumänisch Rumänien 
                                    
                                 
                                 
                                    
                                       ru_RU
                                    
                                    
                                       Russisch Russland 
                                    
                                 
                                 
                                    
                                       sk_SK
                                    
                                    
                                       Slowakisch Slowakei 
                                    
                                 
                                 
                                    
                                       tr_TR
                                    
                                    
                                       Türkisch Türkei
                                    
                                 
                              
                           
                        
                        
                     
                  
               
               
                  String
               
               
                  Sprachkürzel 
               
               
                  Sprachkürzel (Language)
                  
                     
                        
                           
                              
                                 
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                 
                                 
                                    
                                       ca_ES
                                    
                                    
                                       Katalanisch Spanien 
                                    
                                 
                                 
                                    
                                       cs_CZ
                                    
                                    
                                       Tschechisch Tschechien 
                                    
                                 
                                 
                                    
                                       de_AT
                                    
                                    
                                       deutsch Österreich 
                                    
                                 
                                 
                                    
                                       de_CH
                                    
                                    
                                       Deutsch Schweiz 
                                    
                                 
                                 
                                    
                                       de_DE
                                    
                                    
                                       Deutsch Deutschland 
                                    
                                 
                                 
                                    
                                       el_GR
                                    
                                    
                                       Griechisch Griechenland 
                                    
                                 
                                 
                                    
                                       en_GB
                                    
                                    
                                       Englisch Grossbrittanien 
                                    
                                 
                                 
                                    
                                       en_US
                                    
                                    
                                       Englisch USA 
                                    
                                 
                                 
                                    
                                       es_ES
                                    
                                    
                                       Spanisch Spanien 
                                    
                                 
                                 
                                    
                                       fr_CH
                                    
                                    
                                       Französisch Schweiz 
                                    
                                 
                                 
                                    
                                       fr_FR
                                    
                                    
                                       Französisch Frankreich 
                                    
                                 
                                 
                                    
                                       hu_HU
                                    
                                    
                                       Ungarisch Ungarn 
                                    
                                 
                                 
                                    
                                       it_CH
                                    
                                    
                                       Italienisch Schweiz 
                                    
                                 
                                 
                                    
                                       it_IT
                                    
                                    
                                       Italienisch Italien 
                                    
                                 
                                 
                                    
                                       nl_NL
                                    
                                    
                                       Niederländisch Niederlande
                                    
                                 
                                 
                                    
                                       pl_PL
                                    
                                    
                                       Polnisch Polen 
                                    
                                 
                                 
                                    
                                       ro_RO
                                    
                                    
                                       Rumänisch Rumänien 
                                    
                                 
                                 
                                    
                                       ru_RU
                                    
                                    
                                       Russisch Russland 
                                    
                                 
                                 
                                    
                                       sk_SK
                                    
                                    
                                       Slowakisch Slowakei 
                                    
                                 
                                 
                                    
                                       tr_TR
                                    
                                    
                                       Türkisch Türkei
                                    
                                 
                              
                           
                        
                        
                     
                  
               
               
                  X
               
            
            
               
                  vxs:Country
               
               
                  String
               
               
                  Landeskürzel des betreffenden Datenlands
               
               
                  ISO 3166 ALPHA-2weitere Infos siehe Popup-Fenster
               
               
                  X
               
            
            
               
                  vxs:Currency¹
                  
                     
                        
                           
                              
                                 
                                    
                                       Wert
                                    
                                    
                                       Beschreibung
                                    
                                 
                                 
                                    
                                       CZK
                                    
                                    
                                       Krone (CZ) 
                                    
                                 
                                 
                                    
                                       EUR
                                    
                                    
                                       Euro 
                                    
                                 
                                 
                                    
                                       GBP
                                    
                                    
                                       Pfund Sterling (GB) 
                                    
                                 
                                 
                                    
                                       HUF
                                    
                                    
                                       Forint (H) 
                                    
                                 
                                 
                                    
                                       PLN
                                    
                                    
                                       Zloty (PL) 
                                    
                                 
                                 
                                    
                                       RON
                                    
                                    
                                       (neuer) Leu (RO) 
                                    
                                 
                                 
                                    
                                       RUB
                                    
                                    
                                       Rubel (RUS) 
                                    
                                 
                                 
                                    
                                       SFR
                                    
                                    
                                       Franken (CH) 
                                    
                                 
                                 
                                    
                                       SKK
                                    
                                    
                                       Krone (SK) 
                                    
                                 
                                 
                                    
                                       TL
                                    
                                    
                                       Lira (TR)
                                    
                                 
                              
                           
                        
                        
                     
                  
               
               
                  String
               
               
                  Währungskürzel
               
               
                  ISO 4217weitere Infos siehe Popup-Fenster
               
               
                  X
               
            
            
               
                  vxs:Name
               
               
                  String
               
               
                  Bezeichnung des Vorgangs 
               
               
                  
               
               
                  
               
            
            
               
                  vxs:DossierType
               
               
                  String
               
               
                  Typ des anzulegenden Vorgangs
               
               
                  bundlePro 
               
               
                  
               
            
            
               
                  vxs:Vehicle
               
               
                  Vehicle
               
               
                  Enthält Fahrzeugdaten als Unterelemente
               
               
                  
               
               
                  X
               
            
            
               
                  vxs:VAT
               
               
                  VAT
               
               
                  Enthält Steuerdaten als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Valuation
               
               
                  Valuation
               
               
                  Enthält bewertungsrelevante Daten als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  vxs:TradingActivity
               
               
                  TradingActivity
               
               
                  Enthält die Informationen zu den Handelstätigkeiten (Coverage=EXTENDEDBYTRADING)
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:Vehicle
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:Country¹
                  
                     
                        
                           
                              
                                 
                                    
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
                                    
                                 
                              
                           
                        
                        
                        
                     
                  
               
               
                  String
               
               
                  Landeskürzel des betreffenden Datenlands
               
               
                  ISO 3166 ALPHA-2 weitere Infos siehe Popup-Fenster
               
               
                  X
               
            
            
               
                  vxs:DatECode
               
               
                  String
               
               
                  DAT €uropa-Code®
               
               
                  15-stellig
               
               
                  X
               
            
            
               
                  vxs:Container
               
               
                  String
               
               
                  Marktindex 
               
               
                  [Landessetzung, 2-stellig][Nummer des Marktindex, 3stellig]
               
               
                  X
               
            
            
               
                  vxs:ConstructionTime¹
               
               
                  Integer
               
               
                  Bauzeit¹
               
               
                  4-stellig numerisch
               
               
                  X
               
            
            
               
                  vxs:MileageEstimated
               
               
                  Integer
               
               
                  Kilometerstand
               
               
                  numerisch
               
               
                  X
               
            
            
               
                  vxs:InitialRegistration¹
                  
                     
                        Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex darf nicht
                           größer als 1 Jahr sein. In der Fahrzeugbewertung kann sonst kein Wert ermittelt werden.
                           
                     
                  
               
               
                  Date
               
               
                  Erstzulassungsdatum
               
               
                  YYYY-MM-DD
                  weitere Infos siehe Popup-Fenster
               
               
                  X
               
            
            
               
                  vxs:VehicleIdentNumber
               
               
                  String
               
               
                  Fahrzeugidentifikationsnummer (Fahrgestellnummer); Vehicle identification number
               
               
                  17-stellig
               
               
                  
               
            
            
               
                  vxs:TechInfo
               
               
                  TechInfo
               
               
                  Enthält technische Daten des Fahrzeugs als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  vxs:RegistrationData
               
               
                  RegistrationData
               
               
                  Enthält die Zulassungsdaten
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Equipment
               
               
                  Equipment
               
               
                  Enthält Ausstattungslisten als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  vxs:UpperBodies
               
               
                  UpperBodies
               
               
                  Enthält Aufbauten als Unterelemente; nur für Fahrzeugart LKW und Transporter
               
               
                  noch nicht aktiv
               
               
                  
               
            
            
               
                  vxs:Tires
               
               
                  Tires
               
               
                  Enthält die Achsendaten
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:TechInfo
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:CountOfAxles origin="user"
               
               
                  Integer
               
               
                  Anzahl der Vorderachse
               
               
                  
               
               
                  
               
            
            
               
                  vxs:CountOfDrivedAxles origin="user"
               
               
                  Integer
               
               
                  Anzahl der Hinterachse
               
               
                  
               
               
                  
               
            
            
               
                  vxs:WheelBase origin="user"
               
               
                  Integer
               
               
                  Radstand in mm
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Length origin="user"
               
               
                  Integer
               
               
                  Länge
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Width origin="user"
               
               
                  Integer
               
               
                  Breite
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Height origin="user"
               
               
                  Integer
               
               
                  Höhe
               
               
                  
               
               
                  
               
            
            
               
                  vxs:VehicleSeats origin="user"
               
               
                  Integer
               
               
                  Anzahl der Sitzplätze
               
               
                  ###
               
               
                  
               
            
            
               
                  vxs:VehicleDoors origin="user"
               
               
                  Integer
               
               
                  Anzahl der Türen
               
               
                  ###
               
               
                  
               
            
            
               
                  vxs:CountOfAirbags origin="user"
               
               
                  Integer
               
               
                  Anzahl der Airbags
               
               
                  ###
               
               
                  
               
            
            
               
                  vxs:Acceleration origin="user"
               
               
                  Decimal
               
               
                  Beschleunigung
               
               
                  #####
               
               
                  
               
            
            
               
                  vxs:SpeedMax origin="user"
               
               
                  Integer
               
               
                  Höchstgeschwindigkeit
               
               
                  ####
               
               
                  
               
            
            
               
                  vxs:PowerHp origin="user"
               
               
                  Integer
               
               
                  Leistung in PS
               
               
                  #####
               
               
                  
               
            
            
               
                  vxs:PowerKw origin="user"
               
               
                  Decimal
               
               
                  Leistung in kW
               
               
                  #####
               
               
                  
               
            
            
               
                  vxs:Capacitiy origin="user"
               
               
                  Integer
               
               
                  Hubraum
               
               
                  ######
               
               
                  
               
            
            
               
                  vxs:CylinderArrangement origin="user"
               
               
                  String30
               
               
                  Zylinderanordnung
               
               
                  ##
               
               
                  
               
            
            
               
                  vxs:RotationsOnMaxPower origin="user"
               
               
                  Integer
               
               
                  Umdrehungen bei maximaler Leistung
               
               
                  #####
               
               
                  
               
            
            
               
                  vxs:RotationsOnMaxTorque origin="user"
               
               
                  Integer
               
               
                  Umdrehung bei maximalen Drehmoment
               
               
                  #####
               
               
                  
               
            
            
               
                  vxs:Torque origin="user"
               
               
                  Integer
               
               
                  Drehmoment
               
               
                  #####
               
               
                  
               
            
            
               
                  vxs:TankVolume origin="user"
               
               
                  Integer
               
               
                  Tankinhalt(ltr.)
               
               
                  0-99999
               
               
                  
               
            
            
               
                  vxs:ConsumptionInTown origin="user"
               
               
                  Integer
               
               
                  Kraftstoffverbrauch innerorts
               
               
                  0-99999
               
               
                  
               
            
            
               
                  vxs:ConsumptionOutOfTown origin="user"
               
               
                  Integer
               
               
                  Kraftstoffverbrauch außerorts
               
               
                  0-99999
               
               
                  
               
            
            
               
                  vxs:Consumption origin="user"
               
               
                  Integer
               
               
                  Kraftstoffverbrauch kombiniert
               
               
                  0-99999
               
               
                  
               
            
            
               
                  vxs:Co2Emission origin="user"
               
               
                  Integer
               
               
                  CO2-Ausstoß (g/km)
               
               
                  
               
               
                  
               
            
            
               
                  vxs:EmissionClassN
                  
                     
                        Element vxs:EmissionClassN
                        
                           
                              
                                 
                                    
                                       Parameter
                                    
                                    
                                       Datentyp
                                    
                                    
                                       Beschreibung
                                    
                                    
                                       Schreibweise
                                    
                                    
                                       Pflicht
                                    
                                 
                                 
                                    
                                       vxs:EmissionClassItemN
                                       
                                          
                                             Element vxs:EmissionClassItemN
                                             
                                                
                                                   
                                                      
                                                         
                                                            Attribut
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                         
                                                            Pflicht
                                                         
                                                      
                                                      
                                                         
                                                            type
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Typ der Emissionsklasse
                                                         
                                                         
                                                            EU, CN
                                                         
                                                         
                                                            
                                                         
                                                      
                                                      
                                                         
                                                            description
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Beschreibung der Emissionsklasse
                                                         
                                                         
                                                            
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                             
                                                
                                                   
                                                      
                                                         
                                                            Parameter
                                                         
                                                         
                                                            Datentyp
                                                         
                                                         
                                                            Beschreibung
                                                         
                                                         
                                                            Schreibweise
                                                         
                                                         
                                                            Pflicht
                                                         
                                                      
                                                      
                                                         
                                                            vxs:EmissionClassDescription
                                                         
                                                         
                                                            String
                                                         
                                                         
                                                            Beschreibung der Emissionsklasse (neu)
                                                         
                                                         
                                                            
                                                         
                                                         
                                                            
                                                         
                                                      
                                                   
                                                
                                             
                                             
                                          
                                       
                                    
                                    
                                       EmissionClassItemN
                                    
                                    
                                       Enthält Werte in den Attributen type und description
                                    
                                    
                                       
                                    
                                    
                                       
                                    
                                 
                              
                           
                        
                        
                     
                  
               
               
                  EmissionClassN
               
               
                  Schadstoffklasse
               
               
                  
               
               
                  
               
            
            
               
                  vxs:DriveN origin="user"
               
               
                  String
               
               
                  Antriebsart
               
               
                  
               
               
                  
               
            
            
               
                  vxs:EngineCycle origin="user"
               
               
                  Integer
               
               
                  Motorsteuerung (Takt)
               
               
                  0-9
               
               
                  
               
            
            
               
                  vxs:FuelMethod origin="user"
               
               
                  String
               
               
                  Kraftstofftyp
               
               
                  
               
               
                  
               
            
            
               
                  vxs:FuelMethodType origin="user"
               
               
                  String
               
               
                  Kraftstoffart
               
               
                  
               
               
                  
               
            
            
               
                  vxs:UnloadedWeight origin="user"
               
               
                  Integer
               
               
                  Leergewicht (kg)
               
               
                  0-99999
               
               
                  
               
            
            
               
                  vxs:PermissableTotalWeight origin="user"
               
               
                  Integer
               
               
                  Zulässige Gesamtgewicht
               
               
                  0-99999
               
               
                  
               
            
            
               
                  vxs:WidthForGarage origin="user"
               
               
                  Integer
               
               
                  Fahrzeugbreite-Garagenmaß (mm)
               
               
                  0-99999
               
               
                  
               
            
            
               
                  vxs:EnergyEfficiencyClass origin="user"
               
               
                  String
               
               
                  Energieeffizienzklasse
               
               
                  A+,A,B,C,D,E,F,G
               
               
                  
               
            
            
               
                  vxs:TechInfoWltp
               
               
                  TechInfoWltp
               
               
                  Enhält Wltp-Daten des Fahrzeugs als Unterelemente
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:TechInfoWltp
   
      
         Element vxs:TechInfoWltp
         
            
               
                  
                     
                        Parameter
                     
                     
                        Datentyp
                     
                     
                        Beschreibung
                     
                     
                        Schreibweise
                     
                     
                        Pflicht
                     
                  
                  
                     
                        vxs:WltpConsumptionLowMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch (l/100 km) bei niedrigen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionLowMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch (l/100 km) bei niedrigen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionMediumMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch (l/100 km) bei mittleren Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionMediumMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch (l/100 km) bei mittleren Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionHighMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch (l/100 km) bei hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionHighMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch (l/100 km) bei hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionExtraHighMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch (l/100 km) bei sehr hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionExtraHighMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch (l/100 km) bei sehr hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionMixedMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch (l/100 km) bei gemischten Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionMixedMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch (l/100 km) bei gemischten Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentLowCngMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km)
                           bei niedrigen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentLowCngMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km)
                           bei niedrigen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMediumCngMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km)
                           bei mittleren Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMediumCngMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km)
                           bei mittleren Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentHighCngMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km)
                           bei hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentHighCngMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km)
                           bei hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentExtraHighCngMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km)
                           bei sehr hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentExtraHighCngMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km)
                           bei sehr hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMixedCngMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km)
                           bei gemischten Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMixedCngMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch CNG (i.d.R. kg/100 km, in Ausnahmefällen m³/100 km)
                           bei gemischten Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentLowLpgMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch LPG (l/100 km) bei niedrigen Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentLowLpgMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch LPG (l/100 km) bei niedrigen Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMediumLpgMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch LPG (l/100 km) bei mittleren Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMediumLpgMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch LPG (l/100 km) bei mittleren Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentHighLpgMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch LPG (l/100 km) bei hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentHighLpgMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch LPG (l/100 km) bei hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentExtraHighLpgMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch LPG (l/100 km) bei sehr hohen Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentExtraHighLpgMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch LPG (l/100 km) bei sehr hohen Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMixedLpgMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch LPG (l/100 km) bei gemischten Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMixedLpgMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch LPG (l/100 km) bei gemischten Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentLowHMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch H (kg/100 km) bei niedrigen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentLowHMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch H (kg/100 km) bei niedrigen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMediumHMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch H (kg/100 km) bei mittleren Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMediumHMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch H (kg/100 km) bei mittleren Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentHighHMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch H (kg/100 km) bei hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentHighHMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch H (kg/100 km) bei hohen Geschwindigkeiten nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentExtraHighHMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch H (kg/100 km) bei sehr hohen Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentExtraHighHMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch H (kg/100 km) bei sehr hohen Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMixedHMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch H (kg/100 km) bei gemischten Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionBivalentMixedHMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch H (kg/100 km) bei gemischten Geschwindigkeiten nach
                           WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2ClassMin
                     
                     
                        String
                     
                     
                        Minimale CO2 Emissionsklasse nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2ClassMax
                     
                     
                        String
                     
                     
                        Maximale CO2 Emissionsklasse nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2ClassWithDischargedBatteryMin
                     
                     
                        String
                     
                     
                        Minimale CO2 Emissionsklasse mit entladener Batterie nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2ClassWithDischargedBatteryMax
                     
                     
                        String
                     
                     
                        Maximale CO2 Emissionsklasse mit entladener Batterie nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2EmissionMin
                     
                     
                        Decimal
                     
                     
                        Minimaler CO2-Ausstoß (g/km) nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2EmissionMax
                     
                     
                        Decimal
                     
                     
                        Maximaler CO2-Ausstoß (g/km) nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2EmissionWithDischargedBatteryMin
                     
                     
                        Decimal
                     
                     
                        Minimaler CO2-Ausstoß (g/km) mit entladener Batterie nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2EmissionWithDischargedBatteryMax
                     
                     
                        Decimal
                     
                     
                        Maximaler CO2-Ausstoß (g/km) mit entladener Batterie nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Stromverbrauch (kWh/100 km) nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Stromverbrauch (kWh/100 km) nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionWithDischargedBatteryMin
                     
                     
                        Decimal
                     
                     
                        Minimaler Kraftstoffverbrauch (l/100 km) mit entladener Batterie nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionWithDischargedBatteryMax
                     
                     
                        Decimal
                     
                     
                        Maximaler Kraftstoffverbrauch (l/100 km) mit entladener Batterie nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpRangeElectricalMin
                     
                     
                        Integer
                     
                     
                        Elektromotor-Reichweite (km) bei min. nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpRangeElectricalMax
                     
                     
                        Integer
                     
                     
                        Elektromotor-Reichweite (km) bei max. nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpRangeTotalMin
                     
                     
                        Integer
                     
                     
                        Gesamtreichweite (km) bei min. nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpRangeTotalMax
                     
                     
                        Integer
                     
                     
                        Gesamtreichweite (km) bei max. nach WLTP
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        neue Felder:
                     
                     
                        
                     
                     
                        
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2EmissionElectricalMin
                     
                     
                        Decimal
                     
                     
                        CO2-Ausstoß (g/km) bei elektrischem Betrieb nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2EmissionElectricalMax
                     
                     
                        Decimal
                     
                     
                        CO2-Ausstoß (g/km) bei elektrischem Betrieb nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2ClassElectricalMin
                     
                     
                        String
                     
                     
                        CO2-Klasse bei elektrischem Betrieb nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2ClassElectricalMax
                     
                     
                        String
                     
                     
                        CO2-Klasse bei elektrischem Betrieb nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionWithDischargedBatteryLowMin
                     
                     
                        Decimal
                     
                     
                        Kraftstoffverbrauch (l/100km) bei entladener Batterie bei niedrigen Geschwindigkeiten
                           nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionWithDischargedBatteryLowMax
                     
                     
                        Decimal
                     
                     
                        Kraftstoffverbrauch (l/100km) bei entladener Batterie bei niedrigen Geschwindigkeiten
                           nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionWithDischargedBatteryMediumMin
                     
                     
                        Decimal
                     
                     
                        Kraftstoffverbrauch (l/100km) bei entladener Batterie bei mittleren Geschwindigkeiten
                           nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionWithDischargedBatteryMediumMax
                     
                     
                        Decimal
                     
                     
                        Kraftstoffverbrauch (l/100km) bei entladener Batterie bei mittleren Geschwindigkeiten
                           nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionWithDischargedBatteryHighMin
                     
                     
                        Decimal
                     
                     
                        Kraftstoffverbrauch (l/100km) bei entladener Batterie bei hohen Geschwindigkeiten
                           nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionWithDischargedBatteryHighMax
                     
                     
                        Decimal
                     
                     
                        Kraftstoffverbrauch (l/100km) bei entladener Batterie bei hohen Geschwindigkeiten
                           nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionWithDischargedBatteryExtraHighMin
                     
                     
                        Decimal
                     
                     
                        Kraftstoffverbrauch (l/100km) bei entladener Batterie bei sehr hohen Geschwindigkeiten
                           nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionWithDischargedBatteryExtraHighMax
                     
                     
                        Decimal
                     
                     
                        Kraftstoffverbrauch (l/100km) bei entladener Batterie bei sehr hohen Geschwindigkeiten
                           nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionEnergyLtrMin
                     
                     
                        Decimal
                     
                     
                        Energieverbrauch (l/100km) nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionEnergyLtrMax
                     
                     
                        Decimal
                     
                     
                        Energieverbrauch (l/100km) nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionEnergyElectricalMin
                     
                     
                        Decimal
                     
                     
                        Energieverbrauch bei elektrischem Betrieb (kWh/100 km) kombiniert nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionEnergyElectricalMax
                     
                     
                        Decimal
                     
                     
                        Energieverbrauch bei elektrischem Betrieb (kWh/100 km) kombiniert nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalLowMin
                     
                     
                        Decimal
                     
                     
                        Stromverbrauch (kWh/100 km) bei niedrigen Geschwindigkeiten nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalLowMax
                     
                     
                        Decimal
                     
                     
                        Stromverbrauch (kWh/100 km) bei niedrigen Geschwindigkeiten nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalMediumMin
                     
                     
                        Decimal
                     
                     
                        Stromverbrauch (kWh/100 km) bei mittleren Geschwindigkeiten nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalMediumMax
                     
                     
                        Decimal
                     
                     
                        Stromverbrauch (kWh/100 km) bei mittleren Geschwindigkeiten nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalHighMin
                     
                     
                        Decimal
                     
                     
                        Stromverbrauch (kWh/100 km) bei hohen Geschwindigkeiten nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalHighMax
                     
                     
                        Decimal
                     
                     
                        Stromverbrauch (kWh/100 km) bei hohen Geschwindigkeiten nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalExtraHighMin
                     
                     
                        Decimal
                     
                     
                        Stromverbrauch (kWh/100 km) bei sehr hohen Geschwindigkeiten nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalExtraHighMax
                     
                     
                        Decimal
                     
                     
                        Stromverbrauch (kWh/100 km) bei sehr hohen Geschwindigkeiten nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalCityMin
                     
                     
                        Decimal
                     
                     
                        Stromverbrauch (kWh/100 km) im City-Betrieb nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionElectricalCityMax
                     
                     
                        Decimal
                     
                     
                        Stromverbrauch (kWh/100 km) im City-Betrieb nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpRangeElectricalCityMin
                     
                     
                        Integer
                     
                     
                        Reichweite (km) bei elektrischem City-Betrieb nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpRangeElectricalCityMax
                     
                     
                        Integer
                     
                     
                        Reichweite (km) bei elektrischem City-Betrieb nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionCngUnit
                     
                     
                        String
                     
                     
                        CNG Verbrauchseinheit für WLTP-Werte (Benutzer-Feld aktuell nicht unterstützt)
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2EmissionBivalentMin
                     
                     
                        Decimal
                     
                     
                        CO2-Ausstoß (g/km) bei CNG-, LPG- oder Wasserstoffbetrieb nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2EmissionBivalentMax
                     
                     
                        Decimal
                     
                     
                        CO2-Ausstoß (g/km) bei CNG-, LPG- oder Wasserstoffbetrieb nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2ClassBivalentMin
                     
                     
                        String
                     
                     
                        CO2-Klasse bei CNG-, LPG- oder Wasserstoffbetrieb nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2ClassBivalentMax
                     
                     
                        String
                     
                     
                        CO2-Klasse bei CNG-, LPG- oder Wasserstoffbetrieb nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionEnergyBivalentMax
                     
                     
                        Decimal
                     
                     
                        Energieverbrauch (kg/100 km) bei CNG-, LPG- oder Wasserstoffbetrieb (cbm/100 km im
                           Falle von CNG und WltpConsumptionCngUnit == 'CBM') nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionEnergyWeightedLtrMin
                     
                     
                        Decimal
                     
                     
                        Energieverbrauch gewichtet (l/100km) nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionEnergyWeightedLtrMax
                     
                     
                        Decimal
                     
                     
                        Energieverbrauch gewichtet (l/100km) nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionEnergyWeightedKwhMin
                     
                     
                        Decimal
                     
                     
                        Energieverbrauch gewichtet (kWh/100 km) nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpConsumptionEnergyWeightedKwhMax
                     
                     
                        Decimal
                     
                     
                        Energieverbrauch gewichtet (kWh/100 km) nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2EmissionWeightedMin
                     
                     
                        Decimal
                     
                     
                        CO2-Ausstoß (g/km) gewichtet kombiniert nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2EmissionWeightedMax
                     
                     
                        Decimal
                     
                     
                        CO2-Ausstoß (g/km) gewichtet kombiniert nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2ClassWeightedMin
                     
                     
                        String
                     
                     
                        CO2-Klasse gewichtet kombiniert nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpCo2ClassWeightedMax
                     
                     
                        String
                     
                     
                        CO2-Klasse gewichtet kombiniert nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpUtilFactorPercentMin
                     
                     
                        Decimal
                     
                     
                        Nutzungsfaktor (%) nach WLTP min.
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:WltpUtilFactorPercentMax
                     
                     
                        Decimal
                     
                     
                        Nutzungsfaktor (%) nach WLTP max.
                     
                     
                        
                     
                     
                        
                     
                  
               
            
         
         
      
   
   Element vxs:Tires
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:Axles
               
               
                  Axles
               
               
                  Enthält die Achsendaten als Unterlemente.
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:Axle
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:AxleNo
               
               
                  Integer
               
               
                  Nummer der Achse
               
               
                  numerisch
               
               
                  X
               
            
            
               
                  vxs:TireId
               
               
                  Integer
               
               
                  DAT-Reifennummer; optional bei ManualEntry = true, Pflicht bei ManualEntry = false.
               
               
                  numerisch
               
               
                  bedingt
               
            
            
               
                  vxs:TireState
               
               
                  String
               
               
                  Reifenstatus
               
               
                  mounted, unmounted,spare wheel
               
               
                  X
               
            
            
               
                  vxs:NrOfTires
               
               
                  Integer
               
               
                  Reifenanzahl, Werte montierte Reifen: PKW, beliebige Achse: 2; Transporter und LKW, erste Achse: 2, weitere Achsen: 2 oder 4; Kraftrad, erste Achse: 1 oder 2, weitere Achsen: 1. Werte unmontierte Reifen oder Reserverad: 1.
               
               
                  1,
                  2,
                  4
               
               
                  X
               
            
            
               
                  vxs:TireType
               
               
                  String
               
               
                  Reifenart
               
               
                  
               
               
                  
               
            
            
               
                  vxs:TireOriginalPrice
               
               
                  Decimal
               
               
                  Neupreis als Nettowert; ohne Auswirkung bei ManualEntry = false, erforderlich bei ManualEntry = true.
               
               
                  
               
               
                  bedingt
               
            
            
               
                  vxs:TireSpeedIndex
               
               
                  String
               
               
                  Geschwindigkeitsindex
               
               
                  
               
               
                  
               
            
            
               
                  vxs:TireSize
               
               
                  String
               
               
                  Reifengröße
               
               
                  
               
               
                  
               
            
            
               
                  vxs:TireSafetySystem
               
               
                  String
               
               
                  Reifen-Sicherheitssystem
               
               
                  
               
               
                  
               
            
            
               
                  vxs:TireManufacturer
               
               
                  Integer
               
               
                  Code für Reifenhersteller
               
               
                  numerisch
               
               
                  
               
            
            
               
                  vxs:TireManufacturerName
               
               
                  String
               
               
                  Name des Reifenherstellers
               
               
                  
               
               
                  
               
            
            
               
                  vxs:TireOriginalTreadDepth
               
               
                  Integer
               
               
                  Reifenprofiltiefe. Positiver Wert
               
               
                  numerisch
               
               
                  X
               
            
            
               
                  vxs:TireLoadCapacityIndex
               
               
                  Integer
               
               
                  Reifen-Tragfähigkeitsindex in kg
               
               
                  
               
               
                  
               
            
            
               
                  vxs:TireLoadCapacityIndex2
               
               
                  Integer
               
               
                  Reifen-Tragfähigkeitsindex 2 in kg
               
               
                  
               
               
                  
               
            
            
               
                  vxs:TreadDepthLeftOuterPerc
               
               
                  Decimal
               
               
                  Profiltiefe in Prozent; Pflicht bei NrOfTires = 1 für links außen und bei NrOfTires = 2 für links außen und rechts außen und bei NrOfTires = 4 für links außen, links innen, rechts außen und rechts innen.
                  Wurden Angaben in Prozent und Millimeter gemacht, werden die Angaben in Millimeter
                     im Ausdruck verwendet.
               
               
                  numerisch
               
               
                  bedingt
               
            
            
               
                  vxs:TreadDepthLeftInnerPerc
               
            
            
               
                  vxs:TreadDepthRightInnerPerc
               
            
            
               
                  vxs:TreadDepthRightOuterPerc
               
            
            
               
                  
               
            
            
               
                  vxs:TreadDepthLeftOuterMm
               
               
                  Decimal
               
               
                  Profiltiefe in Millimeter. Pflicht bei NrOfTires = 1 für links außen und bei NrOfTires = 2 für links außen und rechts außen und bei NrOfTires = 4 für links außen, links innen, rechts außen und rechts innen.
                  Wurden Angaben in Prozent und Millimeter gemacht, werden die Angaben in Millimeter
                     im Ausdruck verwendet.
               
               
                  numerisch
                  
               
               
                  bedingt
               
            
            
               
                  vxs:TreadDepthLeftInnerMm
               
            
            
               
                  vxs:TreadDepthRightInnerMm
               
            
            
               
                  vxs:TreadDepthRightOuterMm
               
            
            
               
                  vxs:ManualEntry
               
               
                  Boolean
               
               
                  manuelle Dateneingabe
               
               
                  true= manueller Eintragfalse= kein manueller Eintrag
               
               
                  X
               
            
            
               
                  vxs:RetreadedLeftOuter
               
               
                  Boolean
               
               
                  Kennzeichen: Reifen runderneuert
               
               
                  true = runderneuertfalse = nicht runderneuert
               
               
                  
               
            
            
               
                  vxs:RetreadedLeftInner
               
            
            
               
                  vxs:RetreadedRightInner
               
            
            
               
                  vxs:RetreadedRightOuter
               
            
         
      
   
   Element vxs:VAT
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:VatType
               
               
                  String
               
               
                  Besteuerungsart. Wird kein Wert oder ein falscher Wert übergeben, wird bei Gebrauchtfahrzeugen
                     mit Differenzbesteuerung bewertet. Bei Neufahrzeugen wird mit Regelbesteuerung bewertet.
                     Für Neufahrzeuge ist nur die Regelbesteuerung zulässig.
               
               
                  REGULAR = Regelbesteuerung; DIFFERENCE = Differenzbesteuerung
               
               
                  nur für vxs:Condition  Pflicht
               
            
         
      
   
   Element vxs:Valuation
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:ValuationType
               
               
                  String
               
               
                  Bewertungsart; Pflicht für pauschale Ausstattungswerte
               
               
                  VALUATION = Gebrauchtfahrzeug,Standardwert ist VALUATION
               
               
                  bedingt
               
            
            
               
                  vxs:ExtendedMileageCorrection
               
               
                  Boolean
               
               
                  Kennzeichen; seit 04/2015 ohne Auswirkung, da die Berechnung immer mit erweiterter
                     Kilometerkorrektur stattfindet.
               
               
                  
               
               
                  
               
            
            
               
                  vxs:MileageCorr
               
               
                  Decimal
               
               
                  Betrag für Kilometerkorrektur (Netto)
               
               
                  
               
               
                  
               
            
            
               
                  vxs:AdditionalManualMileageCorr
               
               
                  Decimal
               
               
                  Manueller Korrekturwert bei Fahrzeugbewertungen mit einer Laufleistung unter/über
                     der DAT-Richtlinie. Für diesen Fall Pflicht.
               
               
                  numerisch
               
               
                  bedingt
               
            
            
               
                  vxs:InitialRegistrationCorr
               
               
                  Decimal
               
               
                  Betrag für Erstzulassungskorrektur (Netto)
               
               
                  
               
               
                  
               
            
            
               
                  vxs:EquipmentPrice
               
               
                  Decimal
               
               
                  manuelle Vorgabe des Ausstattungsrestwerts (gesamt) als Nettowert; Nicht zulässig
                     in Kombination mit ManualEquipmentOriginalPrice
               
               
                  numerisch, positiv
               
               
                  
               
            
            
               
                  vxs:ManualEquipmentOriginalPrice
               
               
                  Decimal
               
               
                  manuelle Vorgabe eines pauschalen Ausstattungsgesamtpreis in Euro als Nettowert. Nicht
                     zulässig in Kombination mit EquipmentPrice
               
               
                  numerisch, positiv
               
               
                  
               
            
            
               
                  vxs:EquipmentPercentage
               
               
                  Integer
               
               
                  der pauschale Ausstattungsgesamtpreis kann in zwei Teile aufgeteilt werden, die unterschiedlich
                     abgewertet werden. Beispiel: Paket1, 60%, RW | Paket2, T4. Mit diesem Wert legen Sie den ersten prozentualen Anteil fest. 
               
               
                  numerisch [1 - 100]
               
               
                  
               
            
            
               
                  vxs:EquipmentDecreaseType¹
               
               
                  String
               
               
                  Abwertungsart für den ersten  Anteil
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  vxs:EquipmentDecreaseTypeRemaining¹
               
               
                  String
               
               
                  Abwertungsart für den restlichen Anteil
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  vxs:PrognosisDate
               
               
                  Date
               
               
                  Zukunftsprognosedatum
               
               
                  gültig nur ab aktuellen Datum
               
               
                  
               
            
            
               
                  vxs:PrognosisMileageUser
               
               
                  Decimal
               
               
                  Laufleistung für die Zukunftsprognose
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Condition
               
               
                  Condition¹ 
               
               
                  enthält Zustandsdaten als Unterelemente
               
               
                  Condition
               
               
                  
               
            
            
               
                  vxs:DefaultPlatformPresent
               
               
                  String
               
               
                  Serienaufbau vorhanden?
               
               
                  present = Serienaufbau vorhandendesigned but missing = Serienaufbau abgewähltnot designed and missing = nicht vorhanden
               
               
                  
               
            
         
      
   
   Element vxs:RegistrationData
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:LicenseNumber
               
               
                  String
               
               
                  amtliches Kennzeichen
               
               
                  
               
               
                  
               
            
            
               
                  vxs:KbaCode
               
               
                  String
               
               
                  HSN/TSN
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:Equipment
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:SpecialEquipment
               
               
                  EquipSequence
               
               
                  Sonderausstattungen; Enthält 0 bis n Positionen vxs:EquipmentPosition als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  vxs:AdditionalEquipment
               
               
                  EquipSequence
               
               
                  Zusatzausstattungen; Enthält 0 bis n Positionen vxs:EquipmentPosition als Unterelemente
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:EquipmentPosition
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:DatEquipmentId
               
               
                  Integer
               
               
                  DAT Ausstattungsnummer Pflicht bei Sonderausstattung
               
               
                  numerisch
               
               
                  bedingt
               
            
            
               
                  vxs:Description
               
               
                  String
               
               
                  Name/Beschreibung der Ausstattung nur bei Zusatzausstattung möglich
               
               
                  
               
               
                  
               
            
            
               
                  vxs:DecreaseType¹
               
               
                  String
               
               
                  Abwertungsart.Eine Vorgabe wird nur benötigt, falls Sie die DAT-Standardvorgabe überschreiben möchten.
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  vxs:InstallDate
               
               
                  Date
               
               
                  Einbaudatum nur bei Zusatzausstattung möglich
               
               
                  YYYY-MM-DD
               
               
                  
               
            
            
               
                  vxs:OriginalPrice
               
               
                  Decimal
               
               
                  Neupreis als Nettowert nur bei Zusatzausstattung möglich
               
               
                  
               
               
                  
               
            
            
               
                  vxs:ResidualValue
               
               
                  Decimal
               
               
                  Restwert (Netto)
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:Condition
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:IncreaseInValue
               
               
                  Decimal
               
               
                  Werterhöhung (Nettowert)
               
               
                  +###########.##
               
               
                  
               
            
            
               
                  vxs:DecreaseInValue
               
               
                  Decimal
               
               
                  Wertminderung (Nettowert)
               
               
                  +###########.##
               
               
                  
               
            
            
               
                  vxs:TiresMountedValue
               
               
                  Decimal
               
               
                  Wertanpassung als Nettowert aufgrund der montierten Bereifung; Im Fahrzeuggrundwert
                     ist der Neupreis der Serienbereifung mit 50 % enthalten. 
               
               
                  +/-###########.##
               
               
                  
               
            
            
               
                  vxs:TiresUnmountedValue
               
               
                  Decimal
               
               
                  Wertanpassung (Nettowert) aufgrund der unmontierten Reifen
               
               
                  +###########.##
               
               
                  
               
            
            
               
                  vxs:AccidentDamage¹
               
               
                  String
               
               
                  Unfallkennzeichen (nur beschreibend, ohne Einfluss auf Wertkorrektur)
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  vxs:NumberOfOwnersN
               
               
                  String
               
               
                  Anzahl der Halter
               
               
                  [0 - 15, unknown]
               
               
                  
               
            
            
               
                  vxs:OwnerCorrectionPerc
               
               
                  Decimal
               
               
                  Wertkorrektur aufgrund der Anzahl der Vorbesitzer in Prozent 
               
               
                  numerisch [0-15]
               
               
                  
               
            
            
               
                  vxs:ConditionCorrectionFactorPerc
               
               
                  Decimal
               
               
                  Zustandswertkorrektur in Prozent auf den Händlerverkaufspreis.
               
               
                  numerisch [70-130]
               
               
                  
               
            
            
               
                  vxs:RepairCosts
               
               
                  Decimal
               
               
                  Kosten noch durchzuführender Reparaturen (Nettowert)
               
               
                  +#######.##
               
               
                  
               
            
            
               
                  vxs:NextGeneralInspection
                  
               
               
                  Date
               
               
                  Nächste Hauptuntersuchung
               
               
                  YYYY-MM
               
               
                  
               
            
            
               
                  vxs:NextExhaustInspection
                  
               
               
                  Date
               
               
                  Nächste Abgasuntersuchung (nicht für Deutschland verfügbar)
               
               
                  YYYY-MM
               
               
                  
               
            
            
               
                  vxs:NextServiceDate
               
               
                  Date
               
               
                  Nächster Kundendiensttermin
               
               
                  YYYY-MM-DD
               
               
                  
               
            
            
               
                  vxs:LastServiceDate
               
               
                  Date
               
               
                  Letzter Kundendiensttermin
               
               
                  YYYY-MM-DD
               
               
                  
               
            
            
               
                  vxs:NextServiceMileage
               
               
                  Integer
               
               
                  Nächster Kundendienst bei Kilometerstand
               
               
                  numerisch
               
               
                  
               
            
            
               
                  vxs:LastServiceMileage
               
               
                  Integer
               
               
                  Letzter Kundendienst bei Kilometerstand
               
               
                  numerisch
               
               
                  
               
            
            
               
                  vxs:DamageAmount
               
               
                  Decimal
               
               
                  Schadenhöhe
               
               
                  +#########.###
               
               
                  
               
            
            
               
                  vxs:ConditionComment
               
               
                  String
               
               
                  Kommentar zum Zustand
               
               
                  
               
               
                  
               
            
            
               
                  vxs:ConditionCorrectionDescription
               
               
                  String
               
               
                  Grund des Anpassungsfaktors; Voraussetzung: Der Parameter ConditionCorrectionFactorPerc muss gesetzt sein
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:TradingActivity
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:PriceCalculation
               
               
                  PriceCalculation
               
               
                  Preiskalkulation
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:PriceCalculation
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:NominalDaysOnLot 
               
               
                  Integer
               
               
                  Benutzerwert Anzahl der Standtage
               
               
                  numerisch [0-9999]
               
               
                  
               
            
            
               
                  vxs:ActualRepairCosts
               
               
                  Decimal
               
               
                  Aktuelle Instandsetzungskosten(noch nicht verfügbar)
               
               
                  
               
               
                  
               
            
         
      
   
   Variante mit unvollständiger Fahrzeugidentifikation
   Request createValuation
   
      
         
            
               
                  Name
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  contractType
               
               
                  String
               
               
                  Auftragstypen
               
               
                  bundle_valuation
               
               
                  X
               
            
            
               
                  networkType
               
               
                  String
               
               
                  Netzwerktypen
               
               
                  DAT
                  FHD
               
               
                  X
               
            
            
               
                  vxs:Dossier
               
               
                  Dossier
               
               
                  Element das die Vehicle eXchange Struktur (VXS) beinhaltet
               
               
                  
               
               
                  X
               
            
            
               
                  Coverage¹
                  
                     
                        Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.
                        
                        
                           
                              
                                 
                                    
                                       Wert
                                    
                                    
                                       Datenumfang
                                    
                                 
                                 
                                    
                                       MARKETPLACEEXPORT
                                    
                                    
                                       Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO).
                                    
                                 
                                 
                                    
                                       EXTENDEDBYTRADING
                                    
                                    
                                       Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO).
                                    
                                 
                                 
                                    
                                       COMPLETE
                                    
                                    
                                       Defaultwert;  Standard Datenumfang für die Datenrückgabe
                                    
                                 
                                 
                                    
                                       NOVALUATIONRESULT
                                    
                                    
                                       Datenrückgabe ohne die Unterelemente Valuation und VAT
                                    
                                 
                                 
                                    
                                       ENRICHED
                                    
                                    
                                       Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen
                                    
                                 
                                 
                                    
                                       BASE
                                    
                                    
                                       Datenrückgabe ganz ohne Benennungen
                                    
                                 
                                 
                                    
                                       SIMPLE
                                    
                                    
                                       Bei diesem Wert entfallen zusätzlich bestimmte  Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder,  RegistratinData, Engine, Equipment oder TechInfo.
                                    
                                 
                                 
                                    
                                       NONE
                                    
                                    
                                       Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. 
                                    
                                 
                              
                           
                        
                     
                  
               
               
                  String
               
               
                  Begrenzte Datenausgabe für unvollständiger Fahrzeugidentifikation
               
               
                  NOVALUATIONRESULTNONE
               
               
                  X
               
            
            
               
                  templateId
               
               
                  Long
               
               
                  ID der Auftragsvorlage
               
               
                  
               
               
                  
               
            
            
               
                  templateData
               
               
                  HashMap<String, Object>
               
               
                  Benutzerdefinierte Vorlagedaten
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:Dossier
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:Language¹
               
               
                  String
               
               
                  Sprachkürzel
                  Pflicht für createValuationN
               
               
                  Sprachkürzel (Language) 
                  siehe Popup-Fenster
               
               
                  bedingt
               
            
            
               
                  vxs:Name
               
               
                  String
               
               
                  Bezeichnung des Vorgangs
               
               
                  
               
               
                  
               
            
            
               
                  vxs:DossierType
               
               
                  String
               
               
                  Typ des anzulegenden Vorgangs
               
               
                  bundlePro 
               
               
                  
               
            
            
               
                  vxs:Vehicle
               
               
                  Vehicle
               
               
                  Enthält Fahrzeugdaten als Unterelemente
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:Vehicle
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:Country¹
               
               
                  String
               
               
                  Landeskürzel des betreffenden Datenlands
               
               
                  ISO 3166 ALPHA-2 weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  vxs:DatECode
               
               
                  String
               
               
                  DAT €uropa-Code®
               
               
                  15-stellig
               
               
                  
               
            
            
               
                  vxs:Container
               
               
                  String
               
               
                  Marktindex 
               
               
                  [Landessetzung, 2-stellig][Nummer des Marktindex, 3-stellig]
               
               
                  
               
            
            
               
                  vxs:ConstructionTime¹
               
               
                  Integer
               
               
                  Bauzeit
               
               
                  4-stellig numerisch
               
               
                  
               
            
            
               
                  vxs:MileageEstimated
               
               
                  Integer
               
               
                  Kilometerstand
               
               
                  numerisch
               
               
                  
               
            
            
               
                  vxs:InitialRegistration
               
               
                  Date
               
               
                  Erstzulassungsdatum
               
               
                  YYYY-MM-DD
               
               
                  
               
            
            
               
                  vxs:VehicleIdentNumber
               
               
                  String
               
               
                  Fahrzeugidentifikationsnummer (Fahrgestellnummer); (VIN)
               
               
                  17-stellig
               
               
                  
               
            
            
               
                  vxs:RegistrationData
               
               
                  RegistrationData
               
               
                  Enthält die Zulassungsdaten
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:RegistrationData
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:LicenseNumber
               
               
                  String
               
               
                  amtliches Kennzeichen
               
               
                  
               
               
                  
               
            
         
      
   
   ¹ weitere Infos siehe Popup-Fenster
