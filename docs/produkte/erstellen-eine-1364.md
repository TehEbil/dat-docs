---
title: "Erstellen eines neuen Auftrags"
topic_id: "1364"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Erstellen eines neuen Auftrags"
---

# Erstellen eines neuen Auftrags

Mit der Funktion createOrUpdateContract kann ein neuer Auftrag erstellt oder ein bereits vorhandener aktualisiert werden.

Die Unterscheidung ob ein neuer Auftrag erstellt oder ein vorhandener aktualisiert
wird, erfolgt durch das Setzen oder Weglassen des Parameters contractId.

Für die Erstellung eines Auftrags werden mindestens der Auftragstyp (contractType), Netzwerktyp (networkType) und das Dossier Element benötigt.

Das nachfolgende Beispiel zeigt ein Dossier Element mit den Pflichtfeldern, die mindestens benötigt werden.

Beispiel:

```
         <ns2:Dossier>
            <ns2:Name>Claim name</ns2:Name>       
            <ns2:Country>DE</ns2:Country>
            <ns2:Language>de</ns2:Language>
            <ns2:Currency>EUR</ns2:Currency>
         </ns2:Dossier>
```

Hinweis

Aufgrund der Tatsache das ein myclaim Anwender in verschiedenen Netzen Teilhaber sein
kann, wird durch das Setzen des Parameters networkType bestimmt in welches Netz ein Auftrag erstellt werden soll. Soll beispielsweise ein
Auftrag in das SD3 Netz erstellt werden so bekommt der Parameter networkType den Wert „DAT“. Da myclaim mittlerweile eine große Anzahl an verschiedenen Netzen beinhaltet, können die entsprechenden
Netzwerktypen mithilfe der Funktion [listAvailableNetworkTypes](#showid/9283 "Auflisten der vorhandenen Netzwerktypen") erfragt werden..

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | ID des Auftrags (wird benötigt für die Aktualisierung eines bestehenden Auftrags) |  |
| contractType | String | vro\_calculation,  glass | Gängigste Auftragstypen    - vro\_calculation für Fahrzeuginstandsetzungskalkulationen    - glass für reine Glaskalkulationen | X |
| networkType | String | DAT | Konstante eines bestimmten myclaim Netzes    - DAT für SD3 | X |
| Dossier | Dossier |  | Element das die Vehicle eXchange Struktur (VXS) beinhaltet | X |
| templateId | Long |  | ID der Auftragsvorlage |  |
| templateData | HashMap<String, Object> |  | Bereich bei dem Benutzerdefinierte Vorlagendaten |  |
| complexTemplateData | ComplexTemplateData |  |  |  |

Rückgabe

ID (Auftrags ID) des neu erstellten bzw. aktualisierten Auftrags.
