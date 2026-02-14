---
title: "Parameter changeDossierN"
topic_id: "15027"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Aendern eines Vorgangs > Parameter changeDossierN"
---

# Parameter changeDossierN

Request changeDossierN
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  Dossier
               
               
                  Dossier
               
               
                  VXS-Einstiegselement, enthält sämtliche Eingabedaten zum Vorgang
               
               
                  
               
               
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
               
               
                  definiert die Datenausgabemenge 
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:Dossier
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:DossierId
               
               
                  Integer
               
               
                  Eindeutige Vorgangskennung
               
               
                  numerisch
               
               
                  X
               
            
            
               
                  vxs:Language
               
               
                  String
               
               
                  Sprachkürzel 
               
               
                  Sprachkürzel (Language)²
                  
                     
                        
                           
                              
                                 
                                    
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
                                    
                                 
                              
                           
                        
                        
                     
                  
               
               
                  
               
            
            
               
                  vxs:Name
               
               
                  String
               
               
                  Bezeichnung des Vorgangs
               
               
                  
               
               
                  
               
            
            
               
                  vxs:ExternalId
               
               
                  String
               
               
                  Identifikation im Fremdsystem
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Vehicle
               
               
                  Vehicle
               
               
                  Enthält Fahrzeugarten als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  vxs:VAT
               
               
                  VAT
               
               
                  Enthält Steuerdaten als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Valuation
               
               
                  Valuation
               
               
                  Enthält bewertungsrelevante Daten als Unterelemente
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:Vehicle
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:Country²
                  
                     
                        
                           
                              
                                 
                                    
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
               
               
                  
               
            
            
               
                  vxs:DatECode
               
               
                  String
               
               
                  DAT €uropa-Code® .Nur Pflicht bei Fahrzeugneuidentifikation
               
               
                  15-stellig
               
               
                  bedingt
               
            
            
               
                  vxs:Container
               
               
                  String
               
               
                  Marktindex. Nur Pflicht bei Fahrzeugneuidentifikation
               
               
                  [Landessetzung, 2-stellig][Nummer des Marktindex, 3-stellig]
               
               
                  bedingt
               
            
            
               
                  vxs:ConstructionTime
               
               
                  Integer
               
               
                  Bauzeit² Nur Pflicht bei Fahrzeugneuidentifikation
               
               
                  4-stellig numerisch, weitere Infos siehe Popup-Fenster
               
               
                  bedingt
               
            
            
               
                  vxs:MileageEstimated
               
               
                  Integer
               
               
                  Kilometerstand.Pflicht für Gebrauchtfahrzeuge.
               
               
                  numerisch
               
               
                  bedingt
               
            
            
               
                  vxs:MileageType
               
               
                  String
               
               
                  Art des Kilometerstands
               
               
                  Estimated (Standard), Indicated, FromTacho
               
               
                  
               
            
            
               
                  vxs:InitialRegistration²
                  
                     
                        Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex darf nicht
                           größer als 1 Jahr sein. In der Fahrzeugbewertung kann sonst kein Wert ermittelt werden.
                           
                     
                  
               
               
                  Date
               
               
                  Erstzulassungsdatum.Nur Pflicht, wenn Fahrzeugstatus von Neufahrzeug auf Gebrauchtfahrzeug geändert wird
               
               
                  YYYY-MM-DD
                  weitere Infos siehe Popup-Fenster
               
               
                  bedingt
               
            
            
               
                  vxs:VehicleIdentNumber
               
               
                  String
               
               
                  Fahrzeugidentifikationsnummer (Fahrgestellnummer) 
               
               
                  17-stellig
               
               
                  
               
            
            
               
                  vxs:TechInfo
               
               
                  TechInfo
               
               
                  Enthält technische Daten des Fahrzeugs als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  vxs:RegistrationData
               
               
                  RegistrationData
               
               
                  Enthält die Zulassungsdaten
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Equipment
               
               
                  Equipment
               
               
                  Enthält die Ausstattungslisten als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  vxs:UpperBodies
               
               
                  UpperBodies
               
               
                  Enthält die Aufbauten als  Unterelemente. Falls das Element UpperBodies angegeben wird, muss die Liste vollständig angegeben werden, da sie identisch übernommen
                     wird; nur für Fahrzeugart LKW und Transporter verfügbar
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Tires
               
               
                  Tires
               
               
                  Dieses Element beinhaltet die Achsendaten
               
               
                  
               
               
                  
               
            
            
               
                  vxs:VehicleTypeNameN
               
               
                  String
               
               
                  Fahrzeugart
               
               
                  
               
               
                  
               
            
            
               
                  vxs:ManufacturerName
               
               
                  String
               
               
                  Herstellerbezeichnung
               
               
                  
               
               
                  
               
            
            
               
                  vxs:BaseModelName
               
               
                  String
               
               
                  Basistyp
               
               
                  
               
               
                  
               
            
            
               
                  vxs:SubModelName
               
               
                  String
               
               
                  Untertyp
               
               
                  
               
               
                  
               
            
            
               
                  vxs:ContainerNameN
               
               
                  String
               
               
                  Name/Benennung des Container
               
               
                  
               
               
                  
               
            
         
      
   
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
               
               
                  Decimal
               
               
                  Kraftstoffverbrauch innerorts
               
               
                  
               
               
                  
               
            
            
               
                  vxs:ConsumptionOutOfTown origin="user"
               
               
                  Decimal
               
               
                  Kraftstoffverbrauch außerorts
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Consumption origin="user"
               
               
                  Decimal
               
               
                  Kraftstoffverbrauch kombiniert
               
               
                  
               
               
                  
               
            
            
               
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
   
      
         Element vxs:Tires
         
            
               
                  
                     
                        Parameter
                     
                     
                        Datentyp
                     
                     
                        Beschreibung
                     
                     
                        Schreibweise
                     
                     
                        Pflicht
                     
                  
                  
                     
                        vxs:Axles
                     
                     
                        Axles
                     
                     
                        Enthält die Achsendaten als Unterlemente. Bei freien Aktenzeichen können Fahrzeugen mit nur einer montierten Achse angelegt werden.
                     
                     
                        
                     
                     
                        
                     
                  
               
            
         
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
                     
                     
                        mounted, unmounted, spare wheel
                     
                     
                        X
                     
                  
                  
                     
                        vxs:NrOfTires
                     
                     
                        Integer
                     
                     
                        Reifenanzahl, Werte montierte Reifen: PKW, beliebige Achse: 2; Transporter und LKW, erste Achse: 2, weitere Achsen: 2 oder 4; Kraftrad, erste Achse:1 oder 2, weitere Achsen: 1. Werte unmontierte Reifen oder Reserverad: 1.
                     
                     
                        1, 2, 4
                     
                     
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
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:TireOriginalTreadDepthN
                     
                     
                        Decimal
                     
                     
                        Reifenprofiltiefe.
                     
                     
                        [0,0 - 999,0]
                     
                     
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
                        
                     
                     
                        Profiltiefe in Millimeter; Pflicht bei NrOfTires = 1 für links außen und bei NrOfTires = 2 für links außen und rechts außen und bei NrOfTires = 4 für links außen, links innen, rechts außen und rechts innen.
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
                     
                     
                        true = manueller Eintragfalse = kein manueller Eintrag
                     
                     
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
                     mit Differenzbesteuerung und bei Neufahrzeugen mit Regelbesteuerung bewertet. Für
                     Neufahrzeuge ist nur die Regelbesteuerung zulässig.
               
               
                  R, REGULAR = Regelbesteuerung; D, DIFFERENCE = Differenzbesteuerung
               
               
                  
               
            
         
      
   
   Element vxs:Valuation
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:ValuationType
               
               
                  String
               
               
                  Fahrzeugbewertungsart; Ein Gebrauchtfahrzeug kann nicht mehr in ein Neufahrzeug geändert
                     werden. Der umgekehrte Weg ist möglich, dann müssen jedoch MilageEstimated und InitialRegistration angegeben werden.
               
               
                  VALUATION = Gebrauchtfahrzeug,NEW VEHICLE = Neufahrzeug
               
               
                  
               
            
            
               
                  vxs:DeterminatedDate¹³
               
               
                  Date
               
               
                  Stichtag für die Bewertung
               
               
                  YYYY-MM-DD
               
               
                  
               
            
            
               
                  Version
               
               
                  String
               
               
                  Versionsangabe für das neue Verfahren, max. 4 Zeichen
               
               
                  V1.1
               
               
                  
               
            
            
               
                  Approval
               
               
                  String
               
               
                  Hash für die Freigabe der rückwirkenden Bewertung, für die eine zusätzliche Gebühr
                     erhoben wird.
                  In diesem Fall Pflicht für SilverDAT 3 valuateExpert /valuateExpertPlusPartner 
               
               
                  9660d...317d
               
               
                  bedingt
               
            
            
               
                  vxs:ExtendedMileageCorrection
               
               
                  Boolean
               
               
                  Kennzeichen; seit 04/2015 ohne Auswirkung, da die Berechnung immer mit erweiterter
                     Kilometerkorrektur stattfindet.
               
               
                  
               
               
                  
               
            
            
               
                  vxs:MileageCorr
               
               
                  Decimal
               
               
                  Betrag für Kilometerkorrektur als Nettowert
               
               
                  
               
               
                  
               
            
            
               
                  vxs:InitialRegistrationCorr
               
               
                  Decimal
               
               
                  Betrag für Erstzulassungskorrektur als Nettowert
               
               
                  
               
               
                  
               
            
            
               
                  vxs:EquipmentPrice
               
               
                  Decimal
               
               
                  manuelle Vorgabe des Ausstattungsrestwerts (gesamt) als Nettowert Nicht zulässig in
                     Kombination mit ManualEquipmentOriginalPrice
               
               
                  numerisch, positiv
               
               
                  
               
            
            
               
                  vxs:ManualEquipmentOriginalPrice
               
               
                  Decimal
               
               
                  manuelle Vorgabe eines pauschalen Ausstattungsgesamtpreis in Euro als Nettowert. Nicht
                     zulässig in Kombination mit EquipmentPrice
               
               
                  numerisch, positiv
               
               
                  
               
            
            
               
                  vxs:EquipmentPercentage
               
               
                  Integer
               
               
                  Der pauschale Ausstattungsgesamtpreis kann in zwei Teile aufgeteilt werden, die unterschiedlich
                     abgewertet werden. Beispiel: Paket1, 60%, RW | Paket2, T4. Mit diesem Wert legen Sie
                     den ersten prozentualen Anteil fest. 
               
               
                  numerisch [1 - 100]
               
               
                  
               
            
            
               
                  vxs:EquipmentDecreaseType²
               
               
                  String
               
               
                  Abwertungsart für den ersten  Anteil
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  vxs:EquipmentDecreaseTypeRemaining²
               
               
                  String
               
               
                  Abwertungsart für den restlichen Anteil
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  vxs:Condition³
               
               
                  Condition
               
               
                  Enthält Zustandsdaten als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  vxs:AdditionalManualMileageCorr (noch nicht implement.)
               
               
                  Decimal
               
               
                  Manueller Korrekturwert bei Fahrzeugbewertungen mit einer Laufleistung unter/über
                     der DAT-Richtlinie. Pflicht in diesem Fall. 
               
               
                  numerisch
               
               
                  bedingt
               
            
            
               
                  vxs:Forecasts¹
               
               
                  Forecasts
               
               
                  nur bei aktueller Bewertung möglich/ausgewertet; Enthält 0 bis n Positionen mit Restwertprognosedaten
                     (vxs:Forecast). 
               
               
                  
               
               
                  
               
            
            
               
                  vxs:PrognosisDate
               
               
                  Date
               
               
                  Zukunftsprognosedatum
               
               
                  gültig nur ab aktuellem Datum 
               
               
                  
               
            
            
               
                  vxs:PrognosisMileageUser
               
               
                  Decimal
               
               
                  Laufleistung für die Zukunftsprognose
               
               
                  
               
               
                  
               
            
            
               
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
               
               
                  
               
               
                  
               
            
            
               
                  vxs:LicenseNumberType³
               
               
                  String
               
               
                  Art des amtliches Kennzeichens
               
               
                  
               
               
                  
               
            
            
               
                  vxs:KbaCode
               
               
                  String
               
               
                  KbaCode, Bitte geben Sie nur ein KbaCode an
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:Equipment
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:SpecialEquipment
               
               
                  EquipSequence
               
               
                  Sonderausstattungen Enthält 0 bis n Positionen vxs:EquipmentPosition als Unterlemente. Falls eine Sonderausstattung geändert werden soll, dann muss die
                     gesamte Ausstattungsliste übergeben werden.
               
               
                  
               
               
                  
               
            
            
               
                  vxs:AdditionalEquipment
               
               
                  EquipSequence
               
               
                  Zusatzausstattungen Enthält 0 bis n Positionen vxs:EquipmentPosition als Unterlemente. Falls eine Zusatzausstattung geändert werden soll, dann muss die
                     gesamte Ausstattungsliste übergeben werden.
               
               
                  
               
               
                  
               
            
         
      
   
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
               
               
                  Name/Beschreibung der Ausstattung. Nur möglich bei Zusatzausstattung
               
               
                  
               
               
                  
               
            
            
               
                  vxs:DecreaseType²
               
               
                  String
               
               
                  AbwertungsartEine Vorgabe wird nur benötigt, falls Sie die DAT-Standardvorgabe überschreiben möchten.
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  vxs:PercentageOfBasePrice³
               
               
                  Integer
               
               
                  Prozentuale Abwertung der Sonderausstattung. Pflicht, wenn das Element DecreaseType mit dem Wert Percentage belegt wird (nur für SilverDAT valuateExpert verfügbar)
               
               
                  [-25 bis 25]
               
               
                  bedingt
               
            
            
               
                  vxs:InstallDate
               
               
                  Date
               
               
                  Einbaudatum Nur möglich bei Zusatzausstattung 
               
               
                  YYYY-MM-DD
               
               
                  
               
            
            
               
                  vxs:OriginalPrice
               
               
                  Decimal
               
               
                  Neupreis als Nettowert. Nur möglich bei ZusatzausstattungWird nur in den Neupreis der gesamten Ausstattung gerechnet, wenn InstallDate vor dem Erstzulassungsdatum liegt oder nicht gesetzt ist
               
               
                  
               
               
                  
               
            
            
               
                  vxs:OriginalPriceGross
               
               
                  Decimal
               
               
                  Neupreis als Bruttowert. Nur möglich bei ZusatzausstattungWird nur in den Neupreis der gesamten Ausstattung gerechnet, wenn InstallDate vor dem Erstzulassungsdatum liegt oder nicht gesetzt ist
               
               
                  
               
               
                  
               
            
            
               
                  vxs:ResidualValue
               
               
                  Decimal
               
               
                  Restwert als Nettowert
               
               
                  
               
               
                  
               
            
         
      
   
   Element vxs:UpperBody²
   
      
         Element vxs:UpperBody
         
            
               
                  
                     
                        Parameter
                     
                     
                        Datentyp
                     
                     
                        Beschreibung
                     
                     
                        Schreibweise
                     
                     
                        Pflicht
                     
                  
                  
                     
                        vxs:UpperBodyType
                     
                     
                        Integer
                     
                     
                        Nummer der Aufbauart
                     
                     
                        numerisch
                     
                     
                        X
                     
                  
                  
                     
                        vxs:Manufacturer
                     
                     
                        Integer
                     
                     
                        Nummer des Herstellers (derzeit nur 999 möglich)
                     
                     
                        numerisch
                     
                     
                        
                     
                  
                  
                     
                        vxs:MainModel
                     
                     
                        Integer
                     
                     
                        Nummer des Haupttyps
                     
                     
                        numerisch
                     
                     
                        X
                     
                  
                  
                     
                        vxs:SubModel
                     
                     
                        Integer
                     
                     
                        Nummer des Untertyps
                     
                     
                        numerisch
                     
                     
                        X
                     
                  
                  
                     
                        vxs:UpperBodyTypeName
                     
                     
                        String
                     
                     
                        Bezeichnung der Aufbauart
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:ManufacturerName
                     
                     
                        String
                     
                     
                        Bezeichnung des Aufbauherstellers
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:MainModelName
                     
                     
                        String
                     
                     
                        Typbezeichnung
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:SubModelName
                     
                     
                        String
                     
                     
                        Untertypbezeichnung
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:InitialRegistration
                     
                     
                        Date
                     
                     
                        Erstzulassung
                     
                     
                        YYYY-MM-DD
                     
                     
                        
                     
                  
                  
                     
                        vxs:IdentificationNumber
                     
                     
                        String
                     
                     
                        Identifizierungsnummer
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:UpperBodyColor
                     
                     
                        String
                     
                     
                        Aufbaufarbe
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:PaintLabelDescription
                     
                     
                        String
                     
                     
                        Beschreibung von Lackierung und Beschriftung
                     
                     
                        maximal 200 Zeichen
                     
                     
                        
                     
                  
                  
                     
                        vxs:OriginalPrice
                     
                     
                        Decimal
                     
                     
                        Neupreis (Netto)
                     
                     
                        maximal 9 Zeichen (XXXXXXXXX.XX)
                     
                     
                        
                     
                  
                  
                     
                        vxs:OriginalPriceGross
                     
                     
                        Decimal
                     
                     
                        Neupreis (Brutto)
                     
                     
                        maximal 9 Zeichen (XXXXXXXXX.XX)
                     
                     
                        
                     
                  
                  
                     
                        vxs:GeneralCondition
                     
                     
                        Decimal
                     
                     
                        Erhaltungszustand
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:BasePrice
                     
                     
                        Decimal
                     
                     
                        Basiswert (Netto)
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:SalesPrice
                     
                     
                        Decimal
                     
                     
                        Verkaufspreis (Netto)
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:TechInfo
                     
                     
                        TechInfo
                     
                     
                        Enthält technische Daten als Unterelemente
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:Equipment
                     
                     
                        Equipment
                     
                     
                        Enthält Ausstattungslisten als Unterelemente entsprechend Vehicle
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:Condition
                     
                     
                        Condition
                     
                     
                        Enthält Zustandsdaten als Unterelemente; Zulässig sind: IncreaseInValue, DecreaseInValue, AccidentDamage, RepairCosts, ConditionCorrectionFactorPerc
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:CoolingUnit
                     
                     
                        CoolingUnit
                     
                     
                        nur bei Aufbauten mit Kühlfunktion (Aufbauart 21 und 22) möglich; Kühlaggregat; Enthält
                           Daten als Unterelemente
                     
                     
                        
                     
                     
                        
                     
                  
               
            
         
         
         
      
   
   Element vxs:TechInfo²
   
      
         Element vxs:TechInfo
         
            
               
                  
                     
                        Parameter
                     
                     
                        Datentyp
                     
                     
                        Beschreibung
                     
                     
                        Schreibweise
                     
                     
                        Pflicht
                     
                  
                  
                     
                        vxs:UpperBodyMaterial
                     
                     
                        String
                     
                     
                        Aufbaumaterial
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:LoadingLength
                     
                     
                        Integer
                     
                     
                        Länge in mm
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:LoadingWidth
                     
                     
                        Integer
                     
                     
                        Breite in mm
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:LoadingHeight
                     
                     
                        Integer
                     
                     
                        Höhe in mm
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:LoadingSpace
                     
                     
                        Integer
                     
                     
                        Fassungsvermögen in m³
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:Payload
                     
                     
                        Integer
                     
                     
                        Nutzlast in kg
                     
                     
                        
                     
                     
                        
                     
                  
               
            
         
         
         
      
   
   Element vxs:CoolingUnit²
   
      
         Element vxs:CoolingUnit
         
            
               
                  
                     
                        Parameter
                     
                     
                        Datentyp
                     
                     
                        Beschreibung
                     
                     
                        Schreibweise
                     
                     
                        Pflicht
                     
                  
                  
                     
                        vxs:Manufacturer
                     
                     
                        Integer
                     
                     
                        Nummer des Herstellers
                     
                     
                        numerisch
                     
                     
                        X
                     
                  
                  
                     
                        vxs:MainModel
                     
                     
                        Integer
                     
                     
                        Nummer des Modells
                     
                     
                        numerisch
                     
                     
                        X
                     
                  
                  
                     
                        vxs: ManufacturerName
                     
                     
                        String
                     
                     
                        Bezeichnung des Herstellers
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:MainModelName
                     
                     
                        String
                     
                     
                        Modellbezeichnung
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:InitialRegistration
                     
                     
                        Date
                     
                     
                        Erstzulassung
                     
                     
                        YYYY-MM-DD
                     
                     
                        X
                     
                  
                  
                     
                        vxs:OriginalPrice
                     
                     
                        Decimal
                     
                     
                        Neupreis als Nettowert
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:GeneralCondition
                     
                     
                        Decimal
                     
                     
                        Erhaltungszustand
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:SalesPrice
                     
                     
                        Decimal
                     
                     
                        Verkaufspreis als Nettowert
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:DriveType
                     
                     
                        String
                     
                     
                        Antriebsart; Kommaseparierte Liste, Trennzeichen=;
                     
                     
                        gasoline engine = Benzinmotor; diesel engine = Dieselmotor; electric motor = Elektromotor;  generator = Generator; hydraulics = Hydraulik; compressor = Kompressor; vehicle engine = Lkw-Motor; power connection = Netzanschluss
                     
                     
                        
                     
                  
                  
                     
                        vxs:Usage
                     
                     
                        String
                     
                     
                        Verwendung; Kommaseparierte Liste, Trennzeichen=;
                     
                     
                        heating = heizen; cooling = kühlen
                     
                     
                        
                     
                  
                  
                     
                        vxs:MinRecommendedBodyLength
                     
                     
                        Integer
                     
                     
                        Minimale empfohlene Aufbaulänge in mm
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:MaxRecommendedBodyLength
                     
                     
                        Integer
                     
                     
                        Maximale empfohlene Aufbaulänge in mm
                     
                     
                        
                     
                     
                        
                     
                  
               
            
         
         
      
   
   Element vxs:Condition²
   
      
         Element vxs:Condition 
         
            
               
                  
                     
                        Parameter
                     
                     
                        Datentyp
                     
                     
                        Beschreibung
                     
                     
                        Schreibweise
                     
                     
                        Pflicht
                     
                  
                  
                     
                        vxs:IncreaseInValue
                     
                     
                        Decimal
                     
                     
                        Werterhöhung als Geldbetrag  (Netto)
                     
                     
                        +###########.##
                     
                     
                        
                     
                  
                  
                     
                        vxs:DecreaseInValue
                     
                     
                        Decimal
                     
                     
                        Wertminderung als Geldbetrag  (Netto)
                     
                     
                        +###########.##
                     
                     
                        
                     
                  
                  
                     
                        vxs:TiresMountedValue
                     
                     
                        Decimal
                     
                     
                        Wertanpassung aufgrund der montierten Bereifung; Im Fahrzeuggrund- wert ist der Neupreis
                           der Serienbereifung mit 50 % enthalten (Netto) 
                     
                     
                        +/-###########.##
                     
                     
                        
                     
                  
                  
                     
                        vxs:TiresUnmountedValue
                     
                     
                        Decimal
                     
                     
                        Wertanpassung aufgrund der unmontierten Reifen (Netto)
                     
                     
                        +###########.##
                     
                     
                        
                     
                  
                  
                     
                        vxs:AccidentDamage*²
                     
                     
                        String
                     
                     
                        Unfallkennzeichen (nur beschreibend, ohne Einfluss auf Wertkorrektur)
                     
                     
                        weitere Infos siehe Popup-Fenster
                     
                     
                        bedingt
                     
                  
                  
                     
                        vxs:NumberOfOwnersN
                     
                     
                        String
                     
                     
                        Anzahl der Halter
                     
                     
                        [0 - 15, unknown]
                     
                     
                        
                     
                  
                  
                     
                        vxs:NumberOfProprietors
                     
                     
                        String
                     
                     
                        Anzahl der Besitzer
                        (nur für SilverDAT 3 valuateExpertPlusPartner verfügbar)
                     
                     
                        [0 - 15, unknown]
                     
                     
                        
                     
                  
                  
                     
                        vxs:OwnerCorrectionPerc
                     
                     
                        Decimal
                     
                     
                        Wertkorrektur aufgrund der Anzahl der Vorbesitzer in Prozent 
                     
                     
                        Dezimal [0.00 - 15.00]
                     
                     
                        
                     
                  
                  
                     
                        vxs:ConditionCorrectionFactorPerc
                     
                     
                        Decimal
                     
                     
                        Zustandswertkorrektur in Prozent auf den Händlerverkaufspreis.
                     
                     
                        Dezimal [70.00 - 130.00]
                     
                     
                        
                     
                  
                  
                     
                        vxs:RepairCosts
                     
                     
                        Decimal
                     
                     
                        Kosten noch durchzuführender Reparaturen (Nettowert)
                     
                     
                        +#######.##
                     
                     
                        
                     
                  
                  
                     
                        vxs:NextGeneralInspection
                     
                     
                        Date
                     
                     
                        Nächstes Hauptuntersuchungsdatum
                     
                     
                        YYYY-MM-DD
                     
                     
                        
                     
                  
                  
                     
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
                     
                     
                        Nächster Service bei Kilometerstand
                     
                     
                        numerisch
                     
                     
                        
                     
                  
                  
                     
                        vxs:LastServiceMileage
                     
                     
                        Integer
                     
                     
                        Letzter Service bei Kilometerstand
                     
                     
                        numerisch
                     
                     
                        
                     
                  
                  
                     
                        vxs:ConditionComment
                     
                     
                        String
                     
                     
                        Kommentar zum Zustand
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:DamageAmount
                     
                     
                        Integer
                     
                     
                        Schadenhöhe;Vorraussetzung: Der Parameter AccidentDamage muss gesetzt sein.(nur für SilverDAT 3 PRO verfügbar)
                     
                     
                        +#########.##
                     
                     
                        
                     
                  
                  
                     
                        vxs:RepairCostsTradeInMargin
                     
                     
                        Boolean
                     
                     
                        Verkauf im reparierten Zustand
                     
                     
                        true, false
                     
                     
                        
                     
                  
                  
                     
                        vxs:ConditionRegistrationDate
                     
                     
                        Date
                     
                     
                        Datum der letzten Fahrzeuganmeldug
                     
                     
                        YYYY-MM-DD
                     
                     
                        
                     
                  
                  
                     
                        vxs:ConditionDeregistrationDate
                     
                     
                        Date
                     
                     
                        Datum der letzten Fahrzeugabmeldung
                     
                     
                        YYYY-MM-DD
                     
                     
                        
                     
                  
                  
                     
                        vxs:CommentIncreaseInValue
                     
                     
                        String
                     
                     
                        Bemerkung zur Werterhöhung
                     
                     
                        maximal 200 Zeichen
                     
                     
                        
                     
                  
                  
                     
                        vxs:CommentDecreaseInValue
                     
                     
                        String
                     
                     
                        Bemerkung zur Wertminderung
                     
                     
                        maximal 200 Zeichen
                     
                     
                        
                     
                  
                  
                     
                        vxs:ConditionCorrectionDescription
                     
                     
                        String
                     
                     
                        Grund des Anpassungsfaktors; Voraussetzung: Der Parameter ConditionCorrectionFactorPerc muss gesetzt sein
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:CommentRepairCosts³
                     
                     
                        String
                     
                     
                        Kommentar zu den Reperaturkosten
                     
                     
                        
                     
                     
                        
                     
                  
               
            
         
         
      
   
   Element vxs:Forecast²¹
   
      
         Element vxs:Forecast
         
            
               
                  
                     
                        Parameter
                     
                     
                        Datentyp
                     
                     
                        Beschreibung
                     
                     
                        Schreibweise
                     
                     
                        Pflicht
                     
                  
                  
                     
                        vxs:PriceType
                     
                     
                        String
                     
                     
                        Kennzeichen für die Preisangabe EK oder VK; Standardwert ist PURCHASE
                     
                     
                        PURCHASE = EK,SALES = VK
                     
                     
                        
                     
                  
                  
                     
                        vxs:IncludeVat
                     
                     
                        Boolean
                     
                     
                        Kennzeichen für die Mehrwertsteuerangabe (mit oder ohne)
                     
                     
                        true = mitfalse = ohne
                     
                     
                        X
                     
                  
                  
                     
                        vxs:CurveType
                     
                     
                        String
                     
                     
                        Abwertungskurve
                     
                     
                        MINIMUM, MAXIMUM, DEFAULTStandardwert ist DEFAULT
                     
                     
                        
                     
                  
                  
                     
                        vxs:DecreaseType²
                     
                     
                        String
                     
                     
                        Abwertungsart der Ausstattung; Eine Vorgabe wird nur benötigt, falls Sie die DAT-Standardvorgabe
                           überschreiben möchten.
                     
                     
                        weitere Infos siehe Popup-FensterStandardwert ist DEFAULT TABLE
                     
                     
                        
                     
                  
                  
                     
                        vxs:ValueType
                     
                     
                        String
                     
                     
                        Kennzeichen für Wertangabe (EUR, % oder km)
                     
                     
                        MONETARY, PERCENT,  KMStandardwert ist MONETARY
                     
                     
                        
                     
                  
                  
                     
                        vxs:StartType
                     
                     
                        String
                     
                     
                        Kennzeichen für die Angabe des Fahrzeugalters (Gesamt oder ab Bewertungsmonat)
                     
                     
                        INITIAL REGISTRATION, RECENT EVALUATION
                        Standardwert ist INITIAL REGISTRATION
                     
                     
                        
                     
                  
                  
                     
                        vxs:MileageType
                     
                     
                        String
                     
                     
                        Kennzeichen für Laufleistungsangabe (Gesamt oder Laufleistung pro Jahr); Standardwert
                           ist YEAR; Achtung: Wird der Parameter nicht angegeben, wird automatisch der Wert YEAR benutzt, auch wenn im Vorgang TOTAL gespeichert war.
                     
                     
                        TOTAL, YEAR
                     
                     
                        
                     
                  
                  
                     
                        vxs:ConsiderCurrentCondition
                     
                     
                        Boolean
                     
                     
                        Gibt an, ob der aktuelle Fahrzeugzustand in der Restwertprognose berücksichtigt werden
                           soll
                     
                     
                        true = aktuellen Zustand berücksichtigenfalse = aktuellen Zustand nicht berücksichtigenDefaultwert ist false
                     
                     
                        
                     
                  
                  
                     
                        vxs:ForecastItems
                     
                     
                        ForecastItem
                     
                     
                        Enthält 0 bis n Datenpaare bestehend aus Fahrzeugalter und Laufleistung vxs:ForecastItem
                     
                     
                        
                     
                     
                        
                     
                  
               
            
         
         Element vxs:ForecastItem
         
            
               
                  
                     
                        Parameter
                     
                     
                        Datentyp
                     
                     
                        Beschreibung
                     
                     
                        Schreibweise
                     
                     
                        Pflicht
                     
                  
                  
                     
                        vxs:Months
                     
                     
                        Integer
                     
                     
                        Bewertungszeitpunkt in Monaten; Bei StartType = INITIAL REGISTRATION als Gesamtalter angegeben, bei StartType = RECENT EVALUATION relativ zum Bewertungsmonat angegeben. Das Fahrzeug muss zum ersten Bewertungszeitpunkt
                           mindestens 6 Monate alt sein. Das Fahrzeug darf zum letzten Bewertungszeitpunkt höchstens
                           72 Monate alt sein.
                     
                     
                        numerisch
                     
                     
                        X
                     
                  
                  
                     
                        vxs:MileageTotal
                     
                     
                        Integer
                     
                     
                        Gesamtlaufleistung des Fahrzeugs zum zugehörigen Bewertungszeitpunkt. Wird bei MileageType = YEAR ignoriert. Pflicht bei MileageType = TOTAL 
                     
                     
                        numerisch
                     
                     
                        bedingt
                     
                  
                  
                     
                        vxs:MileagePerYear
                     
                     
                        Integer
                     
                     
                        Laufleistung des Fahrzeugs pro Jahr zum zugehörigen Bewertungszeitpunkt. Wird bei
                           MileageType = TOTAL ignoriert. Pflicht bei MileageType = YEAR
                     
                     
                        numerisch
                     
                     
                        bedingt
                     
                  
               
            
         
         
      
   
   Element vxs:ContractData²¹
   
      
         Element vxs:ContractData
         
            
               
                  
                     
                        Parameter
                     
                     
                        Datentyp
                     
                     
                        Beschreibung
                     
                     
                        Schreibweise
                     
                     
                        Pflicht
                     
                  
                  
                     
                        vxs:ContractNumber
                     
                     
                        String
                     
                     
                        Vertragsnummer
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:CustomerNumber
                     
                     
                        String
                     
                     
                        Kundennummer
                     
                     
                        
                     
                     
                        
                     
                  
                  
                     
                        vxs:ContractStartingDate
                     
                     
                        Date
                     
                     
                        Vertragsbeginndatum
                     
                     
                        YYYY-MM-DD
                     
                     
                        
                     
                  
                  
                     
                        vxs:MileageAtContractBegin
                     
                     
                        Integer
                     
                     
                        Laufleistung zum Vertragsbeginn in km
                     
                     
                        numerisch
                     
                     
                        
                     
                  
                  
                     
                        vxs:ContractDurationInMonths
                     
                     
                        Integer
                     
                     
                        Vertragslaufzeit in Monaten 
                     
                     
                        numerisch
                     
                     
                        
                     
                  
                  
                     
                        vxs:ContractMileage
                     
                     
                        Integer
                     
                     
                        Vertragslaufzeit in km
                     
                     
                        numerisch
                     
                     
                        
                     
                  
                  
                     
                        vxs:ContractEndDate
                     
                     
                        Date
                     
                     
                        Vertragsendedatum
                     
                     
                        YYYY-MM-DD
                     
                     
                        
                     
                  
                  
                     
                        vxs:MileageAtContractEnd
                     
                     
                        Integer
                     
                     
                        Laufleistung zum Vertragsende in km
                     
                     
                        numerisch
                     
                     
                        
                     
                  
               
            
         
         
      
   
   
   ¹nur für SilverDAT 3 valuateFinance verfügbar
   ² siehe Popup Fenster
   ³ nur für SilverDAT 3 valuateExpert /valuateExpertPlusPartner verfügbar
