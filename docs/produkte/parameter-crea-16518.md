---
title: "Parameter createDossierN unvollstaendiges Aktenzeichen"
topic_id: "16518"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Unvollständiges Aktenzeichen > Verwalten von unvollstaendigen Aktenzeichen > Erstellen eines neuen unvollstaendigen Aktenzeichens > Parameter createDossierN unvollstaendiges Aktenzeichen"
---

# Parameter createDossierN unvollstaendiges Aktenzeichen

Request createDossierN
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:Dossier
               
               
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
               
               
                  NOVALUATIONRESULT oder NONE
               
               
                  X
               
            
            
               
                  Save
               
               
                  String
               
               
                  Speicherkennzeichen wird nur benötigt, falls der Vorgang nicht gespeichert werden
                     soll. 
               
               
                  truefalseDefaultwert ist true
               
               
                  
               
            
         
      
   
   Element vxs:Dossier
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
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
                                    
                                 
                              
                           
                        
                        
                     
                  
               
               
                  X
               
            
            
               
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
               
               
                  ISO 3166 ALPHA-2weitere Infos siehe Popup-Fenster
               
               
                  X
               
            
            
               
                  vxs:Name
               
               
                  String
               
               
                  Bezeichnung des Vorgangs
               
               
                  
               
               
                  
               
            
            
               
                  vxs:Vehicle
               
               
                  Vehicle
               
               
                  Enthält Fahrzeugdaten als Unterelemente
               
               
                  
               
               
                  X
               
            
         
      
   
   Element vxs:Vehicle
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  vxs:Country²
               
               
                  String
               
               
                  Landeskürzel des betreffenden Datenlands
               
               
                  ISO 3166 ALPHA-2weitere Infos siehe Popup-Fenster
               
               
                  X
               
            
            
               
                  vxs:DatECode
               
               
                  String
               
               
                  DAT €uropa-Code®
               
               
                  15-stellig
               
               
                  
               
            
            
               
                  vxs:Container
               
               
                  String
               
               
                  Marktindex
               
               
                  [Landessetzung, 2-stellig][Nummer des Marktindex, 3-stellig]
               
               
                  
               
            
            
               
                  vxs:ConstructionTime
               
               
                  Integer
               
               
                  Bauzeit
               
               
                  4-stellig numerisch 
               
               
                  
               
            
            
               
                  vxs:MileageEstimated
               
               
                  Integer
               
               
                  Kilometerstand Es ist nur eine Vorgabe für die Laufleistung/Betriebsstunden zulässig
               
               
                  numerisch
               
               
                  
               
            
            
               
                  vxs:MileageType
               
               
                  String
               
               
                  Art des Kilometerstands 
               
               
                  Estimated (Standard), Indicated, FromTacho
               
               
                  
               
            
            
               
                  vxs:InitialRegistration
               
               
                  Date
               
               
                  Erstzulassungsdatum
               
               
                  YYYY-MM-DD
               
               
                  
               
            
            
               
                  vxs:VehicleIdentNumber
               
               
                  String
               
               
                  Fahrzeugidentifikationsnummer (Fahrgestellnummer); 
               
               
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
               
               
                  
               
               
                  
               
            
         
      
   
   
   
   ² siehe Popup Fenster
