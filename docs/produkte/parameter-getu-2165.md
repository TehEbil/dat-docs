---
title: "Parameter getUsedVehicleForecast"
topic_id: "2165"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standard Restwertprognose Gebrauchtfahrzeuge > Parameter getUsedVehicleForecast"
---

# Parameter getUsedVehicleForecast

Element request
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  locale
               
               
                  Locale
               
               
                  
               
               
                  Beispiel: <Locale country="DE" datCountryIndicator="DE" language="de"/>
               
               
                  ISO 3166 ALPHA-2: country, datCountryIndicator
               
               
                  X
               
            
            
               
                  name
               
               
                  String
               
               
                  
               
               
                  Bezeichnung des Vorgangs 
               
               
                  
               
               
                  
               
            
            
               
                  vin
               
               
                  String
               
               
                  
               
               
                  Fahrzeugidentifikationsnummer (Fahrgestellnummer)
               
               
                  17-stellig
               
               
                  
               
            
            
               
                  datECode
               
               
                  String
               
               
                  
               
               
                  DAT €uropa-Code®
               
               
                  15stellig, numerisch
               
               
                  X
               
            
            
               
                  container
               
               
                  String
               
               
                  
               
               
                  Marktindex
               
               
                  [Landessetzung, 2stellig][Nummer des Marktindex, 3stellig]
               
               
                  X
               
            
            
               
                  constructionTimeFrom
               
               
                  Integer
               
               
                  
               
               
                  Bauzeit von; in DAT-Notation (als Filter für die Rückgabe)
               
               
                  [4stellig numerisch]
               
               
                  
               
            
            
               
                  constructionTimeTo
               
               
                  Integer
               
               
                  
               
               
                  Bauzeit bis; in DAT-Notation (schränkt die Rückgabe ein)
               
               
                  [4stellig numerisch]
               
               
                  
               
            
            
               
                  constructionTime
               
               
                  Integer
               
               
                  
               
               
                  Bauzeit in DAT-Notation; eine Berechnungsmöglichkeit finden Sie im Glossar
               
               
                  [4stellig numerisch]
               
               
                  X
               
            
            
               
                  save
               
               
                  String
               
               
                  
               
               
                  Speicherkennzeichen;
               
               
                  truefalse
               
               
                  X
               
            
            
               
                  coverage
                  
                     
                        Mit dem Parameter coverage steuern Sie den Datenumfang der zurückgegeben werden soll.
                        
                        
                           
                              
                                 
                                    
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
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  mileage
               
               
                  Long
               
               
                  
               
               
                  Kilometerangabe
               
               
                  numerisch
               
               
                  X
               
            
            
               
                  registrationDate
               
               
                  Date
               
               
                  
               
               
                  Erstzulassung
               
               
                  JJJJ-MM-DD
               
               
                  X
               
            
            
               
                  restriction
               
               
                  String
               
               
                  
               
               
                  Filter zur Einschränkung der Ausgabedaten, Einschränkung auf "nur FI Fahrzeuge", nur
                     "GS Fahrzeuge", "alle Fahrzeuge"
               
               
                  derzeit nur APPRAISAL
               
               
                  X
               
            
            
               
                  equipment
               
               
                  equipment
               
               
                  
               
               
                  Enthält Ausstattungselemente als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  curveType
               
               
                  String
               
               
                  
               
               
                  Kurvenart; 3 Werte zur Auswahl: Minimal, nach DAT oder Maximal
               
               
                  MINIMUMDATMAXIMUM
               
               
                  X
               
            
            
               
                  decreaseType
               
               
                  String
               
               
                  
               
               
                  Abwertungsart 
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  X
               
            
            
               
                  priceType
               
               
                  String
               
               
                  
               
               
                  Einkaufs- oder Verkaufspreis
               
               
                  SALESPRICE - VK; PURCHASEPRICE - EK
               
               
                  X
               
            
            
               
                  IncludeVat
               
               
                  String
               
               
                  
               
               
                  mit oder ohne Mehrwertsteuerangabe
               
               
                  true,false
               
               
                  X
               
            
            
               
                  ValueType
               
               
                  String
               
               
                  
               
               
                  Form der Wertrückgabe
               
               
                  MONETARY -  Beträge in Euro; MILEAGE - Kilometer-Laufleistung;PERCENTAGE -in Prozent
               
               
                  X
               
            
            
               
                  ExternalId
               
               
                  String
               
               
                  
               
               
                  Identifikation im Fremdsystem
               
               
                  
               
               
                  
               
            
            
               
                  forecastItems
               
               
                  forecastItems
               
               
                  
               
               
                  Enthält eine Liste mit Restwertprognose-Elementen
               
               
                  
               
               
                  X
               
            
            
               
                  regionNo
               
               
                  Integer
               
               
                  
               
               
                  Postleitzahl
               
               
                  numerisch
               
               
                  
               
            
            
               
                  mileageType  
               
               
                  String
               
               
                  mileagePerYear, mileageTotal
               
               
                  Angabe, der zu verwendenden Laufleistungsangabe; mögliche Werte:YEAR - der Wert aus mileagePerYear wird verwendet (DEFAULT).TOTAL -  der Wert aus mileageTotal wird verwendet. 
               
               
                  YEAR (default); TOTAL
               
               
                  
               
            
            
               
                  considerCurrentCondition
               
               
                  Boolean
               
               
                  
               
               
                  Gibt an, ob der aktuelle Fahrzeugzustand in der Restwertprognose berücksichtigt werden
                     soll
               
               
                  true = aktuellen Zustand berücksichtigenfalse = aktuellen Zustand nicht berücksichtigenDefaultwert ist false
               
               
                  
               
            
            
               
                  condition
               
               
                  condition
               
               
                  ermöglicht eine genauere Zustandsbewertung. Beinhaltet noch die folgenden Parameter,
                     um eine exaktere Wertkorrektur durchführen zu können.
               
               
                  
               
               
                  
               
               
                  
               
            
            
               
                  extendedMileageCorrection
               
               
                  String
               
               
                  
               
               
                  Indikator, seit Mai 2015 ohne Wirkung, da die Bewertung immer mit erweiterter Meilenzahl-Korrektur
                     betrieben wird
               
               
                  
               
               
                  
               
            
            
               
                  licenseNumber
               
               
                  String
               
               
                  
               
               
                  Amtliches Kennzeichen
               
               
                  12-stellig
               
               
                  
               
            
         
      
   
   Element equipment 
   
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  equipmentPosition
               
               
                  equipmentPosition
               
               
                  
               
               
                  DAT Ausstattung; 0-n Ausstattungen können übergeben werden
               
               
                  -
               
               
                  
               
            
         
      
   
   Element equipmentPosition
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  datEquipmentId
               
               
                  Integer
               
               
                  
               
               
                  die DAT-AV Nummer der Sonderausstattung
               
               
                  numerisch
               
               
                  X
               
            
            
               
                  devaluationType
               
               
                  String
               
               
                  
               
               
                  Abwertungsart der Ausstattung;Eine Vorgabe wird nur benötigt, falls Sie die DAT-Standardvorgabe überschreiben möchten.
                     
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  residualValue
               
               
                  Decimal
               
               
                  
               
               
                  Restwert der Ausstattung in Euro
               
               
                  numerisch
               
               
                  
               
            
         
      
   
   Element forecastItems
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  forecastItem
               
               
                  forecastItem
               
               
                  
               
               
                  Das Restwertprognose-Element, 0 - n Wiederholungen möglich
               
               
                  
               
               
                  X
               
            
         
      
   
   Element forecastItem
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  ageinMonth
               
               
                  Integer
               
               
                  
               
               
                  Alter in Monaten (ab Erstzulassung)
               
               
                  numerisch [6-72]
               
               
                  X
               
            
            
               
                  mileageperYear
               
               
                  Long
               
               
                  mileageType
               
               
                  Kilometer Laufleistung pro Jahr. Die maximale Laufleistung pro Jahr beträgt derzeit
                     990.000 Kilometer. 
               
               
                  numerisch
               
               
                  bedingt
               
            
            
               
                  mileageTotal
               
               
                  Long
               
               
                  mileageType
               
               
                  Kilometer-Gesamtlaufleistung; die maximale Gesamtlaufleistung ist derzeit auf 200.000
                     Kilometer beschränkt. Die Kilometer-Gesamtlaufleistung darf nicht kleiner als die
                     Kilometerangabe mileage sein.
               
               
                  numerisch
               
               
                  bedingt
               
            
         
      
   
   Element condition
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  numberOfOwners
               
               
                  Integer
               
               
                  Anzahl der Besitzer 
               
               
                  numerisch
               
               
                  
               
            
            
               
                  ownerCorrectionPercent
               
               
                  Decimal
               
               
                  Korrektur durch Anzahl Vorbesitzer in Prozent 
               
               
                  numerisch [0-100]
               
               
                  
               
            
            
               
                  batteryStateOfHealth
               
               
                  Decimal
               
               
                  Ist - State of Health der Batterie
               
               
                  
               
               
                  
               
            
            
               
                  batteryCorr
               
               
                  Decimal
               
               
                  Wertkorrektur der Traktionsbatterie (Netto)
                  Wenn batteryCorr und batteryCorrGross angegeben wurden, wird batteryCorr in der Bewertung berücksichtigt.
                  Nicht möglich für Fahrzeuge mit DatEquipmentId=76
               
               
                  
               
               
                  
               
            
            
               
                  batteryCorrGross
               
               
                  Decimal
               
               
                  Wertkorrektur der Traktionsbatterie (Brutto)
                  Wenn batteryCorr und batteryCorrGross angegeben wurden, wird batteryCorr in der Bewertung berücksichtigt.
                  Nicht möglich für Fahrzeuge mit DatEquipmentId=76
               
               
                  
               
               
                  
               
            
            
               
                  identificationProcedureStateOfHealth
               
               
                  String
               
               
                  Identifikationsverfahren des Ist - State of Health
                  nur möglich, wenn batteryStateOfHealth gesetzt wurde
