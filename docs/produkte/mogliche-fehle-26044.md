---
title: "Mögliche Fehlercodes beim Aufruf der Oberflächen-Schnittstelle"
topic_id: "26044"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Integration der Oberfläche > Aufruf der Methoden der SilverDAT 3 Mietwagenspiegel Oberflächeintegration > Mögliche Fehlercodes beim Aufruf der Oberflächen-Schnittstelle"
---

# Mögliche Fehlercodes beim Aufruf der Oberflächen-Schnittstelle

| Fehlertyp | Fehlercode | Fehlertext | Beschreibung |
| --- | --- | --- | --- |
| Authorization Exception | authorization.login.failed | Signature is not valid | Bitte überprüfen Sie die Kunden-Signatur der Anmeldedaten und versuchen Sie es erneut. |
| Authorization Exception | authorization.login.failed | interfacePartnerSignature missing | Bitte überprüfen Sie die Schnittstellenpartner-Nummer und deren Signatur. Bitte kontaktieren Sie [interfaces@dat.eu](mailto:interfaces@dat.eu "Mail DAT interfaces") falls weiterhin Probleme bestehen. |
| Authorization Exception | authorization.login.failed | interfacePartnerNumber or interfacePartnerSignature missing or incorrect | Bitte überprüfen Sie die Schnittstellenpartner-Nummer und deren Signatur. Bitte kontaktieren Sie [interfaces@dat.eu](mailto:interfaces@dat.eu "Mail DAT interfaces") falls weiterhin Probleme bestehen. |
| Validation Exception | common.error.validation.startPage.invalid | Die angefragte Startseite ist ungültig. | Die vorgegebene Startseite wurde nicht gefunden. Bitte überprüfen Sie Vorgabe für die Startseite und versuchen Sie es erneut. |
| Validation Exception | common.error.validation.processes.pageList.invalid | Wenn Sie das Prozesskennzeichen auf 'true' setzen, dann dürfen Sie keine Seitenliste anfragen. | Bitte beachten Sie, dass über die Seitenliste PageList immer nur ein Prozess eingeschränkt werden kann, deshalb ist diese Option nur zulässig, falls Processes nicht gesetzt ist. Bitte überprüfen Sie diese Vorgaben und versuchen Sie es erneut. |
| Validation Exception | common.error.validation.startPage.pageList.invalid | Wenn Sie eine Seitenliste schicken, dann muss die Startseite darin enthalten sein. | Bitte beachten Sie bei Verwendung der Seitenliste PageList, dass die Startseite StartPage auch in der Seitenliste enthalten sein muss. Bitte überprüfen Sie diese Vorgaben und versuchen Sie es erneut. |
| Validation Exception | common.error.validation.page.pageList.invalid | Die Seite 'anyPagename' gehört nicht zum Prozess 'anyProcess'. In der Seitenliste dürfen nur Seiten verwendet werden, die zum gleichen Prozess gehören. | Bitte beachten Sie bei der Verwendung der Seitenliste PageList, dass nur Seiten angegeben werden dürfen die zum gleichen Prozess gehören. Bitte überprüfen Sie Vorgabe für die Seitenliste und versuchen Sie es erneut. |
