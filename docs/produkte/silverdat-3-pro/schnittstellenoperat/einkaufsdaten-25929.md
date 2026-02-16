---
title: "Einkaufsdaten"
topic_id: "25929"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Erfassung von Neufahrzeugen, Tageszulassungen und Vorführfahrzeugen > Einkaufsdaten"
---

# Einkaufsdaten

Für Neufahrzeuge, Tageszulassungen und Vorführfahrzeuge gibt es keinen Einkaufsprozess.

Die Funktionen setPurchaseOffer und setPurchaseData können nicht aufgerufen werden.

Wird versucht die Funktion setPurchaseData aufzurufen, wird folgende Fehlermeldung geworfen:

| Rückgabecode | Fehlertext |
| --- | --- |
| dat:validation.PurchaseData.notAllowed | Der Aufruf der Methode setPurchaseData ist nicht zulässig für Neufahrzeuge, Tageszulassungen und Vorführfahrzeuge |

Wird versucht die Funktion setPurchaseOffer aufzurufen, wird folgende Fehlermeldung geworfen:

| Rückgabecode | Fehlertext |
| --- | --- |
| dat:validation.PurchaseOffer.notAllowed | Der Aufruf der Methode setPurchaseOffer ist nicht zulässig für Neufahrzeuge, Tageszulassungen und Vorführfahrzeuge |
