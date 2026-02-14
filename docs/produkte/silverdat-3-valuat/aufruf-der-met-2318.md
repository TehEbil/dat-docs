---
title: "Aufruf der Methoden von SilverDAT 3 valuateExpert Oberflächeintegration"
topic_id: "2318"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Integration der Oberfläche > Aufruf der Methoden von SilverDAT 3 valuateExpert Oberflächeintegration"
---

# Aufruf der Methoden von SilverDAT 3 valuateExpert Oberflächeintegration

Beim Aufruf der SilverDAT 3 valuateExpert/PlusPartner Oberflächen-Schnittstelle müssen bestimmte Parameter übergeben werden. Hierbei werden
      die nachfolgend aufgeführten Angaben grundsätzlich benötigt:
   
      
         Endpunkt der externen Server-Anwendung, die SilverDAT 3 valuateExpert/PlusPartner einbindet ExternalUrl
      
      
         Bezeichnung des Inlineframes IframeName
      
      
         Anmeldeinformationen
      
      
         Produktvariante: valuateNG.expert, valuateNG.expertPlusPartner
      
      
         Sprache Locale
      
      
         Land Country
      
      
         Aufrufziel StartPage
      
   
   Die weiteren Angaben sind von der gewünschten Konfiguration abhängig oder optional.
      Die nötigen Eigenschaften und Methoden für den Aufruf und die Kommunikation werden
      durch das globale Objekt valuateNGExternal zur Verfügung gestellt. Die grundsätzlichen Angaben müssen immer, die restlichen
      je nach Bedarf gesetzt werden. Die weiteren Details finden Sie unter Aufbereitung der Eingabeparameter. Die Angabe ihrer Host-URL wird immer benötigt, ebenso wird der Name beziehungsweise
      die ID des iframe benötigt. Die Anmeldeinformationen sind ebenfalls Grundvoraussetzung, die zugehörige
      Beschreibung finden Sie unter Aufbereitung der Authentifizierungsinformationen. Anschließend müssen Sie noch mindestens die entsprechenden Vorgaben für Sprache,
      Land und Aufrufziel angeben. Bitte verwenden Sie zur Fehlerbehandlung bei der Anmeldung
      die Methode setOnLoginFailure. Mit der Methode setOnExecuteSuccess führen Sie die Aktionen nach einer abgeschlossenen Aktion durch. Mit der Methode
      execute führen Sie den eigentlichen Aufruf durch und mit der Methode getDossier können Sie die VXS-Daten des betreffenden Vorgangs abholen.
   Übersicht der benötigten Angaben,Methoden und Eigenschaften
   
      
         
            
               
                  Name
               
               
                  Methode/Eigenschaft von valuateNGExternal
               
               
                  Datentyp
               
               
                  Bedeutung
               
               
                  Abhängigkeit mit
               
               
                  Pflicht
               
            
            
               
                  ExternalUrl
               
               
                  setExternalUrl
               
               
                  String
               
               
                  Host-URLDie Host-URL ist der Endpunkt ihrer Webserver-Anwendung, diese Angabe wird zur Kommunikation
                     von SilverDAT 3 valuateExpert/PlusPartner mit ihrer Anwendung benötigt.
               
               
                  OnExecuteSuccessOnExecuteFailure
               
               
                  X
               
            
            
               
                  IframeName
               
               
                  setIframeName
               
               
                  String
               
               
                  InlineframeDer Name beziehungsweise die ID des Inlineframe iframe wird benötigt, um dem verwendeten iframe einen eindeutigen Bezeichner zu vergeben. 
               
               
                  
               
               
                  X
               
            
            
               
                  SessionAuthentication
               
               
                  setSessionAuthentication
               
               
                  Boolean
               
               
                  AnmeldeartMit SessionAuthentication steuern Sie die Anmeldeart. Sie können sich entweder mit einer gültigen SessionID des Authentication-Services anmelden oder direkt beim Aufruf über die Anmeldeparameter
                     authentifizieren. 
               
               
                  Login
               
               
                  
               
            
            
               
                  Login
               
               
                  login
               
               
                  String
               
               
                  AnmeldungMit den Anmeldeinformationen melden Sie sich über die Schnittstelle an SilverDAT 3 valuateExpert/PlusPartner an. Die Beschreibung dieser Parameter finden Sie unter Aufbereitung der Authentifizierungsinformationen. Bitte beachten Sie, dass mit dem jeweiligen Login unterschiedliche Einschränkungen
                     durch die Berechtigungsvergabe in der Systemkonfiguration verbunden sein können.
               
               
                  CountryStartPagePageList
               
               
                  X
               
            
            
               
                  Locale
               
               
                  setLocale
               
               
                  String
               
               
                  SpracheMit dem Sprachkürzel (Language) steuern Sie die Sprache, die zur Darstellung der SilverDAT 3 valuateExpert/PlusPartner Oberfläche verwendet wird, zum Beispiel en_US. Diese Vorgabe ist führend und verhält sich entsprechend der Sprachumschaltung in der
                     Oberfläche. Die entsprechende Vorgabe eines über die DossierId ausgewählten Vorgangs, oder derjenige im übergebenen Dossier wird ignoriert.
               
               
                  
               
               
                  X
               
            
            
               
                  Country
               
               
                  setCountry
               
               
                  String
               
               
                  LandLandeskürzel für den Zielmarkt; ISO 3166 ALPHA-2, zum Beispiel ES. Diese Vorgabe ist nachrangig und wird von dem Wert eines über die DossierId ausgewählten Vorgangs, beziehungsweise der im übergebenen Dossier angegebenen ist überschrieben.Bitte beachten Sie, dass Sie nur Datenländer verwenden können, die für den Benutzer
                     freigeschaltet sind.
               
               
                  LoginDossierIdDossier
               
               
                  X
               
            
            
               
                  StartPage
               
               
                  setStartPage
               
               
                  String
               
               
                  AufrufzielDas Aufrufziel ist der wichtigste Parameter zur Steuerung der Oberflächen-Schnittstelle,
                     je nach Vorgabe sind unterschiedliche Aktionen und Seitenaufrufe möglich. Die Beschreibung
                     finden Sie unter Aufrufziele. Bitte beachten Sie bei Verwendung von PageList, dass die in StartPage angegeben Seite enthalten sein muss. Bitte beachten Sie auch, dass die in StartPage verwendete Seite in der Systemkonfiguration für den betreffenden Benutzer freigegeben
                     sein muss.
               
               
                  LoginPageListDossierIdDossier
               
               
                  X
               
            
            
               
                  PageList
               
               
                  setPageList
               
               
                  String
               
               
                  SeitenlisteMit der Seitenliste können Sie die für den Anwender zugänglichen Seiten einschränken.
                     Wenn Sie diesen Parameter nicht setzen, kann der Anwender alle zur Verfügung stehenden
                     Seiten nutzen.Bitte beachten Sie die nachfolgenden Punkte bei der Verwendung der Seitenliste:
                  
                     
                        keine Vorgabe bedeutet keine Einschränkung.
                     
                     
                        Workflow muss auf true gesetzt sein.
                     
                     
                        Processes muss auf false gesetzt sein.
                     
                     
                        die in StartPage angegebene Seite muss enthalten sein.
                     
                     
                        die angegebenen Seiten müssen in der Systemkonfiguration für den betreffenden Benutzer
                           freigegeben sein.
                     
                  
               
               
                  LoginStartPageWorkflowProcesses
               
               
                  
               
            
            
               
                  DossierId
               
               
                  setDossierId
               
               
                  Integer
               
               
                  Eindeutige Vorgangskennung; Die Angabe einer DossierId ist bei den Aufrufzielen von overview.eventlist und valuation.create nicht zulässig, bei allen anderen Aufrufzielen ist sie Pflicht, falls kein Dossier übergeben wurde.Nur der Wert von Locale ist für die Spracheinstellung relevant.Die gleichzeitige Angabe eines Dossier und einer DossierId ist nicht zulässig.
               
               
                  StartPageDossierLocale
               
               
                  bedingt
               
            
            
               
                  Dossier
               
               
                  setDossier
               
               
                  Integer
               
               
                  Dossier, VXS-VorgangsdatenDie Angabe eines Dossiers ist bei den Aufrufzielen von overview.eventlist und valuation.create nicht zulässig, bei allen anderen Aufrufzielen ist sie Pflicht, falls keine DossierId angegeben wurde.Nur der Wert von Locale ist für die Spracheinstellung relevant.Die gleichzeitige Angabe von Dossier und DossierId ist nicht zulässig.
               
               
                  StartPageDossierIdLocale
               
               
                  bedingt
               
            
            
               
                  DatGroupHeader
               
               
                  setDatGroupHeader
               
               
                  Boolean
               
               
                  Kopfzeile, Mit dem Parameter DatGroupHeader="true" steuern Sie, ob die DAT Group Kopfzeile angezeigt werden soll.
               
               
                  
               
               
                  
               
            
            
               
                  Workflow
               
               
                  setWorkflow
               
               
                  Boolean
               
               
                  Navigationsberechtigung, Mit der Option Workflow bestimmen Sie, ob der Benutzer innerhalb des in StartPage vorgegebenen Prozesses navigieren darf. Falls Processes zulässig ist, muss auch die Berechtigung für Workflow gesetzt sein. Bitte beachten Sie, dass hierbei nur diejenigen Seiten angesprungen
                     werden können, die für diesen Benutzer in der Systemkonfiguration freigegeben wurden
                     und in der PageList aufgelistet sind.
               
               
                  LoginStartPagePageListProcesses
               
               
                  
               
            
            
               
                  Processes
               
               
                  setProcesses
               
               
                  Boolean
               
               
                  Prozesseflag, Berechtigung, ob der Benutzer innerhalb der freigegebenen Prozesse navigieren darf.Berechtigung zur Nutzung weiterer Prozesse. Diese Berechtigung ist nur dann zulässig,
                     wenn auch die Berechtigungen für Workflow und für Save gesetzt sind. Bitte beachten Sie, dass nur die Prozesse verwendet werden können,
                     die in der Systemkonfiguration freigegeben sind.
               
               
                  LoginStartPageSaveWorkflowPageList
               
               
                  bedingt
               
            
            
               
                  Save
               
               
                  setSave
               
               
                  Boolean
               
               
                  Speicherflag, Berechtigung zum Speichern des Vorgangs im System.Pflicht falls Workflow gesetzt ist.
               
               
                  Processes
               
               
                  bedingt
               
            
            
               
                  Mode
               
               
                  setMode
               
               
                  String
               
               
                  Die Modeumschaltung ist nur für DAT-interne Zwecke vorgesehen.
               
               
                  
               
               
                  
               
            
            
               
                  VehicleIdentNumber
               
               
                  setVehicleIdentNumber
               
               
                  String
               
               
                  Fahrzeugidentifikationsnummer, Mit der Methode setVehicleIdentNumber belegen Sie das Eingabefeld VIN der Modell-Maske vor. Dies ist nur beim Aufrufziel valuation.create zulässig.
               
               
                  setStartPage
               
               
                  
               
            
            
               
                  VehicleIdentNumberRequest
               
               
                  setVehicleIdentNumberRequest
               
               
                  String
               
               
                  Aufruf der VIN-Abfrage, Mit der Methode setVehicleIdentNumberRequest bestimmen Sie, ob die VIN-Abfrage ausgeführt werden soll. Dies ist nur beim Aufrufziel valuation.create zulässig.
               
               
                  setStartPage
               
               
                  
               
            
            
               
                  Name
               
               
                  setName
               
               
                  String
               
               
                  VorgangsnameMit der Methode setName belegen Sie das Eingabefeld Vorgangsname der Auftragseröffnungsmaske vor.
               
               
                  setStartPage
               
               
                  
               
            
            
               
                  InitialRegistration
               
               
                  setInitialRegistration
               
               
                  Date
               
               
                  Erstzulassungsdatum,Mit der Methode setInitialRegistration belegen Sie das Eingabefeld Erstzulassung der Modell-Maske vor. Dies ist nur beim Aufrufziel valuation.create zulässig.
               
               
                  setStartPage
               
               
                  
               
            
            
               
                  MileageEstimated
               
               
                  setMileageEstimated
               
               
                  Integer
               
               
                  Kilometerstand, Mit der Methode setMileageEstimated belegen Sie das Eingabefeld Laufleistung (km) der Modell-Maske vor. Dies ist nur beim Aufrufziel valuation.create zulässig.
               
               
                  setStartPage
               
               
                  
               
            
            
               
                  MileageType
               
               
                  setMileageType
               
               
                  String
               
               
                  Art des Kilometerstandes,Mit der Methode setMileageType bestimmen Sie, ob der Kilometerstand abgelesen (FromTacho), geschätzt (Estimated) oder angegeben (Indicated) wurde. 
               
               
                  
               
               
                  
               
            
            
               
                  KbaNumber
               
               
                  setKbaNumber
               
               
                  String
               
               
                  KBA-Fahrzeugschlüssel im Format HSN/TSN, Mit der Methode setKbaNumber belegen Sie das Eingabefeld KBA der Modell-Maske vor. Dies ist nur beim Aufrufziel valuation.create zulässig.
               
               
                  setStartPage
               
               
                  
               
            
            
               
                  DatECode
               
               
                  setDatECode
               
               
                  String
               
               
                  DAT €uropa-Code®, Mit der Methode setDatECode belegen Sie das Eingabefeld DAT €uropa-Code® der Modell-Maske vor. Dies ist nur beim Aufrufziel valuation.create zulässig.
               
               
                  setStartPage
               
               
                  
               
            
            
               
                  Container
               
               
                  setContainer
               
               
                  Integer
               
               
                  Marktindex, Mit der Methode setContainer belegen Sie das Eingabefeld Marktindex der Modell-Maske vor.Dies ist nur beim Aufrufziel valuation.create zulässig.
               
               
                  setStartPage
               
               
                  
               
            
            
               
                  ConstructionTime
               
               
                  setConstructionTime
               
               
                  Integer
               
               
                  Bauzeit in DAT-Verschlüsselung, Mit der Methode setConstructionTime belegen Sie das Eingabefeld Bauzeit der Modell-Maske vor. Dies ist nur beim Aufrufziel valuation.create zulässig.
               
               
                  setStartPage
               
               
                  
               
            
            
               
                  WithoutVinQueryButton
               
               
                  setWithoutVinQueryButton
               
               
                  Boolean
               
               
                  VIN-Abfrage Button wird ausgegraut, wenn der Wert true ist.Defaultwert ist false.Dies ist nur beim Aufrufziel valuation.create zulässig.
               
               
                  
               
               
                  
               
            
            
               
                  ReadOnly
               
               
                  setReadOnly
               
               
                  Boolean
               
               
                  Der Vorgang wird im Lesemode geöffnet, wenn der Wert true ist. Diese Aktion ist nur beim Aufruf eines bestehenden Vorgangs zulässig. Zulässige Aufrufziele
                     sind: valuation.contractOpening, valuation.model, valuation.equipment, valuation.condition und valuation.historyValuation. Es wird nur die vorgegebene Aufrufseite angezeigt.
                  Die Eigenschaften setProcesses, setWorkflow und setSave müssen auf false gesetzt sein.
               
               
                  setStartPagesetWorkflowsetProcessessetSave
               
               
                  
               
            
            
               
                  IsDisengaged
               
               
                  setIsDisengagedN
               
               
                  Boolean
               
               
                  Umschalten zum freien AktenzeichenWenn der Wert true ist, wird ein freies Aktenzeichen erstellt. Siehe Kapitel Freies Aktenzeichen für mehr Informationen.Wenn der Wert false ist, wird ein Standardvorgang erstellt. Defaultwert ist false.Dies ist nur beim Aufrufziel valuation.create zulässig.
               
               
                  
               
               
                  
               
            
            
               
                  FlapVisible
               
               
                  setFlapVisible
               
               
                  Boolean
               
               
                  Steuerungsflag für Flaps, Mit der Methode setFlapVisible blenden Sie die seitlichen Flaps der Benutzeroberfläche aus.
               
               
                  
               
               
                  
               
            
            
               
                  OnLoginSuccess
               
               
                  setOnLoginSuccess
               
               
                  
               
               
                  Callback-MethodeMethode zur Weiterverarbeitung nach erfolgreicher Anmeldung. 
               
               
                  
               
               
                  X
               
            
            
               
                  OnLoginFailure
               
               
                  setOnLoginFailure
               
               
                  
               
               
                  Callback-MethodeMethode zur Fehlerbehandlung bei der Anmeldung.
               
               
                  
               
               
                  
               
            
            
               
                  OnExecuteSuccess
               
               
                  setOnExecuteSuccess
               
               
                  
               
               
                  Callback-MethodeMit der Methode setOnExecuteSuccess legen Sie die weitere Verarbeitung fest, die nach dem erfolgreichem Abschluss der
                     Eingaben an der Oberfläche durchgeführt wird. Diese Methode wird mit dem Klick auf
                     den Beenden-Button aufgerufen. 
               
               
                  ExternalUrl
               
               
                  X
               
            
            
               
                  OnExecuteFailure
               
               
                  setOnExecuteFailure
               
               
                  
               
               
                  Callback-Methode für FehlerbehandlungMit der Methode setOnExecuteFailure legen Sie die weitere Verarbeitung fest, die bei einem fehlerhaften Abbruch der Eingaben
                     an der Oberfläche durchgeführt wird.
               
               
                  ExternalUrl
               
               
                  
               
            
            
               
                  Logout
               
               
                  OnLogout
               
               
                  
               
               
                  Callback-MethodeMethode zur Behandlung des Session-Timeouts.
               
               
                  
               
               
                  
               
            
            
               
                  OnLogoutSuccess
               
               
                  setOnLogoutSuccess
               
               
                  
               
               
                  Callback-MethodeMethode zur Weiterverarbeitung nach erfolgreicher Abmeldung.
               
               
                  
               
               
                  
               
            
            
               
                  OnLogoutFailure
               
               
                  setOnLogoutFailure
               
               
                  
               
               
                  Callback-MethodeMethode zur Fehlerbehandlung nach fehlerhafter Abmeldung.
               
               
                  
               
               
                  
               
            
            
               
                  Dossier
               
               
                  getDossier
               
               
                  
               
               
                  Dossier, VXS-Vorgangsdaten; Mit dieser Methode holen Sie die VXS-Vorgangsdaten des aktuellen Vorgangs ab.Bitte beachten Sie, dass dies bei dem Aufrufziel overview.eventlist nicht zulässig ist.
               
               
                  
               
               
                  
               
            
            
               
                  
               
               
                  execute
               
               
                  
               
               
                  Methode zum Aufrufen der SilverDAT 3 valuateExpert/PlusPartner Oberfläche mit den vorgegebenen Parametern.
               
               
                  
               
               
                  X
               
            
            
               
                  
               
               
                  ready
               
               
                  
               
               
                  Bereitschaftsanzeige; Methode zur Abfrage, ob die Initialisierung erfolgreich durchgeführt wurde.
