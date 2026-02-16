---
title: "Warnmeldungen beim Anlegen und Ändern von LKW-Bewertungen"
topic_id: "32067"
breadcrumb: "Technische Informationen > Ausgabe Nr. 95 Februar 2026 > Fahrzeugbewertung > valuateExpert/valuateExpertPlusPartner > Erweiterungen > Warnmeldungen beim Anlegen und Ändern von LKW-Bewertungen"
---

# Warnmeldungen beim Anlegen und Ändern von LKW-Bewertungen

Unter Umständen kann es beim Anlegen und Ändern einer Bewertung für einen Lastkraftwagen
dazu kommen, dass die Bewertung des Fahrzeugs und bzw. oder von Ausstattungen nicht
möglich ist. In solchen Fällen wird in der Response zukünftig im Element <Valuation> unter <Warning> eine der folgenden Warnmeldungen ausgegeben:

| Problem | Warnmeldung |
| --- | --- |
| Fahrzeug und Ausstattungen können nicht bewertet werden | Das gewählte Fahrzeug kann nicht mit den Daten der DAT Marktbeobachtung bewertet werden, es ist nur eine manuelle Fahrzeugbewertung über Wertvorgaben durch den Anwender möglich. Zur Bewertung des Fahrzeugs ist die Angabe des Parameters BasePrice2 unter Valuation zwingend notwendig. Dies betrifft aufgrund von fehlenden Herstellerangaben auch die Bewertung von Sonderausstattungen. Die Ausstattungswertermittlung kann nur über manuelle Wertvorgaben durch den Benutzer erfolgen. |
| Ausstattungen können nicht bewertet werden | Aufgrund von fehlenden Neupreisinformationen des Herstellers kann keine Ausstattungswertermittlung nach DAT erfolgen. Die Ausstattungswertermittlung kann nur über manuelle Wertvorgaben durch den Benutzer erfolgen. |

Die Warnmeldungen finden sich im Kompendium unterhalb der Abschnitte zu den möglichen
Fehlercodes beim Anlegen und Ändern von Bewertungen.

Bitte führen Sie entsprechende Anpassungen in Ihren Anwendungen durch, wenn Sie die
neue Funktionalität nutzen möchten.
