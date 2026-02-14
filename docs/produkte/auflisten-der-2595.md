---
title: "Auflisten der Vorlagen"
topic_id: "2595"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Auflisten von Informationen innerhalb einer Kundennummer > Auflisten der Vorlagen"
---

# Auflisten der Vorlagen

Die Funktion listTemplates listet entsprechend nach [Vorlagentyp](#showid/2597 "Vorlage Typen (templateTypes)") die vorhandenen Vorlagen auf und gibt diese jeweils mit Vorlagenname, Vorlagen ID,
Vorlagen Typ als Liste zurück.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| templateTypes | Datentyp | custom, offlineOpen, onlineOpen, offlineUpload, glassInvoiceRates, glassAdminInvoiceRates, calculation, contactPerson, vro\_calculation, test, companyData, manualPosition, operationSupply, wagesSettings, userSettings, vro\_fi\_calculation, GDVRelease2000, GDVRelease2003, legend, vro\_domus\_calculation | Liste aller Vorlagen Typen die aufgelistet werden können. | X |

Rückgabe

Liste der gefilterten Vorlagen.

Beispiel

```
/* 1 */
MyClaimExternalService_Service mycExtService_service = new MyClaimExternalService_Service();
MyClaimExternalService myClaimExternalService = mycExtService_service.getMyClaimExternalServicePort();

/* 2 */
final String JAVAX_XML_REQUEST_HEADERS = "javax.xml.ws.http.request.headers";
BindingProvider bindingProviderMyClaimExternalService = (BindingProvider) myClaimExternalService;
Map<String, List<String>> reqHeadersMyClaimExternalService = (Map<String,List<String>>) bindingProviderMyClaimExternalService.getRequestContext().get( JAVAX_XML_REQUEST_HEADERS );
if (reqHeadersMyClaimExternalService == null) {
  reqHeadersMyClaimExternalService = new HashMap<String, List<String>>();
  bindingProviderMyClaimExternalService.getRequestContext().put(JAVAX_XML_REQUEST_HEADERS,reqHeadersMyClaimExternalService);
}
bindingProviderMyClaimExternalService.put("Cookie", cookieHeaders);

/* 3 */
String postalCode = "70789";
String customerRole = CustomerRole.EXPERT;
String networkType = NetworkType.MOBILE;  /* ... or another mnemonic from the enum */

final List<String> templateTypes = new LinkedList<String>();
templateTypes.add(FieldSetSource.custom);
templateTypes.add(FieldSetSource.vro_calculation);
List<TemplateOverview> templates = myClaimExternalService.listTemplates(templateTypes);
TemplateOverview template = templates.get(0);

/* access the template details here */
```
