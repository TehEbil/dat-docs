---
title: "Schema verwalten"
topic_id: "10927"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Schema verwalten"
---

# Schema verwalten

Mit der Funktion setProductCheckDetailsList legen Sie die Schemas, Gruppen und Prüfpunkte an. Hierbei kann ein Schema mehrere
Gruppen beinhalten, sowie eine Gruppe mehrere Prüfpunkte beinhalten kann. Einem Schema
kann durch setLinkImageList auch Bilder hinzugefügt werden. Der Parameter Usage wird benötigt um das Schema zu einem bestimmten Produkt zu zuordnen. Mithilfe von
der Funktion getProductCheckDetailsList holen Sie Daten eines Schemas. Mit der Funktion deleteProductCheckDetailsList löschen Sie Schemas, Gruppen und Prüfpunkte.

Beachten Sie, dass nur in der Funktion setProductCheckDetailsList der Parameter Usage gesetzt wird. Wenn Sie den Parameter Usage ändern wollen, müssen Sie das alte Schema löschen und ein neues Schema mit der Funktion
setProductCheckDetailsList erstellen.

- Wenn Sie für Usage den Wert BC angegeben haben, erstellen Sie Daten zum Produkt Grundüberprüfung.
- Wenn Sie für Usage den Wert LR angegeben haben, erstellen Sie Daten zum Produkt Leasingrückgabe.
- Wenn Sie für Usage den Wert CR angegeben haben, erstellen Sie Daten zum Produkt Zustandsbericht. Die Kindelemente
  von ConditionDetails sind nur für das Produkt Zustandsbericht verfügbar.
