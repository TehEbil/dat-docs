---
title: "Aufruf der Methoden der SilverDAT 3 Mietwagenspiegel Oberflächeintegration"
topic_id: "26040"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Integration der Oberfläche > Aufruf der Methoden der SilverDAT 3 Mietwagenspiegel Oberflächeintegration"
---

# Aufruf der Methoden der SilverDAT 3 Mietwagenspiegel Oberflächeintegration

Beim Aufruf der SilverDAT 3 Mietwagenspiegel Oberflächen-Schnittstelle müssen bestimmte Parameter übergeben werden. Hierbei werden
      die nachfolgend aufgeführten Angaben grundsätzlich benötigt:
   
      
         Endpunkt der externen Server-Anwendung, die SilverDAT 3 Mietwagenspiegel einbindet ExternalUrl
      
      
         Bezeichnung des Inlineframes IframeName
      
      
         Anmeldeinformationen
      
      
         Sprache Locale
      
      
         Land Country
      
      
         Aufrufziel StartPage
      
   
   Die weiteren Angaben sind von der gewünschten Konfiguration abhängig oder optional.
      Die nötigen Eigenschaften und Methoden für den Aufruf und die Kommunikation werden
      durch das globale Objekt rentalPricesExternal zur Verfügung gestellt. Die grundsätzlichen Angaben müssen immer, die restlichen je
      nach Bedarf gesetzt werden. Die weiteren Details finden Sie unter Aufbereitung der Eingabeparameter. Die Angabe ihrer Host-URL wird immer benötigt, ebenso wird der Name beziehungsweise
      die ID des iframe benötigt. Die Anmeldeinformationen sind ebenfalls Grundvoraussetzung, die zugehörige
      Beschreibung finden Sie unter Aufbereitung der Authentifizierungsinformationen. Anschließend müssen Sie noch mindestens die entsprechenden Vorgaben für Sprache,
      Land und Aufrufziel angeben. Bitte verwenden Sie zur Fehlerbehandlung bei der Anmeldung
      die Methode setOnLoginFailure. Mit der Methode setOnExecuteSuccess führen Sie die Aktionen nach einer abgeschlossenen Aktion durch. Mit der Methode
      execute führen Sie den eigentlichen Aufruf durch.
   Übersicht der benötigten Angaben,Methoden und Eigenschaften
   
      
         
            
               
                  Name
               
               
                  Methode/Eigenschaft von rentalPricesExternal 
               
               
                  Datentyp
               
               
                  Bedeutung
               
               
                  Abhängigkeit mit
               
               
                  Pflicht
               
            
            
               
                  ExternalUrl
               
               
                  setExternalUrl
               
               
                  String
               
               
                  Host-URLDie Host-URL ist der Endpunkt ihrer Webserver-Anwendung, diese Angabe wird zur Kommunikation
                     von SilverDAT 3 Mitwagenspiegel mit ihrer Anwendung benötigt.
               
               
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
               
               
                  AnmeldungMit den Anmeldeinformationen melden Sie sich über die Schnittstelle an SilverDAT 3 Mietwagenspiegel an. Die Beschreibung dieser Parameter finden Sie unter Aufbereitung der Authentifizierungsinformationen. Bitte beachten Sie, dass mit dem jeweiligen Login unterschiedliche Einschränkungen
                     durch die Berechtigungsvergabe in der Systemkonfiguration verbunden sein können.
               
               
                  CountryStartPagePageList
               
               
                  X
               
            
            
               
                  Locale
               
               
                  setLocale
               
               
                  String
               
               
                  SpracheMit dem Sprachkürzel (Language) steuern Sie die Sprache, die zur Darstellung der SilverDAT 3 Mietwagenspiegel Oberfläche verwendet wird, zum Beispiel de_DE. Diese Vorgabe ist führend und verhält sich entsprechend der Sprachumschaltung in der
                     Oberfläche.
               
               
                  
               
               
                  X
               
            
            
               
                  Country
               
               
                  setCountry
               
               
                  String
               
               
                  LandLandeskürzel für den Zielmarkt; ISO 3166 ALPHA-2, zum Beispiel DE. Bitte beachten Sie, dass Sie nur Datenländer verwenden können, die für den Benutzer
                     freigeschaltet sind.
               
               
                  Login
               
               
                  X
               
            
            
               
                  StartPage
               
               
                  setStartPage
               
               
                  String
               
               
                  AufrufzielDas Aufrufziel ist der wichtigste Parameter zur Steuerung der Oberflächen-Schnittstelle,
                     je nach Vorgabe sind unterschiedliche Aktionen und Seitenaufrufe möglich. Die Beschreibung
                     finden Sie unter Aufrufziele. Bitte beachten Sie bei Verwendung von PageList, dass die in StartPage angegebene Seite enthalten sein muss.
               
               
                  LoginPageList
               
               
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
                     
                  
               
               
                  LoginStartPageWorkflowProcesses
               
               
                  
               
            
            
               
                  DatGroupHeader
               
               
                  setDatGroupHeader
               
               
                  Boolean
               
               
                  Kopfzeile, Mit dem Parameter DatGroupHeader="true" steuern Sie, ob die DAT Group Kopfzeile angezeigt werden soll.
               
               
                  
               
               
                  
               
            
            
               
                  Workflow
               
               
                  setWorkflow
               
               
                  Boolean
               
               
                  Navigationsberechtigung, Mit der Option Workflow bestimmen Sie, ob der Benutzer innerhalb des in StartPage vorgegebenen Prozesses navigieren darf. Falls Processes zulässig ist, muss auch die Berechtigung für Workflow gesetzt sein.
               
               
                  LoginStartPagePageListProcesses
               
               
                  
               
            
            
               
                  Processes
               
               
                  setProcesses
               
               
                  Boolean
               
               
                  Prozesseflag, Berechtigung, ob der Benutzer innerhalb der freigegebenen Prozesse navigieren darf.Berechtigung zur Nutzung weiterer Prozesse. Diese Berechtigung ist nur dann zulässig,
                     wenn auch die Berechtigungen für Workflow und für Save gesetzt sind.
               
               
                  LoginStartPageWorkflowPageList
               
               
                  bedingt
               
            
            
               
                  Save
               
               
                  setSave
               
               
                  Boolean
               
               
                  Speicherflag, 
               
               
                  Processes
               
               
                  
               
            
            
               
                  Mode
               
               
                  setMode
               
               
                  String
               
               
                  Die Modeumschaltung ist nur für DAT-interne Zwecke vorgesehen.
               
               
                  
               
               
                  
               
            
            
               
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
               
               
                  
               
               
                  
               
            
            
               
                  
               
               
                  execute
               
               
                  
               
               
                  Methode zum Aufrufen der SilverDAT 3 Mietwagenspiegel Oberfläche mit den vorgegebenen Parametern.
               
               
                  
               
               
                  X
               
            
            
               
                  
               
               
                  ready
               
               
                  
               
               
                  Bereitschaftsanzeige; Methode zur Abfrage, ob die Initialisierung erfolgreich durchgeführt wurde.
