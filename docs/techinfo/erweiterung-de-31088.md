---
title: "Erweiterung der Funktionen getSparePartsDetails(), getSparePartsDetailsByVIN(), getSparePartsDetailsForDPN() und getSparePartsDetailsForDPNByVIN()"
topic_id: "31088"
breadcrumb: "Technische Informationen > Ausgabe Nr. 93 September 2025 > Reparaturkostenkalkulation > SilverDAT calculatePro/SilverDAT calculateItalia > Erweiterungen > Erweiterung der Funktionen getSparePartsDetails(), getSparePartsDetailsByVIN(), getSparePartsDetailsForDPN() und getSparePartsDetailsForDPNByVIN()"
---

# Erweiterung der Funktionen getSparePartsDetails(), getSparePartsDetailsByVIN(), getSparePartsDetailsForDPN() und getSparePartsDetailsForDPNByVIN()

Mit dem September Release 2025 werden die Funktionen getSparePartsDetails(), getSparePartsDetailsForDPN(), getSparePartsDetailsByVIN() und getSparePartsDetailsForDPNByVIN() um folgenden Parameter erweitert:

Anfrage - getSparePartsDetails() und getSparePartsDetailsForDPN()

<request><settings>

| Name | Typ | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| <finisNumber> | Boolean | [true | false]    true: Es wird die FINIS-Ersatzteilenummer zurückgegeben.    false: Es wird eine Ford-Katalognummer zurückgegeben. | Steuerung, ob die FINIS-Ersatzteilenummer oder die Ford-Katalognummer in der Response zurückgegeben wird. |

Anfrage - getSparePartsDetailsByVIN() und getSparePartsDetailsForDPNByVIN()

<request>

| Name | Typ | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| <finisNumber> | Boolean | [true | false]    true: Es wird die FINIS-Ersatzteilenummer zurückgegeben.    false: Es wird eine Ford-Katalognummer zurückgegeben. | Steuerung, ob die FINIS-Ersatzteilenummer oder die Ford-Katalognummer in der Response zurückgegeben wird. |

Rückgabe

Der Node sparePartsInformation wird um folgendes Element erweitert:

<sparePartsInformations><sparePartsInformation>

| Element | Typ | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| <finisNumber> | Boolean | [true | false]    true: Es handelt sich um eine FINIS-Ersatzteilenummer.    false: Es handelt sich um eine Ford-Katalognummer. | Rückgabe, ob es sich um eine FINIS-Ersatzteilnummer oder um eine Ford-Katalognummer handelt. |

Weitere Informationen finden Sie in unserem Kompendium unter: [getSparePartsDetails()](#showid/17314 "Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie"), [getSparePartsDetailsByVIN](#showid/17318 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie")(), [getSparePartsDetailsForDPN()](#showid/17322 "Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie "),  [getSparePartsDetailsForDPNByVIN()](#showid/17326 "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie ") und [SparePartsInformation](#showid/17192 "SparePartsInformation").
